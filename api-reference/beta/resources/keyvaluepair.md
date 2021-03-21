---
title: keyValuePair 资源类型
description: 操作参数的键值对。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 8897ea3d3788ce3fa846d845cb0854101b0b2ce7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960423"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="bfa42-103">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfa42-103">keyValuePair resource type</span></span>

<span data-ttu-id="bfa42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfa42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfa42-105">操作参数的键值对。</span><span class="sxs-lookup"><span data-stu-id="bfa42-105">Key value pair for action parameters.</span></span>

## <a name="properties"></a><span data-ttu-id="bfa42-106">属性</span><span class="sxs-lookup"><span data-stu-id="bfa42-106">Properties</span></span>

| <span data-ttu-id="bfa42-107">属性</span><span class="sxs-lookup"><span data-stu-id="bfa42-107">Property</span></span>     | <span data-ttu-id="bfa42-108">类型</span><span class="sxs-lookup"><span data-stu-id="bfa42-108">Type</span></span>        | <span data-ttu-id="bfa42-109">说明</span><span class="sxs-lookup"><span data-stu-id="bfa42-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bfa42-110">name</span><span class="sxs-lookup"><span data-stu-id="bfa42-110">name</span></span>|<span data-ttu-id="bfa42-111">String</span><span class="sxs-lookup"><span data-stu-id="bfa42-111">String</span></span>|<span data-ttu-id="bfa42-112">此键值对的名称。</span><span class="sxs-lookup"><span data-stu-id="bfa42-112">Name for this key-value pair.</span></span> <span data-ttu-id="bfa42-113">可能的名称包括 `AdditionalWSFedEndpointCheckResult` `AllowedAuthenticationClassReferencesCheckResult` `AlwaysRequireAuthenticationCheckResult` ：、、、、、、、、、、。 `AutoUpdateEnabledCheckResult` `ClaimsProviderNameCheckResult` `EncryptClaimsCheckResult` `EncryptedNameIdRequiredCheckResult` `MonitoringEnabledCheckResult` `NotBeforeSkewCheckResult` `RequestMFAFromClaimsProvidersCheckResult` `SignedSamlRequestsRequiredCheckResult` `AdditionalAuthenticationRulesCheckResult` `TokenLifetimeCheckResult` `DelegationAuthorizationRulesCheckResult` `IssuanceAuthorizationRulesCheckResult` `IssuanceTransformRulesCheckResult`</span><span class="sxs-lookup"><span data-stu-id="bfa42-113">Possible names are: `AdditionalWSFedEndpointCheckResult`,  `AllowedAuthenticationClassReferencesCheckResult`, `AlwaysRequireAuthenticationCheckResult`,   `AutoUpdateEnabledCheckResult`, `ClaimsProviderNameCheckResult`, `EncryptClaimsCheckResult`,  `EncryptedNameIdRequiredCheckResult`, `MonitoringEnabledCheckResult`,`NotBeforeSkewCheckResult`,  `RequestMFAFromClaimsProvidersCheckResult`, `SignedSamlRequestsRequiredCheckResult`, `AdditionalAuthenticationRulesCheckResult`, `TokenLifetimeCheckResult`,  `DelegationAuthorizationRulesCheckResult`, `IssuanceAuthorizationRulesCheckResult`, `IssuanceTransformRulesCheckResult`.</span></span>|
|<span data-ttu-id="bfa42-114">value</span><span class="sxs-lookup"><span data-stu-id="bfa42-114">value</span></span>|<span data-ttu-id="bfa42-115">String</span><span class="sxs-lookup"><span data-stu-id="bfa42-115">String</span></span>|<span data-ttu-id="bfa42-116">此键值对的值。</span><span class="sxs-lookup"><span data-stu-id="bfa42-116">Value for this key-value pair.</span></span> <span data-ttu-id="bfa42-117">如果验证检查通过 () ， (验证检查失败) ， (验证检查为警告) ，则可能会返回结果 `0` `1` `2` 值。</span><span class="sxs-lookup"><span data-stu-id="bfa42-117">Possible result values are `0` (when the validation check passed), `1` (when the validation check failed), or `2` (when the validation check is a warning).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfa42-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfa42-118">JSON representation</span></span>

<span data-ttu-id="bfa42-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfa42-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

