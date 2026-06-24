killall Xcode 2>/dev/null || true
killall Simulator 2>/dev/null || true
killall com.apple.CoreSimulator.CoreSimulatorService 2>/dev/null || true
open -a Xcode




grep -R "EXCLUDED_ARCHS\|VALID_ARCHS\|ONLY_ACTIVE_ARCH\|ARCHS" ios/Runner.xcodeproj ios/Podfile ios/Pods/Pods.xcodeproj 2>/dev/null
