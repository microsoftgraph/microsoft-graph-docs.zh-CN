# <a name="deviceappmanagement-resource-type"></a>deviceAppManagement 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

充当所有设备应用管理功能的容器的单例实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceAppManagement](../api/intune_onboarding_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md)|读取 [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) 对象的属性和关系。|
|[更新 deviceAppManagement](../api/intune_onboarding_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md)|更新 [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) 对象的属性。|
|[syncMicrosoftStoreForBusinessApps 操作](../api/intune_onboarding_deviceappmanagement_syncmicrosoftstoreforbusinessapps.md)|无|将 Intune 帐户与适用于企业的 Microsoft Store 同步|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|适用于企业的 Microsoft Store 的应用上次成功同步帐户的时间。|
|isEnabledForMicrosoftStoreForBusiness|Boolean|帐户是否已启用从适用于企业的 Microsoft Store 同步应用程序。|
|microsoftStoreForBusinessLanguage|String|用于从适用于企业的 Microsoft Store 同步应用程序的区域设置信息。 特定于国家/地区的区域性。 这些区域性的名称遵循 RFC 4646（Windows Vista 和更高版本）。 格式为 <languagecode2>-<country/regioncode2>，其中 <languagecode2> 是从 ISO 639-1 派生的两个小写字母组成的代码，<country/regioncode2> 是从 ISO 3166 派生的两个大写字母组成的代码。 例如，“en-US”（“英语(美国)）是一个特定的区域性。|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|从适用于企业的 Microsoft Store 的应用程序同步上次完成的时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|vppTokens|[vppToken](../resources/intune_onboarding_vpptoken.md) 集合|此组织的 Vpp 令牌列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```



