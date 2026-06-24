grep -RIn "EXCLUDED_ARCHS\|ARCHS.*x86_64\|VALID_ARCHS" ios/Podfile ios/Runner.xcodeproj ios/Pods/Pods.xcodeproj ios/Flutter 2>/dev/null

cd ios
rm -rf Pods Podfile.lock
/usr/bin/arch -arm64 pod install
 
