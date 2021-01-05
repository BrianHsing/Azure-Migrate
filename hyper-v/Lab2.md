# Lab2 - 發現 Hyper-V VM

- 點選「發現」<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/discovery.PNG "discovery")
- 選擇「是，使用 Hyper-V」，輸入 Hyper-V 裝置名稱，並點選「產生金鑰」，完成後請複製並記好，最後，點選「下載」.VHD檔案<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/selectHypervanddownload-update.PNG "selectHypervanddownload")<br>
- 解壓縮 AzureMigrateAppliance.zip，在 Hyper-V Manager 選擇 Import Virtual Machine 匯入<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/importama1.PNG "importama1")<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/importama2.PNG "importama2")<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/importama3.PNG "importama3")<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/importama4.PNG "importama4")<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/importama5.PNG "importama5")<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/completeimportama.PNG "completeimportama")<br>
- 初始化設定 AzureMigrateAppliance_v3.20.05.27 (administrator/isadmin@123)<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/licenseTerms.PNG "licenseTerms")<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/customizeSetting.PNG "customizeSetting")<br>
- 手動設定網路介面 (192.168.0.100/255.255.255.0/192.168.0.1/8.8.8.8)<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/ama-networking-setting.PNG "ama-networking-setting")<br>
- 手動設定 C:\Windows\System32\drivers\etc\host，輸入 192.168.0.1 hyperv，儲存此文件
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/ama-dns-setting.PNG "ama-dns-setting")<br>
- Set up discovery for Azure Migrate<br>
- Browser https://localhost:44368<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/settingweb2.png "settingweb2")<br>
- Set up prerequisites，勾選 Accepted license terms，輸入 Credentials (administrator/isadmin@123)<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/windowsSecurity.PNG "windowsSecurity")<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/completePrep.PNG "completePrep")<br>
- Register with Azure Migrate<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/registerAM.PNG "registerAM")<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/providehost.PNG "providehost")<br>
- Provide Hyper-V hosts details<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/addhosts.PNG "addhosts")<br>
![GITHUB](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/image/completeAM.PNG "completeAM")<br>

[Lab3 - 評定 Hyper-V VM](https://github.com/BrianHsing/Azure-Migrate/blob/master/hyper-v/Lab3.md)<br>