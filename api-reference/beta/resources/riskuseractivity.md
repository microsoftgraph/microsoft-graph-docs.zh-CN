---
title: riskUserActivity 资源类型
description: author
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 26dc0cf4d8309e2cc116b4b4265a3d592d316a56
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43178898"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="826f9-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="826f9-103">riskUserActivity resource type</span></span>

<span data-ttu-id="826f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="826f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="826f9-105">属性</span><span class="sxs-lookup"><span data-stu-id="826f9-105">Properties</span></span>

| <span data-ttu-id="826f9-106">属性</span><span class="sxs-lookup"><span data-stu-id="826f9-106">Property</span></span>       | <span data-ttu-id="826f9-107">类型</span><span class="sxs-lookup"><span data-stu-id="826f9-107">Type</span></span>    |<span data-ttu-id="826f9-108">说明</span><span class="sxs-lookup"><span data-stu-id="826f9-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="826f9-109">eventTypes</span><span class="sxs-lookup"><span data-stu-id="826f9-109">eventTypes</span></span> | <span data-ttu-id="826f9-110">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="826f9-110">riskEventType collection</span></span> |<span data-ttu-id="826f9-111">可能的值包括 unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、leakedCredentials、investigationsThreatIntelligence、generic、adminConfirmedUserCompromised、mcasImpossibleTravel、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="826f9-111">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="826f9-112">介绍</span><span class="sxs-lookup"><span data-stu-id="826f9-112">detail</span></span>     | <span data-ttu-id="826f9-113">riskDetail</span><span class="sxs-lookup"><span data-stu-id="826f9-113">riskDetail</span></span>  | <span data-ttu-id="826f9-114">可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="826f9-114">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="826f9-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="826f9-115">JSON representation</span></span>

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
