# <a name="windowsinformationprotectionnetworklearningsummary-resource-type"></a>windowsInformationProtectionNetworkLearningSummary 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 信息保护网络学习摘要实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsInformationProtectionNetworkLearningSummaries](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_list.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 集合|列出 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 对象的属性和关系。|
|[获取 windowsInformationProtectionNetworkLearningSummary](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_get.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|读取 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 对象的属性和关系。|
|[创建 windowsInformationProtectionNetworkLearningSummary](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_create.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|创建新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 对象。|
|[删除 windowsInformationProtectionNetworkLearningSummary](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_delete.md)|无|删除 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)。|
|[更新 windowsInformationProtectionNetworkLearningSummary](../api/intune_wip_windowsinformationprotectionnetworklearningsummary_update.md)|[windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md)|更新 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ID|字符串|WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。|
|url|字符串|网站 URL|
|deviceCount|Int32|设备计数|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionNetworkLearningSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "String (identifier)",
  "url": "String",
  "deviceCount": 1024
}
```








