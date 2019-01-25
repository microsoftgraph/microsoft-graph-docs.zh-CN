---
title: 风险的资源类型
description: 汇聚风险级别、 风险状态和风险详细信息 risky 用户登录，或风险事件。
localization_priority: Normal
author: cloudhandler
ms.prod: security
ms.openlocfilehash: 48fda9624e45072240bc694b8b5e152fe3ef0764
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524819"
---
# <a name="risk-resource-type"></a><span data-ttu-id="70093-103">风险的资源类型</span><span class="sxs-lookup"><span data-stu-id="70093-103">risk resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70093-104">汇聚风险级别、 风险状态和风险详细信息 risky 用户登录，或风险事件。</span><span class="sxs-lookup"><span data-stu-id="70093-104">Aggregates the risk level, risk state and risk detail for the risky user, sign in, or risk event.</span></span>

## <a name="properties"></a><span data-ttu-id="70093-105">属性</span><span class="sxs-lookup"><span data-stu-id="70093-105">Properties</span></span>

| <span data-ttu-id="70093-106">属性</span><span class="sxs-lookup"><span data-stu-id="70093-106">Property</span></span>   | <span data-ttu-id="70093-107">类型</span><span class="sxs-lookup"><span data-stu-id="70093-107">Type</span></span>|<span data-ttu-id="70093-108">说明</span><span class="sxs-lookup"><span data-stu-id="70093-108">Description</span></span>|
|:---------------|:--------|:----------|
|`stateDetail`|<span data-ttu-id="70093-109">riskDetail</span><span class="sxs-lookup"><span data-stu-id="70093-109">riskDetail</span></span>|<span data-ttu-id="70093-110">提供原因后面的 risky 用户、 登录或风险事件特定状态。</span><span class="sxs-lookup"><span data-stu-id="70093-110">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="70093-111">可能的值为： `none`， `adminGeneratedTemporaryPassword`， `userPerformedSecuredPasswordChange`， `userPerformedSecuredPasswordReset`， `adminConfirmedSigninSafe`， `aiConfirmedSigninSafe`， `userPassedMFADrivenByRiskBasedPolicy`， `adminDismissedAllRiskForUser`， `adminConfirmedSigninCompromised`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="70093-111">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="70093-112">值`none`是指的任何操作已执行上的用户或登录到目前为止。</span><span class="sxs-lookup"><span data-stu-id="70093-112">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> |
|`riskLevelAggregated`|<span data-ttu-id="70093-113">riskLevel</span><span class="sxs-lookup"><span data-stu-id="70093-113">riskLevel</span></span>|<span data-ttu-id="70093-114">提供 risky 用户、 登录或风险事件的总体风险级别。</span><span class="sxs-lookup"><span data-stu-id="70093-114">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="70093-115">可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="70093-115">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="70093-116">值`hidden`是指为 Azure AD 身份保护未启用的用户或登录。</span><span class="sxs-lookup"><span data-stu-id="70093-116">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskLevelDuringSignIn`|<span data-ttu-id="70093-117">riskLeve</span><span class="sxs-lookup"><span data-stu-id="70093-117">riskLeve</span></span>|<span data-ttu-id="70093-118">登录过程中 （即基于实时风险事件） 提供登录的风险级别。</span><span class="sxs-lookup"><span data-stu-id="70093-118">Provides the risk level of a sign-in during the sign-in (i.e. based on the real-time risk events).</span></span> <span data-ttu-id="70093-119">可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="70093-119">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="70093-120">值`hidden`是指为 Azure AD 身份保护未启用登录。</span><span class="sxs-lookup"><span data-stu-id="70093-120">The value `hidden` means the sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`state`|<span data-ttu-id="70093-121">riskState</span><span class="sxs-lookup"><span data-stu-id="70093-121">riskState</span></span>|<span data-ttu-id="70093-122">提供 risky 用户、 登录或风险事件的风险状态。</span><span class="sxs-lookup"><span data-stu-id="70093-122">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="70093-123">可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="70093-123">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70093-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70093-124">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/risk.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
