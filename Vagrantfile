require 'vagrant-aws'
Vagrant.configure('2') do |config|
    config.vm.box = 'dummy'
    config.vm.provider 'aws' do |aws, override|
    aws.access_key_id = "AKIAIPANIDC5BWJYD3SA"
    aws.secret_access_key = "elZTI0HbGFJdkQXda6zcxpJ6moz2UErhwmN8wCPM"
    aws.keypair_name = 'MyVPCKeyPair'
    aws.instance_type = 't2.micro'
    aws.region = 'us-east-2'
    aws.ami = 'ami-82f4dae7'
    aws.security_groups = ['default']
    override.ssh.username = 'ubuntu'
    override.ssh.private_key_path = '~/Documents/vagrant/aws/MyVPCKeyPair.pem'
  end
end
