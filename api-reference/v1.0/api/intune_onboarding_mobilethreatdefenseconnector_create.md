# <a name="create-mobilethreatdefenseconnector"></a>创建 mobileThreatDefenseConnector

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

创建新的 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象。
## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementServiceConfig.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 mobileThreatDefenseConnector 对象的 JSON 表示形式。

下表显示创建 mobileThreatDefenseConnector 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|lastHeartbeatDateTime|DateTimeOffset|管理员启用“连接到 MTP”选项后的上次检测信号的时间戳|
|partnerState|String|此租户的合作伙伴状态。可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。|
|androidEnabled|Boolean|Android 切换，打开或关闭|
|androidDeviceBlockedOnMissingPartnerData|Boolean|对于 Android，允许管理员配置必须先从数据同步合作伙伴接收到数据才能将其视为符合|
|iosDeviceBlockedOnMissingPartnerData|Boolean|对于 IOS，允许管理员配置必须先从数据同步合作伙伴接收到数据才能将其视为符合|
|partnerUnsupportedOsVersionBlocked|Boolean|允许管理员阻止启用的平台上不符合最低版本要求的设备|
|iosEnabled|Boolean|IOS 切换，打开或关闭|
|partnerUnresponsivenessThresholdInDays|Int32|获取或设置每个租户允许此合作伙伴集成不响应的天数|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



