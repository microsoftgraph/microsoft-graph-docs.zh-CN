---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7dfca5eedebe7f2fe524c79cee52e5855af7f291
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520862"
---
# <a name="securescorecontrolprofile-resource-type"></a>secureScoreControlProfile 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfile](securescorecontrolprofiles.md)集合 |获取 secureScoreControlProfile 对象的集合。|


## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|   azureTenantId   |   字符串  |   租户 ID 的 GUID 字符串。  |
|   controlName |   String  |   控件的名称。 |
|   title   |   String  |   控件的标题。   |
| complianceInformation | [complianceInformation](complianceinformation.md)集合 | 与安全得分控制相关联的合规性信息的集合 |
|   controlCategory |   String  |   控制措施类别（帐户、数据、设备、应用程序、基础结构）。  |
|   actionType  |   String  |   控制操作类型（Config、审阅、行为）。 |
|   service |   String  |   拥有控件的服务（Exchange、Sharepoint、Azure AD）。 |
|   maxScore |  String  |   指定日期的当前获得的最大分数。   |
|   单层 |  String  |   控制层（Core，纵深防御，高级。）    |
|   userImpact |    String  | 实施控制的用户影响（低、中等、高）。    |
|   implementationCost |    String  |   Implemmentating 控件的资源成本（low、适中、high）。 |
|   排名 |  Int32   |   Microsoft 的控制堆栈排名。   |
|   病毒 |   String 集合   |   控制缓解的威胁列表（accountBreach、dataDeletion、dataExfiltration、dataSpillage、elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗）。 |
|   被 |    布尔 |   指示是否已对控件进行折旧的标志。   |
|   纠正 |   String  |   对控件将有助于修正的内容的说明。 |
|   remediationImpact | String  |   对修正用户影响的说明。 |
|   actionUrl | String  |   可将控件 actioned 到的位置的 URL。 |
|   controlStateUpdates | [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合 |    用于指示租户已标记控件的位置的标志（忽略、thirdParty、已审阅）（支持[更新](../api/securescorecontrolprofiles-update.md)）。 |
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
