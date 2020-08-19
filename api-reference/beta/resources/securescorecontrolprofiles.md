---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 3eeb7b0bd1575a336cdeb9ff73e808a057f61743
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807479"
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
|   controlName |   String  |   控件的名称。 |
|   title   |   String  |   控件的标题。   |
| complianceInformation | [complianceInformation](complianceinformation.md) 集合 | 与安全得分控制相关联的合规性信息的集合 |
|   controlCategory |   String  |   控制操作类别 (帐户、数据、设备、应用程序、基础结构) 。  |
|   actionType  |   String  |   Control action type (Config、审阅和行为) 。 |
|   service |   String  |   拥有控件 (Exchange、Sharepoint、Azure AD) 的服务。 |
|   maxScore |  String  |   指定日期的当前获得的最大分数。   |
|   单层 |  String  |   控制层 (核心、纵深防御、高级 )     |
|   userImpact |    String  | 实施控制 (低、中、高) 的用户影响。    |
|   implementationCost |    String  |   Implemmentating 控件的资源成本 (low、适中、高) 。 |
|   排名 |  Int32   |   Microsoft 的控制堆栈排名。   |
|   病毒 |   String 集合   |   控制缓解 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗) 的威胁列表。 |
|   被 |    布尔值 |   指示是否已对控件进行折旧的标志。   |
|   纠正 |   String  |   对控件将有助于修正的内容的说明。 |
|   remediationImpact | String  |   对修正用户影响的说明。 |
|   actionUrl | String  |   可将控件 actioned 到的位置的 URL。 |
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
