---
title: synchronizationSecretKeyStringValuePair 资源类型
description: '代表单个机密值。 '
localization_priority: Normal
ms.openlocfilehash: 55cbd6b19ddf6c6f622ad7daddea569558e31f0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818730"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="d4207-103">synchronizationSecretKeyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4207-103">synchronizationSecretKeyStringValuePair resource type</span></span>

> <span data-ttu-id="d4207-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4207-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4207-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4207-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4207-106">代表单个机密值。</span><span class="sxs-lookup"><span data-stu-id="d4207-106">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="d4207-107">属性</span><span class="sxs-lookup"><span data-stu-id="d4207-107">Properties</span></span>
| <span data-ttu-id="d4207-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4207-108">Property</span></span>     | <span data-ttu-id="d4207-109">类型</span><span class="sxs-lookup"><span data-stu-id="d4207-109">Type</span></span>   |<span data-ttu-id="d4207-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4207-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4207-111">Key</span><span class="sxs-lookup"><span data-stu-id="d4207-111">key</span></span>|<span data-ttu-id="d4207-112">字符串</span><span class="sxs-lookup"><span data-stu-id="d4207-112">String</span></span>| <span data-ttu-id="d4207-113">可能的值为： `None`， `UserName`， `Password`， `SecretToken`， `AppKey`， `BaseAddress`， `ClientIdentifier`， `ClientSecret`， `SingleSignOnType`， `Sandbox`， `Url`， `Domain`， `ConsumerKey`， `ConsumerSecret`， `TokenKey`， `TokenExpiration`， `Oauth2AccessToken`， `Oauth2AccessTokenCreationTime`， `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="d4207-113">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="d4207-114">值</span><span class="sxs-lookup"><span data-stu-id="d4207-114">value</span></span>|<span data-ttu-id="d4207-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d4207-115">String</span></span>|<span data-ttu-id="d4207-116">机密的值。</span><span class="sxs-lookup"><span data-stu-id="d4207-116">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4207-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4207-117">JSON representation</span></span>

<span data-ttu-id="d4207-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4207-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
