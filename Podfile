platform :ios, '13.0'
use_frameworks!

target 'Texture+IGListKit' do
  pod 'Texture/IGListKit+PinRemote-full', :git => 'https://github.com/Zabolotiny/Texture.git', :branch => 'releases/p11.9'
end

post_install do |installer|
  installer.generated_projects.each do |project|
    project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '11.0'
         end
    end
  end
end
