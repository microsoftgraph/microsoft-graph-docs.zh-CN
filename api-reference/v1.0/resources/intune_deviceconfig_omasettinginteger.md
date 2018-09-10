# <a name="omasettinginteger-resource-type"></a>omaSettingInteger 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

OMA 设置整数定义。

继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称。 继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|description|字符串|说明。 继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|omaUri|String|OMA。 继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|值|Int32|值。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```








