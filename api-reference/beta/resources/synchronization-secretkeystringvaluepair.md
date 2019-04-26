---
title: synchronizationSecretKeyStringValuePair 资源类型
description: '表示单个机密值。 '
localization_priority: Normal
ms.openlocfilehash: 36ec5ababb6c972bad336b3cfa8da4d34ba66c55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342879"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="f50c5-103">synchronizationSecretKeyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="f50c5-103">synchronizationSecretKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f50c5-104">表示单个机密值。</span><span class="sxs-lookup"><span data-stu-id="f50c5-104">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="f50c5-105">属性</span><span class="sxs-lookup"><span data-stu-id="f50c5-105">Properties</span></span>
| <span data-ttu-id="f50c5-106">属性</span><span class="sxs-lookup"><span data-stu-id="f50c5-106">Property</span></span>     | <span data-ttu-id="f50c5-107">类型</span><span class="sxs-lookup"><span data-stu-id="f50c5-107">Type</span></span>   |<span data-ttu-id="f50c5-108">说明</span><span class="sxs-lookup"><span data-stu-id="f50c5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f50c5-109">Key</span><span class="sxs-lookup"><span data-stu-id="f50c5-109">key</span></span>|<span data-ttu-id="f50c5-110">String</span><span class="sxs-lookup"><span data-stu-id="f50c5-110">String</span></span>| <span data-ttu-id="f50c5-111">可能的值为`None`: `UserName`、 `Password`、 `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain` `ConsumerKey`、、、、、、、、、、、、、、、、 `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="f50c5-111">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="f50c5-112">value</span><span class="sxs-lookup"><span data-stu-id="f50c5-112">value</span></span>|<span data-ttu-id="f50c5-113">String</span><span class="sxs-lookup"><span data-stu-id="f50c5-113">String</span></span>|<span data-ttu-id="f50c5-114">密码的值。</span><span class="sxs-lookup"><span data-stu-id="f50c5-114">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f50c5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f50c5-115">JSON representation</span></span>

<span data-ttu-id="f50c5-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f50c5-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
