# <a name="appconfigurationsettingitem-resource-type"></a>appConfigurationSettingItem 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含应用配置设置项的属性。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|appConfigKey|字符串|应用配置密钥。|
|appConfigKeyType|[mdmAppConfigKeyType](../resources/intune_apps_mdmappconfigkeytype.md)|应用配置密钥类型。可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。|
|appConfigKeyValue|字符串|应用配置密钥值。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```








