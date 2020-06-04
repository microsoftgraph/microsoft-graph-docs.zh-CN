---
title: riskUserActivity 资源类型
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8032a721a8f8a94d7cd1481edf58ee785092bcfd
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556315"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="e0ffd-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0ffd-103">riskUserActivity resource type</span></span>

<span data-ttu-id="e0ffd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0ffd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="e0ffd-105">属性</span><span class="sxs-lookup"><span data-stu-id="e0ffd-105">Properties</span></span>

| <span data-ttu-id="e0ffd-106">属性</span><span class="sxs-lookup"><span data-stu-id="e0ffd-106">Property</span></span>       | <span data-ttu-id="e0ffd-107">类型</span><span class="sxs-lookup"><span data-stu-id="e0ffd-107">Type</span></span>    |<span data-ttu-id="e0ffd-108">说明</span><span class="sxs-lookup"><span data-stu-id="e0ffd-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e0ffd-109">eventTypes</span><span class="sxs-lookup"><span data-stu-id="e0ffd-109">eventTypes</span></span> | <span data-ttu-id="e0ffd-110">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="e0ffd-110">riskEventType collection</span></span> |<span data-ttu-id="e0ffd-111">风险事件类型的列表。</span><span class="sxs-lookup"><span data-stu-id="e0ffd-111">List of risk event types.</span></span> <span data-ttu-id="e0ffd-112">已弃用。</span><span class="sxs-lookup"><span data-stu-id="e0ffd-112">Deprecated.</span></span> <span data-ttu-id="e0ffd-113">请改用**riskEventType** 。</span><span class="sxs-lookup"><span data-stu-id="e0ffd-113">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="e0ffd-114">riskEventType</span><span class="sxs-lookup"><span data-stu-id="e0ffd-114">riskEventType</span></span>|<span data-ttu-id="e0ffd-115">string</span><span class="sxs-lookup"><span data-stu-id="e0ffd-115">string</span></span>|<span data-ttu-id="e0ffd-116">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="e0ffd-116">The type of risk event detected.</span></span> <span data-ttu-id="e0ffd-117">可能的值为、、、、、、、、、、、、 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` 和 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="e0ffd-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="e0ffd-118">介绍</span><span class="sxs-lookup"><span data-stu-id="e0ffd-118">detail</span></span>     | <span data-ttu-id="e0ffd-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="e0ffd-119">riskDetail</span></span>  | <span data-ttu-id="e0ffd-120">可能的值为、、、、、、、、、、、 `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="e0ffd-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e0ffd-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0ffd-121">JSON representation</span></span>

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
