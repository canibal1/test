arch -arm64 xcodebuild test \
  -workspace ios/Runner.xcworkspace \
  -scheme RunnerTests \
  -derivedDataPath code_coverage_results \
  -destination 'platform=iOS Simulator,name=iPhone 17,OS=26.5,arch=arm64' \
  -enableCodeCoverage YES \
  ARCHS=arm64 \
  ONLY_ACTIVE_ARCH=YES
