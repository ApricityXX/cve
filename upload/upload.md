NBS&HappySoftWeChat phpwechat has an arbitrary upload vulnerability

official website:http://efamily.gfarmsh.com/

version:NBS&HappySoftWeChat phpwechat 1.1.6 

![WPS图片(1)](https://github.com/ApricityXX/cve/assets/129482555/8eb12095-0edb-452e-83cf-9de0c23ac80d)

http://www.cgw.qhjgsc.com//api/upload/index.php?action=imageupload&originalname=&upload_hidden_val=upload_hidden_valpc_site_logo&upload_file=upload_filepc_site_logo&upload_loading=upload_loadingpc_site_logo&img_demo=img_demopc_site_logo

First upload a picture horse, and then find the upload successful.
![WPS图片(2)](https://github.com/ApricityXX/cve/assets/129482555/6106d81b-ac5e-414e-8454-3a2c5c6b616b)

Then change the file suffix to php for replay requests.
![WPS图片(3)](https://github.com/ApricityXX/cve/assets/129482555/9a9e234f-a125-43e1-91a6-e05fde9876ca)

It is found that the first few digits of the file name after upload are fixed, and the last 5 digits are random digits. Then the explosion.

![WPS图片(4)](https://github.com/ApricityXX/cve/assets/129482555/16ae0d70-536a-457f-b797-f16d8cfa7a92)

Once it's set up, start blasting.
![WPS图片(5)](https://github.com/ApricityXX/cve/assets/129482555/04ac4dc1-0b52-48c6-ba36-bd9589472450)

Finally, the upload was successful.

![WPS图片(6)](https://github.com/ApricityXX/cve/assets/129482555/7845b3aa-f910-4808-8674-af95a42ba788)
