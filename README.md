cask 'eset-cyber-security' do
  version :latest
  sha256 :no_check

  if MacOS.release <= :lion
  else
    url 'https://download.eset.com/com/eset/apps/home/eav/mac/latest/eset_cybersecurity_en_.dmg'
    name 'ESET Cyber Security'
  end
  
  app 'ESET Cyber Security.app'
  
end
