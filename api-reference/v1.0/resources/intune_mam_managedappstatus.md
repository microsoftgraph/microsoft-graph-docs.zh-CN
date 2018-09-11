# <a name="managedappstatus-resource-type"></a>managedAppStatus 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示组织的应用保护和配置状态。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedAppStatuses](../api/intune_mam_managedappstatus_list.md)|[managedAppStatus](../resources/intune_mam_managedappstatus.md) 集合|列出 [managedAppStatus](../resources/intune_mam_managedappstatus.md) 对象的属性和关系。|
|[获取 managedAppStatus](../api/intune_mam_managedappstatus_get.md)|[managedAppStatus](../resources/intune_mam_managedappstatus.md)|读取 [managedAppStatus](../resources/intune_mam_managedappstatus.md) 对象的属性和关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|状态报告的友好名称。|
|id|字符串|实体的键。|
|version|字符串|实体的版本。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```








