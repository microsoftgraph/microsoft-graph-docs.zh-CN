# <a name="devicecompliancepolicysettingstate-resource-type"></a>deviceCompliancePolicySettingState 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

给定设备的设备符合性策略设置状态。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|setting|字符串|报告的设置|
|settingName|字符串|报告的本地化/用户友好设置名称|
|instanceDisplayName|字符串|报告的设置实例的名称。|
|状态|[complianceStatus](../resources/intune_shared_compliancestatus.md)|设置合规性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。|
|errorCode|Int64|设置的错误代码|
|errorDescription|字符串|错误说明|
|userId|字符串|UserId|
|userName|字符串|UserName|
|userEmail|字符串|UserEmail|
|userPrincipalName|字符串|UserPrincipalName。|
|sources|[settingSource](../resources/intune_deviceconfig_settingsource.md) 集合|参与策略|
|currentValue|字符串|设备上设置的当前值|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



