---
title: riskUserActivity 资源类型
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ddf71668af9d66c1d3ea495a8438c444b9317a23
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2020
ms.locfileid: "43510992"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="602d2-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="602d2-103">riskUserActivity resource type</span></span>

<span data-ttu-id="602d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="602d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="602d2-105">属性</span><span class="sxs-lookup"><span data-stu-id="602d2-105">Properties</span></span>

| <span data-ttu-id="602d2-106">属性</span><span class="sxs-lookup"><span data-stu-id="602d2-106">Property</span></span>       | <span data-ttu-id="602d2-107">类型</span><span class="sxs-lookup"><span data-stu-id="602d2-107">Type</span></span>    |<span data-ttu-id="602d2-108">说明</span><span class="sxs-lookup"><span data-stu-id="602d2-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="602d2-109">eventTypes</span><span class="sxs-lookup"><span data-stu-id="602d2-109">eventTypes</span></span> | <span data-ttu-id="602d2-110">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="602d2-110">riskEventType collection</span></span> |<span data-ttu-id="602d2-111">风险事件类型的列表。</span><span class="sxs-lookup"><span data-stu-id="602d2-111">List of risk event types.</span></span> <span data-ttu-id="602d2-112">已弃用。</span><span class="sxs-lookup"><span data-stu-id="602d2-112">Deprecated.</span></span> <span data-ttu-id="602d2-113">请改用**riskEventTypes** 。</span><span class="sxs-lookup"><span data-stu-id="602d2-113">Use **riskEventTypes** instead.</span></span> |
|<span data-ttu-id="602d2-114">riskEventType</span><span class="sxs-lookup"><span data-stu-id="602d2-114">riskEventType</span></span>|<span data-ttu-id="602d2-115">string</span><span class="sxs-lookup"><span data-stu-id="602d2-115">string</span></span>|<span data-ttu-id="602d2-116">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="602d2-116">The type of risk event detected.</span></span> <span data-ttu-id="602d2-117">可能的值为`unlikelyTravel`、 `anonymizedIPAddress` `maliciousIPAddress` `unfamiliarFeatures` `malwareInfectedIPAddress` `suspiciousIPAddress` `leakedCredentials` `investigationsThreatIntelligence` `unknownFutureValue`、、 `genericadminConfirmedUserCompromised`、、、、、、、、、和。 `mcasImpossibleTravel` `mcasSuspiciousInboxManipulationRules` `investigationsThreatIntelligenceSigninLinked` `maliciousIPAddressValidCredentialsBlockedIP`</span><span class="sxs-lookup"><span data-stu-id="602d2-117">The possible values are `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `genericadminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, and `unknownFutureValue`.</span></span> |
| <span data-ttu-id="602d2-118">介绍</span><span class="sxs-lookup"><span data-stu-id="602d2-118">detail</span></span>     | <span data-ttu-id="602d2-119">riskDetail</span><span class="sxs-lookup"><span data-stu-id="602d2-119">riskDetail</span></span>  | <span data-ttu-id="602d2-120">可能的值为`none`、 `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` `unknownFutureValue`、、、、、、、、、、。 `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised`</span><span class="sxs-lookup"><span data-stu-id="602d2-120">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="602d2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="602d2-121">JSON representation</span></span>

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
