---
title: secureScoreControlProfiles 资源类型
description: 表示每个控件数据的租户的安全分数。 默认情况下，它返回租户的所有控件并且可以显式拉单个控件。
localization_priority: Normal
ms.openlocfilehash: 4e599bbffd291de51ba478f8661999d01c8c8998
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576057"
---
# <a name="securescorecontrolprofiles-resource-type"></a>secureScoreControlProfiles 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示每个控件数据的租户的安全分数。 默认情况下，它返回租户的所有控件并且可以显式拉单个控件。


## <a name="methods"></a>方法

| 方法   | 返回类型|说明|
|:---------------|:--------|:----------|
|[列出 secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) | [secureScoreControlProfile](securescorecontrolprofiles.md) |读取属性和 secureScoreControlProfiles 对象的元数据。|


## <a name="properties"></a>属性

|名称 |类型 |说明 |
|:--|:--|:--|
|   azureTenantId   |   String  |   GUID string 租户 id。  |
|   控件名称 |   String  |   控件的名称。 |
|   title   |   String  |   控件的标题。   |
|   controlCategory |   String  |   控制操作类别 （帐户、 数据、 设备、 应用程序、 基础结构）。  |
|   actionType  |   String  |   控制操作类型 （Config、 审阅、 行为）。 |
|   service |   String  |   拥有控件 （Exchange、 Sharepoint、 Azure AD） 的服务。 |
|   maxScore |  双精度  |   当前在指定日期上获得最大分数。   |
|   层 |  String  |   控件层 (核心、 防护深入，高级。)    |
|   userImpact |    String  | 用户影响实现控件 （低、 中等，高）。    |
|   implementationCost |    String  |   资源成本 implemmentating 控件 （低、 中等，高）。 |
|   排名 |  Int32   |   Microsoft 的堆栈控件的排名。   |
|   威胁 |   String 集合   |   控制可以缓解的威胁的列表 (accountBreach，dataDeletion，dataExfiltration，dataSpillage，elevationOfPrivilege，maliciousInsider，passwordCracking，phishingOrWhaling，欺骗)。 |
|   弃用 |    布尔值 |   用于指示控件进行折旧计算的标志。   |
|   修正 |   String  |   内容控件的说明将帮助纠正。 |
|   remediationImpact | String  |   对用户的修正影响的说明。 |
|   actionUrl | String  |   该控件可进行的 URL。 |
|   lastModifiedDateTime |  字符串 （方法） |   上次修改日期 |
|   controlStateUpdates |   [secureScoreControlStateUpdate](securescorecontrolstateupdate.md)集合 |  标志指示其中租户具有标记控件 （忽略，第三方，审阅） （支持[更新](../api/securescorecontrolprofiles-update.md)）。 |
|   vendorInformation | [securityVendorInformation](securityvendorinformation.md) | 包含有关安全产品/服务供应商、 提供商和 subprovider 详细信息 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。|

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
    "referenceId": "String", 
    "controlName": "String", 
    "maxScore": "Double",
    "controlCategory": "string",
    "actionType": "string",
    "service": "String",
    "tier": "string",
    "userImpact": "string",
    "implementationCost ": "string",
    "rank ": "Int32",
    "deprecated ": "Boolean",
    "remediation": "String",
    "remediationImpact ": "String",
    "actionUrl": "String",
    "lastModifiedDateTime": "   String (DateTimeOffset)",
    "controlStateUpdates": [{"odata.type":"microsoft.graph.secureScorecontrolStateUpdates"}],
    "tenantNotes": "String",
    "upn": "String",    
    "vendorInformation" : "microsoft.graph.securityVendorInformation"
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
