# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a>microsoftStoreForBusinessAppAssignmentSettings 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。

继承自 [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|useDeviceContext|布尔值|是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```








