# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'LicensePlistTest' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for LicensePlistTest
  pod 'Alamofire'
  pod 'Firebase'
  pod 'LicensePlist'
  target 'LicensePlistTestTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'LicensePlistTestUITests' do
    # Pods for testing
  end

end
post_install do | installer |
  require 'fileutils'
  FileUtils.cp_r('Pods/Target Support Files/Pods-LicensePlistTest/Pods-LicensePlistTest-acknowledgements.plist', 'LicensePlistTest/Settings.bundle/Acknowledgements.plist', :remove_destination => true)
end
