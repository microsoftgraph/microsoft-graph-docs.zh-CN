---
title: riskyUser 资源类型
description: 表示有风险的 Azure AD 用户。 Azure AD 会根据各种信号和机器学习持续评估用户风险。 此 API 提供对 Azure AD 中所有风险用户的编程访问。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 179a6cbddf3e4b27c47761bd81aad1052ae7f728
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343533"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="e8384-105">riskyUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8384-105">riskyUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8384-106">表示有风险的 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="e8384-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="e8384-107">Azure AD 会根据各种信号和机器学习持续评估用户风险。</span><span class="sxs-lookup"><span data-stu-id="e8384-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="e8384-108">此 API 提供对 Azure AD 中所有风险用户的编程访问。</span><span class="sxs-lookup"><span data-stu-id="e8384-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="e8384-109">有关风险事件的详细信息, 请参阅[Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)。</span><span class="sxs-lookup"><span data-stu-id="e8384-109">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="e8384-110">**注意:** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="e8384-110">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="e8384-111">方法</span><span class="sxs-lookup"><span data-stu-id="e8384-111">Methods</span></span>

| <span data-ttu-id="e8384-112">方法</span><span class="sxs-lookup"><span data-stu-id="e8384-112">Method</span></span>   | <span data-ttu-id="e8384-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="e8384-113">Return Type</span></span>|<span data-ttu-id="e8384-114">说明</span><span class="sxs-lookup"><span data-stu-id="e8384-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8384-115">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e8384-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="e8384-116">[riskyUser](riskyUser.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8384-116">[riskyUser](riskyUser.md) collection</span></span>|<span data-ttu-id="e8384-117">列出有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="e8384-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="e8384-118">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="e8384-118">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="e8384-119">riskyUser</span><span class="sxs-lookup"><span data-stu-id="e8384-119">riskyUser</span></span>](riskyUser.md)|<span data-ttu-id="e8384-120">获取特定的有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="e8384-120">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="e8384-121">确认 riskyUsers 已泄露</span><span class="sxs-lookup"><span data-stu-id="e8384-121">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="e8384-122">无</span><span class="sxs-lookup"><span data-stu-id="e8384-122">None</span></span> |<span data-ttu-id="e8384-123">确认有风险的用户受到威胁。</span><span class="sxs-lookup"><span data-stu-id="e8384-123">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="e8384-124">消除 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="e8384-124">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="e8384-125">无</span><span class="sxs-lookup"><span data-stu-id="e8384-125">None</span></span> | <span data-ttu-id="e8384-126">消除有风险的用户的风险。</span><span class="sxs-lookup"><span data-stu-id="e8384-126">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="e8384-127">属性</span><span class="sxs-lookup"><span data-stu-id="e8384-127">Properties</span></span>

| <span data-ttu-id="e8384-128">属性</span><span class="sxs-lookup"><span data-stu-id="e8384-128">Property</span></span>   | <span data-ttu-id="e8384-129">类型</span><span class="sxs-lookup"><span data-stu-id="e8384-129">Type</span></span>|<span data-ttu-id="e8384-130">说明</span><span class="sxs-lookup"><span data-stu-id="e8384-130">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="e8384-131">用户面临风险的唯一 id</span><span class="sxs-lookup"><span data-stu-id="e8384-131">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="e8384-132">指示是否删除用户。</span><span class="sxs-lookup"><span data-stu-id="e8384-132">Indicates whether the user is deleted.</span></span> <span data-ttu-id="e8384-133">可能的值包括`true`:、`false`</span><span class="sxs-lookup"><span data-stu-id="e8384-133">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="e8384-134">指示用户是否为来宾用户。</span><span class="sxs-lookup"><span data-stu-id="e8384-134">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="e8384-135">可取值为：`true`、`false`。</span><span class="sxs-lookup"><span data-stu-id="e8384-135">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="e8384-136">如此如果用户的标识位于租户外部, 请考虑。</span><span class="sxs-lookup"><span data-stu-id="e8384-136">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="e8384-137">此用户可以是在 Azure AD、MSA 或第三方标识提供程序中具有标识的 B2B 或 B2C 用户。</span><span class="sxs-lookup"><span data-stu-id="e8384-137">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="e8384-138">假如果用户的标识位于租户内部, 则考虑</span><span class="sxs-lookup"><span data-stu-id="e8384-138">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="e8384-139">指示后端正在处理用户的危险状态 wehther</span><span class="sxs-lookup"><span data-stu-id="e8384-139">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="e8384-140">上次更新有风险的用户的日期和时间</span><span class="sxs-lookup"><span data-stu-id="e8384-140">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="e8384-141">可能的值为 low、medium、high、hidden、none、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="e8384-141">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="e8384-142">可能的值为 none、confirmedSafe、修正、atRisk、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="e8384-142">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="e8384-143">可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="e8384-143">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="e8384-144">有风险的用户显示名称</span><span class="sxs-lookup"><span data-stu-id="e8384-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="e8384-145">有风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e8384-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8384-146">关系</span><span class="sxs-lookup"><span data-stu-id="e8384-146">Relationships</span></span>
| <span data-ttu-id="e8384-147">关系</span><span class="sxs-lookup"><span data-stu-id="e8384-147">Relationship</span></span> | <span data-ttu-id="e8384-148">类型</span><span class="sxs-lookup"><span data-stu-id="e8384-148">Type</span></span>   |<span data-ttu-id="e8384-149">说明</span><span class="sxs-lookup"><span data-stu-id="e8384-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8384-150">日志</span><span class="sxs-lookup"><span data-stu-id="e8384-150">history</span></span>|<span data-ttu-id="e8384-151">[riskyUserHistoryItem](riskyuserhistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8384-151">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>| |

## <a name="json-representation"></a><span data-ttu-id="e8384-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8384-152">JSON representation</span></span>

<span data-ttu-id="e8384-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8384-153">Here is a JSON representation of the resource.</span></span>

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
"isGuest": "boolean",
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
