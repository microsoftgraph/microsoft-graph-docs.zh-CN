# <a name="update-androidforworksettings"></a>更新 androidForWorkSettings

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 对象的 JSON 表示形式。

下表显示了创建 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|Android for Work 设置标识符|
|bindStatus|String|使用 Google EMM API 的租户的绑定状态。可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。|
|lastAppSyncDateTime|DateTimeOffset|应用同步的上次完成时间|
|lastAppSyncStatus|String|上次应用程序同步结果。可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。|
|ownerUserPrincipalName|String|创建了企业的所有者 UPN|
|ownerOrganizationName|String|载入 Android for Work 时使用的组织名称|
|lastModifiedDateTime|DateTimeOffset|Android for Work 设置的上次修改时间|
|enrollmentTarget|String|指示哪些用户可以在 Android for Work 设备管理中注册设备。可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。|
|targetGroupIds|String 集合|指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。|



## <a name="response"></a>响应
如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 417

{
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```



