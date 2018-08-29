# <a name="windowsinformationprotectionapplearningsummary-resource-type"></a>windowsInformationProtectionAppLearningSummary 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 信息保护应用学习摘要实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windowsInformationProtectionAppLearningSummaries](../api/intune_wip_windowsinformationprotectionapplearningsummary_list.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 集合|列出 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 对象的属性和关系。|
|[Get windowsInformationProtectionAppLearningSummary](../api/intune_wip_windowsinformationprotectionapplearningsummary_get.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|读取 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 对象的属性和关系。|
|[Create windowsInformationProtectionAppLearningSummary](../api/intune_wip_windowsinformationprotectionapplearningsummary_create.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|创建新的 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 对象。|
|[Delete windowsInformationProtectionAppLearningSummary](../api/intune_wip_windowsinformationprotectionapplearningsummary_delete.md)|无|删除 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)。|
|[Update windowsInformationProtectionAppLearningSummary](../api/intune_wip_windowsinformationprotectionapplearningsummary_update.md)|[windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md)|更新 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|WindowsInformationProtectionAppLearningSummary 的唯一标识符。|
|applicationName|字符串|应用程序名称|
|applicationType|[applicationType](../resources/intune_wip_applicationtype.md)|应用类型 可取值为：`universal`、`desktop`。|
|deviceCount|Int32|设备计数|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLearningSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "String (identifier)",
  "applicationName": "String",
  "applicationType": "String",
  "deviceCount": 1024
}
```



