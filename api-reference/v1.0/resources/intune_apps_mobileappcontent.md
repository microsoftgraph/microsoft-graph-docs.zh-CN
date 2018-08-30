# <a name="mobileappcontent-resource-type"></a>mobileAppContent 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppContents](../api/intune_apps_mobileappcontent_list.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md) 集合|列出 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性和关系。|
|[获取 mobileAppContent](../api/intune_apps_mobileappcontent_get.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)|读取 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性和关系。|
|[创建 mobileAppContent](../api/intune_apps_mobileappcontent_create.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)|创建新的 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象。|
|[删除 mobileAppContent](../api/intune_apps_mobileappcontent_delete.md)|无|删除 [mobileAppContent](../resources/intune_apps_mobileappcontent.md)。|
|[更新 mobileAppContent](../api/intune_apps_mobileappcontent_update.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)|更新 [mobileAppContent](../resources/intune_apps_mobileappcontent.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|应用内容版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|files|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 集合|此应用内容版本的文件列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mobileAppContent"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```



