---
title: secureScoreControlProfile 资源类型
description: 表示租户每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可以显式拉取单个控件。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6c54901018dcb6eccf36be2f6f4b0fc1c7d9da8d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899832"
---
# <a name="securescorecontrolprofile-resource-type"></a>secureScoreControlProfile 资源类型

命名空间：microsoft.graph

表示租户每个控件数据的安全分数。 默认情况下，它将返回租户的所有控件，并可以显式拉取单个控件。


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) | [secureScoreControlProfile](securescorecontrolprofile.md) |读取 secureScoreControlProfiles 对象的属性和元数据。|
|[获取 secureScoreControlProfile](../api/securescorecontrolprofile-get.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |读取 secureScoreControlProfiles 对象的属性和元数据。|
|[更新 securescorecontrolprofile](../api/securescorecontrolprofile-update.md) | [securescorecontrolprofile](securescorecontrolprofile.md) |更新 securescorecontrolprofile 对象。 |


## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|id|String|提供程序生成的 GUID/唯一标识符。 只读。 必填。|
|azureTenantId|字符串|租户 ID 的 GUID 字符串。|
|actionType|String|控制操作类型 (配置、审阅、行为) 。|
|actionUrl|String|可在其中操作控件的 URL。 |
|controlCategory|String|控制操作类别 (标识、数据、设备、应用、基础结构) 。|
|title|String|控件的标题。|
|废弃|Boolean|指示控件是否已弃用的标志。|
|implementationCost|String|控制 (低、中、高) 的资源成本。|
|lastModifiedDateTime|DateTimeOffset|上次修改控件配置文件实体的时间。 时间戳类型表示日期和时间| 
|maxScore|双精度|控件的最大可实现分数。|
|排名|Int32|Microsoft 的堆栈控制排名。|
|修复|String|控件将帮助修正的说明。|
|remediationImpact|String|修正对用户的影响的说明。|
|service|String| (Exchange、Sharepoint、Azure AD) 拥有控件的服务。|
|威胁|字符串集合|控件缓解 (accountBreach、dataDeletion、dataExfiltration、dataSpillage 的威胁列表，
elevationOfPrivilege，maliciousInsider，passwordCracking，phishingOrWhaling，欺骗) 。|
|层|String|控制层 (核心、深度防御、高级)    |
|userImpact|String|实现控制 (低、中、高) 的用户影响。   |
|complianceInformation|[complianceInformation](complianceinformation.md) 集合|与安全分数控制关联的合规性信息的集合|
|controlStateUpdates|[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) 集合|标记，指示租户标记控件的位置 (忽略，thirdParty 已查看)  (支持 [更新](../api/securescorecontrolprofile-update.md)) 。|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|复杂类型，包含有关安全产品/服务供应商、提供程序和子保护程序 (的详细信息，例如，供应商=Microsoft;provider=SecureScore) 。 必填。|

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

