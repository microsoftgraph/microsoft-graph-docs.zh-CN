---
title: secureScoreControlProfile 资源类型
description: 表示租户每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可以显式拉取单个控件。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 4d401b4003ef8ce0a4384daf16a03ce9d2851694
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735948"
---
# <a name="securescorecontrolprofile-resource-type"></a>secureScoreControlProfile 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可以显式拉取单个控件。


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
| complianceInformation | [complianceInformation](complianceinformation.md) 集合 | 与安全分数控制关联的合规性信息的集合 |
|   controlCategory |   字符串  |   控制操作类别 (帐户、数据、设备、应用、基础结构) 。  |
|   actionType  |   String  |   控制操作类型 (配置、审阅、行为) 。 |
|   service |   String  |    (Exchange、Sharepoint、Azure AD) 拥有控件的服务。 |
|   maxScore |  字符串  |   当前在指定日期获得的最大分数。   |
|   层 |  String  |   控制层 (核心、深度防御、高级)     |
|   userImpact |    字符串  | 实现控制 (低、中、高) 的用户影响。    |
|   implementationCost |    字符串  |   控制 (低、中、高) 的资源成本。 |
|   排名 |  Int32   |   Microsoft 的堆栈控制排名。   |
|   威胁 |   String 集合   |   控件缓解 (accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗) 的威胁列表。 |
|   废弃 |    布尔值 |   指示控件是否已弃用的标志。   |
|   修复 |   String  |   控件将帮助修正的说明。 |
|   remediationImpact | 字符串  |   修正对用户的影响的说明。 |
|   actionUrl | String  |   可在其中操作控件的 URL。 |
|   controlStateUpdates | [secureScoreControlStateUpdate](securescorecontrolstateupdate.md) 集合 |    标记，指示租户标记控件的位置 (忽略，thirdParty 已查看)  (支持 [更新](../api/securescorecontrolprofiles-update.md)) 。 |
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


