---
title: synchronizationSecretKeyStringValuePair 资源类型
description: '表示单个机密值。 '
localization_priority: Normal
ms.openlocfilehash: a937063ea04bd3726932e423a065026d51b05aa4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523227"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="9a99d-103">synchronizationSecretKeyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a99d-103">synchronizationSecretKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a99d-104">表示单个机密值。</span><span class="sxs-lookup"><span data-stu-id="9a99d-104">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="9a99d-105">属性</span><span class="sxs-lookup"><span data-stu-id="9a99d-105">Properties</span></span>
| <span data-ttu-id="9a99d-106">属性</span><span class="sxs-lookup"><span data-stu-id="9a99d-106">Property</span></span>     | <span data-ttu-id="9a99d-107">类型</span><span class="sxs-lookup"><span data-stu-id="9a99d-107">Type</span></span>   |<span data-ttu-id="9a99d-108">说明</span><span class="sxs-lookup"><span data-stu-id="9a99d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a99d-109">Key</span><span class="sxs-lookup"><span data-stu-id="9a99d-109">key</span></span>|<span data-ttu-id="9a99d-110">String</span><span class="sxs-lookup"><span data-stu-id="9a99d-110">String</span></span>| <span data-ttu-id="9a99d-111">可能的值为`None`: `UserName`、 `Password`、 `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain` `ConsumerKey`、、、、、、、、、、、、、、、、 `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="9a99d-111">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="9a99d-112">value</span><span class="sxs-lookup"><span data-stu-id="9a99d-112">value</span></span>|<span data-ttu-id="9a99d-113">String</span><span class="sxs-lookup"><span data-stu-id="9a99d-113">String</span></span>|<span data-ttu-id="9a99d-114">密码的值。</span><span class="sxs-lookup"><span data-stu-id="9a99d-114">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a99d-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a99d-115">JSON representation</span></span>

<span data-ttu-id="9a99d-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a99d-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-secretkeystringvaluepair.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
