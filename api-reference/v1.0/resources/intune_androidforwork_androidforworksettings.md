# <a name="androidforworksettings-resource-type"></a>androidForWorkSettings 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android for Work 设置。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 androidForWorkSettings](../api/intune_androidforwork_androidforworksettings_get.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|读取 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 对象的属性和关系。|
|[更新 androidForWorkSettings](../api/intune_androidforwork_androidforworksettings_update.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|更新 [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 对象的属性。|
|[requestSignupUrl 操作](../api/intune_androidforwork_androidforworksettings_requestsignupurl.md)|String|生成用于注册 Android for Work 管理的注册 URL。|
|[completeSignup 操作](../api/intune_androidforwork_androidforworksettings_completesignup.md)|无|完成 Android for Work 管理的注册流程。|
|[syncApps 操作](../api/intune_androidforwork_androidforworksettings_syncapps.md)|无|同步企业批准的应用程序。|
|[取消绑定操作](../api/intune_androidforwork_androidforworksettings_unbind.md)|无|禁用企业的 Android for Work 管理。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Android for Work 设置标识符|
|bindStatus|String|使用 Google EMM API 的租户的绑定状态 可取值为：`notBound`、`bound`、`boundAndValidated`、`unbinding`。|
|lastAppSyncDateTime|DateTimeOffset|应用同步的上次完成时间|
|lastAppSyncStatus|String|上次应用程序同步结果 可取值为：`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none`。|
|ownerUserPrincipalName|String|创建了企业的所有者 UPN|
|ownerOrganizationName|String|载入 Android for Work 时使用的组织名称|
|lastModifiedDateTime|DateTimeOffset|Android for Work 设置的上次修改时间|
|enrollmentTarget|String|指示哪些用户可以在 Android for Work 设备管理中注册设备 可取值为：`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions`。|
|targetGroupIds|String collection|指定当 enrollmentTarget 设置为“定向”时可以在 Android for Work 设备管理中注册设备的 AAD 组。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ]
}
```



