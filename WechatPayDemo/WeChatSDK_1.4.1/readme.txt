
2013.9.23 WeChatSDK_iOS_1.4.1改动:
sendReq:接口支持SendMessageToWXReq类型。
safeSendReq:接口支持SendAuthReq、PayReq类型。
使用OAuth功能的只能调用safeSendReq:接口。

WeChatSDK_iOS_1.4.0说明:
1、libWeChatSDK.a 对应 原开放平台的libWeChatSDK_armv7_armv7s.a。

2、OAuth授权登录流程改变，具体使用文档请找jacobyang

3、废除该接口
/*! @brief 获取当前微信的版本所支持的API最高版本
 *
 * @return 返回微信支持的最高API版本号。
 */
+(NSString *) getWXAppSupportMaxApiVersion;
微信5.0以后，对于微信是否支持某些功能，由微信侧来判断处理。

注：最新SDK支持iOS7分享，请配合线上微信5.0.1使用