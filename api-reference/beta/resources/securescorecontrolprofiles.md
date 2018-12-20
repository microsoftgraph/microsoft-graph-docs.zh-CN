---
title: secureScoreControlProfiles 资源类型
description: 表示每个控件数据的租户的安全分数。 默认情况下，它返回租户的所有控件并且可以显式拉单个控件。
ms.openlocfilehash: 3e7dc463d7521e1980b41034ae4121ab610dd8f5
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380581"
---
# <a name="securescorecontrolprofiles-resource-type"></a>secureScoreControlProfiles 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示每个控件数据的租户的安全分数。 默认情况下，它返回租户的所有控件并且可以显式拉单个控件。


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfiles](securescorecontrolprofiles.md) |读取属性和 secureScoreControlProfiles 对象的元数据。|


## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|   azureTenantId   |   字符串  |   GUID string 租户 id。  |
|   控件名称 |   字符串  |   控件的名称。 |
|   title   |   字符串  |   控件的标题。   |
| complianceInformation | [complianceInformation](complianceinformation.md)集合 | 与关联的合规性信息的集合安全分数控件 |
|   controlCategory |   字符串  |   控制操作类别 （帐户、 数据、 设备、 应用程序、 基础结构）。  |
|   actionType  |   String  |   控制操作类型 （Config、 审阅、 行为）。 |
|   service |   String  |   拥有控件 （Exchange、 Sharepoint、 Azure AD） 的服务。 |
|   maxScore |  字符串  |   当前在指定日期上获得最大分数。   |
|   层 |  字符串  |   控件层 (核心、 防护深入，高级。)    |
|   userImpact |    字符串  | 用户影响实现控件 （低、 中等，高）。    |
|   implementationCost |    字符串  |   资源成本 implemmentating 控件 （低、 中等，高）。 |
|   排名 |  Int32   |   Microsoft 的堆栈控件的排名。   |
|   威胁 |   字符串集合   |   控制可以缓解的威胁的列表 (accountBreach，dataDeletion，dataExfiltration，dataSpillage，elevationOfPrivilege，maliciousInsider，passwordCracking，phishingOrWhaling，欺骗)。 |
|   弃用 |    Boolean |   用于指示控件进行折旧计算的标志。   |
|   修正 |   字符串  |   内容控件的说明将帮助纠正。 |
|   remediationImpact | 字符串  |   对用户的修正影响的说明。 |
|   actionUrl | 字符串  |   该控件可进行的 URL。 |
|   controlStateUpdates |   [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合 |    标志指示其中租户具有标记控件 （忽略，第三方，审阅） （支持[更新](../api/securescorecontrolprofiles-update.md)）。 |

## <a name="relationships"></a>Relationships

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


<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
