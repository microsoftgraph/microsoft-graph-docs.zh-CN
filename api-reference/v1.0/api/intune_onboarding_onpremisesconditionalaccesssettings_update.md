# <a name="update-onpremisesconditionalaccesssettings"></a>更新 onPremisesConditionalAccessSettings

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象的属性。
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
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|授权|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象的 JSON 表示形式。

下表显示创建 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|尚未记录|
|enabled|Boolean|指示是否为该组织启用了本地条件访问|
|includedGroups|Guid 集合|本地条件访问将面向的用户组。 这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。|
|excludedGroups|Guid 集合|将由本地条件访问豁免的用户组。 这些组中的所有用户都将从条件访问策略中豁免。|
|overrideDefaultRule|Boolean|允许设备时重写默认访问规则以确保授予访问。|



## <a name="response"></a>响应
如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 195

{
  "enabled": true,
  "includedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "excludedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "excludedGroups": [
    "79199ed9-e50b-4257-8de4-70b9c8685061"
  ],
  "overrideDefaultRule": true
}
```



