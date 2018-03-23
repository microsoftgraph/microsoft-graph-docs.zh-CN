# <a name="update-managedappstatusraw"></a>更新 managedAppStatusRaw

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

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
PATCH /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象的 JSON 表示形式。

下表显示创建 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|状态报告的友好名称。 继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)|
|id|String|实体的键。 继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)|
|version|String|实体的版本。 继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)|
|content|[Json](../resources/intune_mam_json.md)|状态报告内容。|



## <a name="response"></a>响应
如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
Content-type: application/json
Content-length: 139

{
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "id": "80847581-7581-8084-8175-848081758480",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



