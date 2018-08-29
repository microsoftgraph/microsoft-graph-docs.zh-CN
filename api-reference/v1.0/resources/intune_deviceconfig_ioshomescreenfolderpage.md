# <a name="ioshomescreenfolderpage-resource-type"></a>iosHomeScreenFolderPage 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含主屏幕上的应用的文件夹
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|文件夹页的名称|
|应用|[iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md) 集合|要在文件夹内的页面上显示的应用的集合。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```



