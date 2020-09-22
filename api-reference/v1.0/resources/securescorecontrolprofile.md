---
title: secureScoreControlProfile 资源类型
description: 表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c7af5b2ab614dae57ef7c18aee80133cd7a2096a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984066"
---
# <a name="securescorecontrolprofile-resource-type"></a>secureScoreControlProfile 资源类型

命名空间：microsoft.graph

表示租户的每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可显式提取各个控件。


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) | [secureScoreControlProfile](securescorecontrolprofile.md) |读取 secureScoreControlProfiles 对象的属性和元数据。|
|[获取 secureScoreControlProfile](../api/securescorecontrolprofile-get.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |读取 secureScoreControlProfiles 对象的属性和元数据。|
|[更新 securescorecontrolprofile](../api/securescorecontrolprofile-update.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |更新 securescorecontrolprofile 对象。 |


## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|id|String|提供程序生成的 GUID/唯一标识符。 只读。 必需。|
|azureTenantId|字符串|租户 ID 的 GUID 字符串。|
|actionType|String|Control action type (Config、审阅和行为) 。|
|actionUrl|String|可将控件 actioned 到的位置的 URL。 |
|controlCategory|String|控制操作类别 (标识、数据、设备、应用程序、基础结构) 。|
|title|String|控件的标题。|
|被|Boolean|指示是否已对控件进行折旧的标志。|
|implementationCost|String|Implemmentating 控件的资源成本 (low、适中、高) 。|
|lastModifiedDateTime|DateTimeOffset|上次修改控件配置文件实体的时间。 时间戳类型表示日期和时间| 
|maxScore|双精度|控件的最大实现得分。|
|排名|Int32|Microsoft 的控制堆栈排名。|
|纠正|String|对控件将有助于修正的内容的说明。|
|remediationImpact|String|对修正用户影响的说明。|
|service|String|拥有控件 (Exchange、Sharepoint、Azure AD) 的服务。|
|病毒|String collection|控制缓解 (accountBreach、dataDeletion、dataExfiltration、dataSpillage 的威胁列表
elevationOfPrivilege、maliciousInsider、passwordCracking、phishingOrWhaling、欺骗) 。|
|单层|String|控制层 (核心、纵深防御、高级 )    |
|userImpact|String|实施控制 (低、中、高) 的用户影响。   |
|complianceInformation|[complianceInformation](complianceinformation.md) 集合|与安全得分控制相关联的合规性信息的集合|
|controlStateUpdates|[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) 集合|用于指示租户已将控件标记 (忽略、thirdParty、已评审)  (支持 [更新](../api/securescorecontrolprofile-update.md)) 的标记。|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|包含有关安全产品/服务供应商、提供商和 subprovider 的详细信息的复杂类型 (例如，供应商 = Microsoft;provider = SecureScore) 。 必需。|

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
  "id": "String (identifier)",
  "azureTenantId": "String",
  "actionType": "String",
  "actionUrl": "String",
  "controlCategory": "String",
  "title": "String", 
  "deprecated": "Boolean",
  "implementationCost": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "maxScore": "Double",
  "rank": "Int32",
  "remediation": "String",
  "remediationImpact": "String",
  "service": "String",
  "threats": ["String"],
  "tier": "String",
  "userImpact": "String",
  "complianceInformation": [{"@odata.type": "microsoft.graph.complianceInformation"}], 
  "controlStateUpdates": [{"@odata.type": "microsoft.graph.secureScoreControlStateUpdate"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlProfiles resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

