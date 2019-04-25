---
title: secureScoreControlProfiles 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下, 它将返回租户的所有控件, 并可显式提取各个控件。
localization_priority: Normal
ms.openlocfilehash: 3e800271f1ef5f8ac7847d14d97ae6f24f1e01cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549172"
---
# <a name="securescorecontrolprofiles-resource-type"></a>secureScoreControlProfiles 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户的每个控件数据的安全分数。 默认情况下, 它将返回租户的所有控件, 并可显式提取各个控件。


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |读取 secureScoreControlProfiles 对象的属性和元数据。|


## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   租户 ID 的 GUID 字符串。  |
|   controlName |   String  |   控件的名称。 |
|   title   |   字符串  |   控件的标题。   |
| complianceInformation | [complianceInformation](complianceinformation.md)集合 | 与安全得分控制相关联的合规性信息的集合 |
|   controlCategory |   String  |   控制措施类别 (帐户、数据、设备、应用程序、基础结构)。  |
|   actionType  |   String  |   控制操作类型 (Config、审阅、行为)。 |
|   service |   String  |   拥有控件的服务 (Exchange、Sharepoint、Azure AD)。 |
|   maxScore |  String  |   指定日期的当前获得的最大分数。   |
|   单层 |  String  |   控制层 (Core, 纵深防御, 高级。)    |
|   userImpact |    String  | 实施控制的用户影响 (低、中等、高)。    |
|   implementationCost |    String  |   implemmentating 控件的资源成本 (low、适中、high)。 |
|   排名 |  Int32   |   Microsoft 的控制堆栈排名。   |
|   病毒 |   String 集合   |   控制缓解的威胁列表 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗)。 |
|   被 |    布尔值 |   指示是否已对控件进行折旧的标志。   |
|   纠正 |   String  |   对控件将有助于修正的内容的说明。 |
|   remediationImpact | String  |   对修正用户影响的说明。 |
|   actionUrl | String  |   可将控件 actioned 到的位置的 URL。 |
|   controlStateUpdates |   [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合 |    用于指示租户已标记控件的位置的标志 (忽略、thirdParty、已审阅) (支持[更新](../api/securescorecontrolprofiles-update.md))。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScores"
}-->

```json
{
"title": "String", 
"azureTenantId": "Guid", 
"referenceId": "String", 
"controlName": "String", 
"maxScore": "Int32",
"actionCategory": "Collection(microsoft.graph.SecureScore.actionCategory)",
"actionType": "Collection(microsoft.graph.SecureScore.actionType)",
"service": "String",
"tier": "Collection(microsoft.graph.SecureScore.tier)",
"userImpact": "Collection(microsoft.graph.SecureScore.ranking)",
"implementationCost ": "Collection(microsoft.graph.SecureScore.ranking)",
"rank ": "Int32",
"threats": "Collection(microsoft.graph.SecureScore.threat)",
"deprecated ": "Boolean",
"remediation": "String",
"remediationImpact ": "String",
"actionUrl": "String",
"controlStateUpdates": "Collection(microsoft.graph.SecureScore.controlStateUpdates)",
"tenantNotes": "String",
"upn": "String",
"comments": "String",
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securescorecontrolprofiles.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
