# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'

begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

require 'motion-cocoapods'

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  # Basic information
  app.name                              = 'Test'
  app.short_version                     = '1.0'
  app.version                           = '1.0'
  app.identifier                        = 'testman.com.test'

  # Versions and orientations
  app.deployment_target                 = '9.0'
  app.device_family                     = [:iphone]
  app.interface_orientations            = [:portrait]

  # app.libs += ['/usr/lib/libicucore.dylib', '/usr/lib/libz.dylib', '/usr/lib/libc++.dylib']
  # app.frameworks += ['CFNetwork', 'Security', 'SystemConfiguration']
  # app.weak_frameworks += ['Accounts', 'Social']

  # app.info_plist['Fabric'] = { 'APIKey' => '1234',
  #   'Kits' => [{'KitInfo' => {
  #   'consumerKey' => '1234',
  #   'consumerSecret' => '1234',
  #   'KitName' => 'Twitter'}}]
  # }
  # app.vendor_project('vendor/Frameworks/Fabric.framework', :static, :products => ['Fabric'], :headers_dir => 'Headers', force_load: true)
  # app.vendor_project('vendor/Frameworks/TwitterCore.framework', :static, :products => ['TwitterCore'], :headers_dir => 'Headers', force_load: true)
  # app.vendor_project('vendor/Frameworks/TwitterKit.framework', :static, :products => ['TwitterKit'], :headers_dir => 'Headers', force_load: true)


  app.pods do
    pod 'Fabric'
    pod 'TwitterKit'
  end
end
