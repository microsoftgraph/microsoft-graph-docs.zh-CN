---
title: riskUserActivity 资源类型
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7772bde328004ffd26133421cc97a9f296ae9370
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442871"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="fd038-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd038-103">riskUserActivity resource type</span></span>

<span data-ttu-id="fd038-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd038-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="fd038-105">属性</span><span class="sxs-lookup"><span data-stu-id="fd038-105">Properties</span></span>

| <span data-ttu-id="fd038-106">属性</span><span class="sxs-lookup"><span data-stu-id="fd038-106">Property</span></span>       | <span data-ttu-id="fd038-107">类型</span><span class="sxs-lookup"><span data-stu-id="fd038-107">Type</span></span>    |<span data-ttu-id="fd038-108">说明</span><span class="sxs-lookup"><span data-stu-id="fd038-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fd038-109">eventTypes</span><span class="sxs-lookup"><span data-stu-id="fd038-109">eventTypes</span></span> | <span data-ttu-id="fd038-110">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="fd038-110">riskEventType collection</span></span> |<span data-ttu-id="fd038-111">风险事件类型列表。</span><span class="sxs-lookup"><span data-stu-id="fd038-111">List of risk event types.</span></span> <span data-ttu-id="fd038-112">已弃用。</span><span class="sxs-lookup"><span data-stu-id="fd038-112">Deprecated.</span></span> <span data-ttu-id="fd038-113">请 **改为使用 riskEventType。**</span><span class="sxs-lookup"><span data-stu-id="fd038-113">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="fd038-114">riskEventType</span><span class="sxs-lookup"><span data-stu-id="fd038-114">riskEventType</span></span>|<span data-ttu-id="fd038-115">string</span><span class="sxs-lookup"><span data-stu-id="fd038-115">string</span></span>|<span data-ttu-id="fd038-116">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="fd038-116">The type of risk event detected.</span></span> <span data-ttu-id="fd038-117">可能的值是 `unlikelyTravel` ， `anonymizedIPAddress` ， ， ， ， ， ， `maliciousIPAddress` ， `unfamiliarFeatures` `malwareInfectedIPAddress` 和 `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="fd038-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="fd038-118">detail</span><span class="sxs-lookup"><span data-stu-id="fd038-118">detail</span></span>     | <span data-ttu-id="fd038-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="fd038-119">riskDetail</span></span>  | <span data-ttu-id="fd038-120">可能的值是 `none` ， `adminGeneratedTemporaryPassword` ， ， ， ， ， `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="fd038-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="fd038-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd038-121">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskUserActivity"
}-->
```json
{
    "eventTypes": ["String"],
    "detail": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "",
  "tocPath": "",
  "suppressions": []
}
-->


