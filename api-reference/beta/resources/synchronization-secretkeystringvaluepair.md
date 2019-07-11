---
title: synchronizationSecretKeyStringValuePair 资源类型
description: '表示单个机密值。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d69b6b562ba4f42fd73f4f2fe51c2ad0ec0e4ce3
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620442"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="9d8a8-103">synchronizationSecretKeyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d8a8-103">synchronizationSecretKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d8a8-104">表示单个机密值。</span><span class="sxs-lookup"><span data-stu-id="9d8a8-104">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="9d8a8-105">属性</span><span class="sxs-lookup"><span data-stu-id="9d8a8-105">Properties</span></span>
| <span data-ttu-id="9d8a8-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d8a8-106">Property</span></span>     | <span data-ttu-id="9d8a8-107">类型</span><span class="sxs-lookup"><span data-stu-id="9d8a8-107">Type</span></span>   |<span data-ttu-id="9d8a8-108">说明</span><span class="sxs-lookup"><span data-stu-id="9d8a8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d8a8-109">Key</span><span class="sxs-lookup"><span data-stu-id="9d8a8-109">key</span></span>|<span data-ttu-id="9d8a8-110">String</span><span class="sxs-lookup"><span data-stu-id="9d8a8-110">String</span></span>| <span data-ttu-id="9d8a8-111">可能的值为`None`: `UserName`、 `Password`、 `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain` `ConsumerKey`、、、、、、、、、、、、、、、、 `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="9d8a8-111">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="9d8a8-112">value</span><span class="sxs-lookup"><span data-stu-id="9d8a8-112">value</span></span>|<span data-ttu-id="9d8a8-113">String</span><span class="sxs-lookup"><span data-stu-id="9d8a8-113">String</span></span>|<span data-ttu-id="9d8a8-114">密码的值。</span><span class="sxs-lookup"><span data-stu-id="9d8a8-114">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d8a8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d8a8-115">JSON representation</span></span>

<span data-ttu-id="9d8a8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d8a8-116">The following is a JSON representation of the resource.</span></span>

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
