---
title: riskyUser 资源类型
description: 表示处于风险中的 Azure AD 用户。 Azure AD 根据各种信号和机器学习持续评估用户风险。 此 API 为 Azure AD 中所有处于风险中的用户提供编程访问。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: 9a234bc4c84ed6acc569f98c8c9b5d475a5b56be
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442852"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="0400b-105">riskyUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="0400b-105">riskyUser resource type</span></span>

<span data-ttu-id="0400b-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0400b-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0400b-107">表示处于风险中的 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="0400b-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="0400b-108">Azure AD 根据各种信号和机器学习持续评估用户风险。</span><span class="sxs-lookup"><span data-stu-id="0400b-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="0400b-109">此 API 为 Azure AD 中所有处于风险中的用户提供编程访问。</span><span class="sxs-lookup"><span data-stu-id="0400b-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="0400b-110">有关风险事件详细信息，请参阅 Azure [Active Directory Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="0400b-110">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="0400b-111">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="0400b-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="0400b-112">Methods</span><span class="sxs-lookup"><span data-stu-id="0400b-112">Methods</span></span>

| <span data-ttu-id="0400b-113">方法</span><span class="sxs-lookup"><span data-stu-id="0400b-113">Method</span></span>   | <span data-ttu-id="0400b-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="0400b-114">Return Type</span></span>|<span data-ttu-id="0400b-115">说明</span><span class="sxs-lookup"><span data-stu-id="0400b-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0400b-116">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0400b-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="0400b-117">[riskyUser](riskyuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0400b-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="0400b-118">列出有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="0400b-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="0400b-119">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="0400b-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="0400b-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="0400b-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="0400b-121">获取特定有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="0400b-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="0400b-122">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="0400b-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="0400b-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0400b-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="0400b-124">获取 Azure AD 用户的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="0400b-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="0400b-125">确认 riskyUsers 泄露</span><span class="sxs-lookup"><span data-stu-id="0400b-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="0400b-126">无</span><span class="sxs-lookup"><span data-stu-id="0400b-126">None</span></span> |<span data-ttu-id="0400b-127">确认风险用户受到威胁。</span><span class="sxs-lookup"><span data-stu-id="0400b-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="0400b-128">消除 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0400b-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="0400b-129">无</span><span class="sxs-lookup"><span data-stu-id="0400b-129">None</span></span> | <span data-ttu-id="0400b-130">消除风险用户的风险。</span><span class="sxs-lookup"><span data-stu-id="0400b-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="0400b-131">属性</span><span class="sxs-lookup"><span data-stu-id="0400b-131">Properties</span></span>

| <span data-ttu-id="0400b-132">属性</span><span class="sxs-lookup"><span data-stu-id="0400b-132">Property</span></span>   | <span data-ttu-id="0400b-133">类型</span><span class="sxs-lookup"><span data-stu-id="0400b-133">Type</span></span>|<span data-ttu-id="0400b-134">说明</span><span class="sxs-lookup"><span data-stu-id="0400b-134">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="0400b-135">处于风险中的用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="0400b-135">Unique ID of the user at risk.</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="0400b-136">指示是否删除用户。</span><span class="sxs-lookup"><span data-stu-id="0400b-136">Indicates whether the user is deleted.</span></span> <span data-ttu-id="0400b-137">可取值为：`true`、`false`。</span><span class="sxs-lookup"><span data-stu-id="0400b-137">Possible values are: `true`, `false`.</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="0400b-138">指示后端是否正在处理用户的风险状态。</span><span class="sxs-lookup"><span data-stu-id="0400b-138">Indicates whether a user's risky state is being processed by the backend.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="0400b-139">风险用户上次更新的日期和时间</span><span class="sxs-lookup"><span data-stu-id="0400b-139">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="0400b-140">可能的值为低、中、高、隐藏、无、unknownFutureValue。</span><span class="sxs-lookup"><span data-stu-id="0400b-140">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="0400b-141">可能的值是 none、confirmedSafe、修正、atRisk、unknownFutureValue。</span><span class="sxs-lookup"><span data-stu-id="0400b-141">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="0400b-142">可能的值为 none、adminGeneratedTemporaryPassword、 userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromed、hidden、adminConfirmedUserCompromed、unknownFutureValue。</span><span class="sxs-lookup"><span data-stu-id="0400b-142">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="0400b-143">有风险的用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="0400b-143">Risky user display name.</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="0400b-144">有风险的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="0400b-144">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0400b-145">关系</span><span class="sxs-lookup"><span data-stu-id="0400b-145">Relationships</span></span>

<span data-ttu-id="0400b-146">无。</span><span class="sxs-lookup"><span data-stu-id="0400b-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0400b-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0400b-147">JSON representation</span></span>

<span data-ttu-id="0400b-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0400b-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isProcessing": "boolean",
"isDeleted": "boolean",
"riskDetail":  "string",
"riskLevel":  "string",
"riskState":  "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
