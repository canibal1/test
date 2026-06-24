cd ios
pod deintegrate
pod install
cd ..
fvm flutter clean
fvm flutter pub get

rm -rf ~/Library/Developer/Xcode/DerivedData/*
killall Xcode 2>/dev/null || true
killall Simulator 2>/dev/null || true
killall com.apple.CoreSimulator.CoreSimulatorService 2>/dev/null || true
open ios/Runner.xcworkspace
