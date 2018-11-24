# <a name="update-deviceappmanagement"></a>更新 deviceAppManagement

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
以下权限之一需要调用此 API。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。  请注意，在相应权限根据工作流而有所不同。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象的 JSON 表示形式。

下表显示创建 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|**入职培训**|
|isEnabledForMicrosoftStoreForBusiness|Boolean|帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。|
|microsoftStoreForBusinessLanguage|String|用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。 特定于国家/地区的区域性。 这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。 格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。 例如，“en-US”（“英语(美国)）是一个特定的区域性。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|从适用于企业的 Microsoft Store 的应用程序同步上次完成的时间。|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。|

## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 对象。

## <a name="example-request"></a>示例请求

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a>响应示例

为简便起见，如下所示的响应对象可能会被截断。 将从实际调用中返回所有属性。

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



