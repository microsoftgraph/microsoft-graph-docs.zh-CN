# <a name="omasettingbase64-resource-type"></a>omaSettingBase64 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

OMA 设置 Base64 定义。

继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|显示名称。 继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|说明|字符串|说明。 继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|omaUri|字符串|OMA。 继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)|
|fileName|字符串|与值属性关联的文件名 (*.cer | *.crt | *.p7b | *.bin)。|
|值|字符串|值。 （Base64 编码字符串）|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```








