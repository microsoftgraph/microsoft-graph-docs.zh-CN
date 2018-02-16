# <a name="user-resource-type"></a>用户资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示 Azure Active Directory 用户对象。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List users](../api/intune_mam_user_list.md)|[user](../resources/intune_mam_user.md) 集合|列出 [user](../resources/intune_mam_user.md) 对象的属性和关系。|
|[获取 user](../api/intune_mam_user_get.md)|[user](../resources/intune_mam_user.md)|读取 [user](../resources/intune_mam_user.md) 对象的属性和关系。|
|[创建 user](../api/intune_mam_user_create.md)|[user](../resources/intune_mam_user.md)|创建新的 [user](../resources/intune_mam_user.md) 对象。|
|[删除 user](../api/intune_mam_user_delete.md)|无|删除 [user](../resources/intune_mam_user.md)。|
|[更新 user](../api/intune_mam_user_update.md)|[user](../resources/intune_mam_user.md)|更新 [user](../resources/intune_mam_user.md) 对象的属性。|
|[getManagedAppDiagnosticStatuses 函数](../api/intune_mam_user_getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md) 集合|获取给定用户的诊断验证状态。|
|[getManagedAppPolicies 函数](../api/intune_mam_user_getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) 集合|获取给定用户的应用限制。|
|[wipeManagedAppRegistrationsByDeviceTag 操作](../api/intune_mam_user_wipemanagedappregistrationsbydevicetag.md)|无|对含有指定设备标记的应用注册发布擦除操作。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户标识符。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md) 集合|属于用户的零个或多个托管的应用注册。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



