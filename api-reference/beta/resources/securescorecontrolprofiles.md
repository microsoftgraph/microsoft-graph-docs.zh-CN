---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f4bcee22036cf344fec83be8ec08bba602e08c3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087556"
---
# <a name="securescorecontrolprofile-resource-type"></a>secureScoreControlProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfile](securescorecontrolprofiles.md) 集合 |获取 secureScoreControlProfile 对象的集合。|


## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|   azureTenantId   |   字符串  |   租户 ID 的 GUID 字符串。  |
|   controlName |   字符串  |   控件的名称。 |
|   title   |   String  |   控件的标题。   |
| complianceInformation | [complianceInformation](complianceinformation.md) 集合 | 与安全得分控制相关联的合规性信息的集合 |
|   controlCategory |   字符串  |   控制操作类别 (帐户、数据、设备、应用程序、基础结构) 。  |
|   actionType  |   String  |   Control action type (Config、审阅和行为) 。 |
|   service |   String  |   拥有控件 (Exchange、Sharepoint、Azure AD) 的服务。 |
|   maxScore |  字符串  |   指定日期的当前获得的最大分数。   |
|   单层 |  字符串  |   控制层 (核心、纵深防御、高级 )     |
|   userImpact |    字符串  | 实施控制 (低、中、高) 的用户影响。    |
|   implementationCost |    字符串  |   Implemmentating 控件的资源成本 (low、适中、高) 。 |
|   排名 |  Int32   |   Microsoft 的控制堆栈排名。   |
|   病毒 |   String 集合   |   控制缓解 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗) 的威胁列表。 |
|   被 |    布尔 |   指示是否已对控件进行折旧的标志。   |
|   纠正 |   字符串  |   对控件将有助于修正的内容的说明。 |
|   remediationImpact | 字符串  |   对修正用户影响的说明。 |
|   actionUrl | 字符串  |   可将控件 actioned 到的位置的 URL。 |
|   controlStateUpdates | [secureScoreControlStateUpdate](securescorecontrolstateupdate.md) 集合 |    用于指示租户已将控件标记 (ignore、thirdParty、已评审)  (支持 [更新](../api/securescorecontrolprofiles-update.md)) 的标记。 |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
}-->

```json
{
  "title": "String",
  "azureTenantId": "String (identifier)",
  "maxScore": 1024.13,
  "actionType": "String",
  "service": "String",
  "tier": "String",
  "userImpact": "string",
  "implementationCost ": "String",
  "rank ": 100,
  "threats": ["string"],
  "deprecated ": false,
  "remediation": "String",
  "remediationImpact ": "String",
  "actionUrl": "String",
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}],
  "controlCategory": "string",
  "lastModifiedDateTime": "String (timestamp)"
}


```


<!--
{
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


