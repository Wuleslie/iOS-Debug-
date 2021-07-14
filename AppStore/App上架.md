#### App Icon

现在上架时，App的图标不在App Store Connect网站上选择文件上传，而是跟Xcode打包上传的build绑定在一起，即在Xcode工程里配置，AppIcon里增加了App Store 1024*1024的尺寸。

#### Preview截图尺寸

这里有[Screenshot specifications](https://help.apple.com/app-store-connect/#/devd274dd925)具体要求。针对iPhone设备，必需的是6.5 inch（1284 x 2778 pixels）、5.5 inch（1242 x 2208 pixels），其他可自行复用这两个尺寸的截图。而iPad则必需3/4代、2代iPad Pro，尺寸均为12.9 inch（2048 x 2732 pixels）。

#### 上架国家与地区

Apple审核通过后，如果立即将App的状态变为Ready for Sale，可能在App Store上搜不到，从Connect应用中点击View on App Store，提示App Not Available，如下图。这时可以确认下自己的App的发放范围，默认是全部国家和地区。如果确认设置无误，那就稍作等待，延迟一会儿（大约半个小时）就能在App Store搜到。有任何问题，可联系[苹果技术支持](https://developer.apple.com/contact/topic/select)，选择自己的问题类型，会有客服致电或者邮件跟进。