# <a name="managedmobileapp-resource-type"></a>managedMobileApp 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

部署应用的标识符。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedMobileApps](../api/intune_mam_managedmobileapp_list.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md) 集合|列出 [managedMobileApp](../resources/intune_mam_managedmobileapp.md) 对象的属性和关系。|
|[获取 managedMobileApp](../api/intune_mam_managedmobileapp_get.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|读取 [managedMobileApp](../resources/intune_mam_managedmobileapp.md) 对象的属性和关系。|
|[创建 managedMobileApp](../api/intune_mam_managedmobileapp_create.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|创建新的 [managedMobileApp](../resources/intune_mam_managedmobileapp.md) 对象。|
|[删除 managedMobileApp](../api/intune_mam_managedmobileapp_delete.md)|无|删除 [managedMobileApp](../resources/intune_mam_managedmobileapp.md)。|
|[更新 managedMobileApp](../api/intune_mam_managedmobileapp_update.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|更新 [managedMobileApp](../resources/intune_mam_managedmobileapp.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|含有其操作系统类型的应用标识符。|
|id|String|实体的键。|
|version|String|实体版本。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



