---
title: 风险的资源类型
description: 汇聚风险级别、 风险状态和风险详细信息 risky 用户登录，或风险事件。
ms.openlocfilehash: bc8ea5c30f78560ae8750e7750596f282feb4825
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044080"
---
# <a name="risk-resource-type"></a><span data-ttu-id="f9690-103">风险的资源类型</span><span class="sxs-lookup"><span data-stu-id="f9690-103">risk resource type</span></span>

> <span data-ttu-id="f9690-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f9690-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9690-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f9690-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9690-106">汇聚风险级别、 风险状态和风险详细信息 risky 用户登录，或风险事件。</span><span class="sxs-lookup"><span data-stu-id="f9690-106">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="f9690-107">属性</span><span class="sxs-lookup"><span data-stu-id="f9690-107">Properties</span></span>

| <span data-ttu-id="f9690-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9690-108">Property</span></span>   | <span data-ttu-id="f9690-109">类型</span><span class="sxs-lookup"><span data-stu-id="f9690-109">Type</span></span>|<span data-ttu-id="f9690-110">说明</span><span class="sxs-lookup"><span data-stu-id="f9690-110">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="f9690-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="f9690-111">riskDetail</span></span>|<span data-ttu-id="f9690-112">提供原因后面的 risky 用户、 登录或风险事件特定状态。</span><span class="sxs-lookup"><span data-stu-id="f9690-112">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="f9690-113">可能的值为： `none`， `adminGeneratedTemporaryPassword`， `userPerformedSecuredPasswordChange`， `userPerformedSecuredPasswordReset`， `adminConfirmedSigninSafe`， `aiConfirmedSigninSafe`， `userPassedMFADrivenByRiskBasedPolicy`， `adminDismissedAllRiskForUser`， `adminConfirmedSigninCompromised`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="f9690-113">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="f9690-114">值`none`是指的任何操作已执行上的用户或登录到目前为止。</span><span class="sxs-lookup"><span data-stu-id="f9690-114">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="f9690-115">riskLevel</span><span class="sxs-lookup"><span data-stu-id="f9690-115">riskLevel</span></span>|<span data-ttu-id="f9690-116">提供 risky 用户、 登录或风险事件的总体风险级别。</span><span class="sxs-lookup"><span data-stu-id="f9690-116">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="f9690-117">可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="f9690-117">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="f9690-118">值`hidden`是指为 Azure AD 身份保护未启用的用户或登录。</span><span class="sxs-lookup"><span data-stu-id="f9690-118">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="f9690-119">riskLeve</span><span class="sxs-lookup"><span data-stu-id="f9690-119">riskLeve</span></span>|<span data-ttu-id="f9690-120">登录过程中 （即基于实时风险事件） 提供登录的风险级别。</span><span class="sxs-lookup"><span data-stu-id="f9690-120">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="f9690-121">可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="f9690-121">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="f9690-122">值`hidden`是指为 Azure AD 身份保护未启用登录。</span><span class="sxs-lookup"><span data-stu-id="f9690-122">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="f9690-123">riskState</span><span class="sxs-lookup"><span data-stu-id="f9690-123">riskState</span></span>|<span data-ttu-id="f9690-124">提供 risky 用户、 登录或风险事件的风险状态。</span><span class="sxs-lookup"><span data-stu-id="f9690-124">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="f9690-125">可能的值为： `none`， `confirmedSafe`， `remediated`， `dismissed`， `atRisk`， `confirmedCompromised`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="f9690-125">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f9690-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9690-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
    "stateDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
    "riskLevelAggregated":  {"@odata.type": "microsoft.graph.riskLevel"},
    "riskLevelDuringSignIn":  {"@odata.type": "microsoft.graph.riskLevel"},
    "state":  {"@odata.type": "microsoft.graph.riskState"}
  }
  ```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
