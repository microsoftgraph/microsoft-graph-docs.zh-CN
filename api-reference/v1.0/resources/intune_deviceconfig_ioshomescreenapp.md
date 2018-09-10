# <a name="ioshomescreenapp-resource-type"></a>iosHomeScreenApp 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示主屏幕上应用的图标

继承自 [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|继承自 [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) 的应用的名称|
|bundleID|String|应用的 BundleID|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```








