# <a name="managedappregistration-resource-type"></a>managedAppRegistration 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

ManagedAppEntity 是应用管理工作流下所有其他实体类型的基实体类型。
ManagedAppRegistration 资源表示具有管理功能的组织成员使用的应用的详细信息。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List managedAppRegistrations](../api/intune_mam_managedappregistration_list.md)|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) 集合|列出 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) 对象的属性和关系。|
|[Get managedAppRegistration](../api/intune_mam_managedappregistration_get.md)|[managedAppRegistration](../resources/intune_mam_managedappregistration.md)|读取 [managedAppRegistration](../resources/intune_mam_managedappregistration.md) 对象的属性和关系。|
|[getUserIdsWithFlaggedAppRegistration 函数](../api/intune_mam_managedappregistration_getuseridswithflaggedappregistration.md)|String collection|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建日期和时间|
|lastSyncDateTime|DateTimeOffset|上次应用与管理服务同步的日期和时间。|
|applicationVersion|String|应用版本|
|managementSdkVersion|String|应用管理 SDK 版本|
|platformVersion|String|操作系统版本|
|deviceType|String|主机设备类型|
|deviceTag|String|应用管理 SDK 生成的标记，它可帮助关联托管在同一设备上的应用。 不保证在所有情况下与应用关联。|
|deviceName|String|主机设备名称|
|flaggedReasons|[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)集合|标记应用注册的零个或多个原因。 例如， 在取得 root 权限的设备上运行的应用|
|userId|String|此应用注册所属的用户 ID。|
|appIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|应用包标识符|
|id|String|实体的键。|
|版本|String|实体版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|appliedPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合|当已注册的应用上次与管理服务同步时，已应用于该应用的零个或多个策略。|
|intendedPolicies|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合|目前适用于应用的零个或多个策略管理员。|
|操作|[managedAppOperation](../resources/intune_mam_managedappoperation.md) 集合|在应用注册时触发的零个或多个长时间运行的操作。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune_mam_managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
