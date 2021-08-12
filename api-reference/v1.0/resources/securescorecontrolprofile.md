---
title: secureScoreControlProfile 资源类型
description: 表示每个控件数据的租户安全分数。 默认情况下，它返回租户的所有控件，并可以显式拉取单个控件。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cfb05d70e098a1483827783d2e3e3755f3b9393c619133ea8a547b8d39bfe988
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54184485"
---
# <a name="securescorecontrolprofile-resource-type"></a>secureScoreControlProfile 资源类型

命名空间：microsoft.graph

表示每个控件数据的租户安全分数。 默认情况下，它返回租户的所有控件，并可以显式拉取单个控件。


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
|actionType|String|控件操作类型 (配置、审阅、行为) 。|
|actionUrl|String|控件可操作位置的 URL。 |
|controlCategory|String|控制操作类别 (标识、数据、设备、应用、基础结构) 。|
|title|String|控件的标题。|
|已弃用|Boolean|用于指示控件是否被弃用的标志。|
|implementationCost|String|利用低、中等、高 (控制的资源) 。|
|lastModifiedDateTime|DateTimeOffset|上次修改控件配置文件实体的时间。 时间戳类型表示日期和时间| 
|maxScore|双精度|控件的最大可获取分数。|
|排名|Int32|Microsoft 的控件堆栈排名。|
|remediation|String|该控件将帮助修正哪些内容的说明。|
|remediationImpact|String|对修正用户的影响的说明。|
|service|String|拥有 Azure AD (Exchange、Sharepoint、Azure AD) 。|
|威胁|String collection|控制的威胁列表可缓解 (帐户Breach，dataDeletion，dataExfiltration，dataSpillage，
elevationOfPrivilege，maliciousInsider，passwordCracking，phishingOrLing，spoofing) 。|
|tier|String|控制层 (核心、深度防御、高级)    |
|userImpact|String|对低、中等、高 (控件的用户) 。   |
|complianceInformation|[complianceInformation](complianceinformation.md) 集合|与安全分数控制关联的合规性信息的集合|
|controlStateUpdates|[secureScoreControlStateUpdate](securescorecontrolstateupdate.md) 集合|指示租户在何处标记控件的标志 (，第三部分，查看)  ([更新) 。](../api/securescorecontrolprofile-update.md)|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|复杂类型，包含有关安全产品/服务供应商、提供程序和子 (的详细信息，例如，vendor=Microsoft;provider=SecureScore) 。 必填。|

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

