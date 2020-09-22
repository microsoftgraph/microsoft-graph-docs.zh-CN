---
title: riskUserActivity 资源类型
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ecfe618a8db9f03bbf088ea053476fe6e51bcbf7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988938"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="c4479-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4479-103">riskUserActivity resource type</span></span>

<span data-ttu-id="c4479-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4479-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="c4479-105">属性</span><span class="sxs-lookup"><span data-stu-id="c4479-105">Properties</span></span>

| <span data-ttu-id="c4479-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4479-106">Property</span></span>       | <span data-ttu-id="c4479-107">类型</span><span class="sxs-lookup"><span data-stu-id="c4479-107">Type</span></span>    |<span data-ttu-id="c4479-108">说明</span><span class="sxs-lookup"><span data-stu-id="c4479-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c4479-109">eventTypes</span><span class="sxs-lookup"><span data-stu-id="c4479-109">eventTypes</span></span> | <span data-ttu-id="c4479-110">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="c4479-110">riskEventType collection</span></span> |<span data-ttu-id="c4479-111">风险事件类型的列表。</span><span class="sxs-lookup"><span data-stu-id="c4479-111">List of risk event types.</span></span> <span data-ttu-id="c4479-112">已弃用。</span><span class="sxs-lookup"><span data-stu-id="c4479-112">Deprecated.</span></span> <span data-ttu-id="c4479-113">请改用 **riskEventType** 。</span><span class="sxs-lookup"><span data-stu-id="c4479-113">Use **riskEventType** instead.</span></span> |
|<span data-ttu-id="c4479-114">riskEventType</span><span class="sxs-lookup"><span data-stu-id="c4479-114">riskEventType</span></span>|<span data-ttu-id="c4479-115">字符串</span><span class="sxs-lookup"><span data-stu-id="c4479-115">string</span></span>|<span data-ttu-id="c4479-116">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="c4479-116">The type of risk event detected.</span></span> <span data-ttu-id="c4479-117">可能的值为、、、、、、、、、、、、 `unlikelyTravel` `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `genericadminConfirmedUserCompromised` `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP` 和 `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="c4479-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="c4479-118">介绍</span><span class="sxs-lookup"><span data-stu-id="c4479-118">detail</span></span>     | <span data-ttu-id="c4479-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="c4479-119">riskDetail</span></span>  | <span data-ttu-id="c4479-120">可能的值为、、、、、、、、、、、 `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="c4479-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c4479-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4479-121">JSON representation</span></span>

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


