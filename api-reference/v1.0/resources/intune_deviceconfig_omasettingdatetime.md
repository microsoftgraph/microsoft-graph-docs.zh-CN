# <a name="omasettingdatetime-resource-type"></a>omaSettingDateTime 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

OMA 设置日期时间定义。

继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称。 继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|description|String|说明。 继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|omaUri|String|OMA。 继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|value|DateTimeOffset|值。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.omaSetting",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



