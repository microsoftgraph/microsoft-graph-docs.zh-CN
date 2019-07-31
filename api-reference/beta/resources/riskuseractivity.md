---
title: riskUserActivity 资源类型
description: author
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b4b33d4f9344f8031076f00b1b442b882fffe6d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965353"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="0fa1f-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fa1f-103">riskUserActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="0fa1f-104">属性</span><span class="sxs-lookup"><span data-stu-id="0fa1f-104">Properties</span></span>

| <span data-ttu-id="0fa1f-105">属性</span><span class="sxs-lookup"><span data-stu-id="0fa1f-105">Property</span></span>       | <span data-ttu-id="0fa1f-106">类型</span><span class="sxs-lookup"><span data-stu-id="0fa1f-106">Type</span></span>    |<span data-ttu-id="0fa1f-107">说明</span><span class="sxs-lookup"><span data-stu-id="0fa1f-107">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0fa1f-108">eventTypes</span><span class="sxs-lookup"><span data-stu-id="0fa1f-108">eventTypes</span></span> | <span data-ttu-id="0fa1f-109">riskEventType 集合</span><span class="sxs-lookup"><span data-stu-id="0fa1f-109">riskEventType collection</span></span> |<span data-ttu-id="0fa1f-110">可能的值是 unlikelyTravel、anonymizedIPAddress、maliciousIPAddress、unfamiliarFeatures、malwareInfectedIPAddress、suspiciousIPAddress、leakedCredentials、investigationsThreatIntelligence、genericadminConfirmedUserCompromised、mcasImpossibleTravel、mcasSuspiciousInboxManipulationRules、investigationsThreatIntelligenceSigninLinked、maliciousIPAddressValidCredentialsBlockedIP、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="0fa1f-110">The possible values are unlikelyTravel, anonymizedIPAddress, maliciousIPAddress, unfamiliarFeatures, malwareInfectedIPAddress, suspiciousIPAddress, leakedCredentials, investigationsThreatIntelligence, generic, adminConfirmedUserCompromised, mcasImpossibleTravel, mcasSuspiciousInboxManipulationRules, investigationsThreatIntelligenceSigninLinked, maliciousIPAddressValidCredentialsBlockedIP, unknownFutureValue.</span></span>  |
| <span data-ttu-id="0fa1f-111">介绍</span><span class="sxs-lookup"><span data-stu-id="0fa1f-111">detail</span></span>     | <span data-ttu-id="0fa1f-112">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0fa1f-112">riskDetail</span></span>  | <span data-ttu-id="0fa1f-113">可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="0fa1f-113">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0fa1f-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fa1f-114">JSON representation</span></span>

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
