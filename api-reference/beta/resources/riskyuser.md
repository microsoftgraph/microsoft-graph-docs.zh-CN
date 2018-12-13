---
title: riskyUsers 资源类型
description: 代表 Azure AD 用户面临危险。 Azure AD 不断计算用户根据各种信号和机器学习的风险。 此 API 在 Azure AD 中所有存在风险的用户提供编程访问。
ms.openlocfilehash: 47856ab28a52046f19087e0f59745efb9855e81a
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241060"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="0b3ff-105">riskyUsers 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b3ff-105">riskyUsers resource type</span></span>

> <span data-ttu-id="0b3ff-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b3ff-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b3ff-108">代表 Azure AD 用户面临危险。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="0b3ff-109">Azure AD 不断计算用户根据各种信号和机器学习的风险。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="0b3ff-110">此 API 在 Azure AD 中所有存在风险的用户提供编程访问。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="0b3ff-111">**注意：** 此 API 要求的 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-111">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="0b3ff-112">有关风险事件的详细信息，请参阅[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-112">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="0b3ff-113">方法</span><span class="sxs-lookup"><span data-stu-id="0b3ff-113">Methods</span></span>

| <span data-ttu-id="0b3ff-114">方法</span><span class="sxs-lookup"><span data-stu-id="0b3ff-114">Method</span></span>   | <span data-ttu-id="0b3ff-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b3ff-115">Return Type</span></span>|<span data-ttu-id="0b3ff-116">说明</span><span class="sxs-lookup"><span data-stu-id="0b3ff-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0b3ff-117">列表 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0b3ff-117">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="0b3ff-118">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0b3ff-118">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="0b3ff-119">列出 risky 用户和及其属性。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-119">List risky users and their properties.</span></span>|
|[<span data-ttu-id="0b3ff-120">获取 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0b3ff-120">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="0b3ff-121">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="0b3ff-121">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="0b3ff-122">获取特定 risky 用户和其属性。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-122">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="0b3ff-123">属性</span><span class="sxs-lookup"><span data-stu-id="0b3ff-123">Properties</span></span>

| <span data-ttu-id="0b3ff-124">属性</span><span class="sxs-lookup"><span data-stu-id="0b3ff-124">Property</span></span>   | <span data-ttu-id="0b3ff-125">类型</span><span class="sxs-lookup"><span data-stu-id="0b3ff-125">Type</span></span>|<span data-ttu-id="0b3ff-126">说明</span><span class="sxs-lookup"><span data-stu-id="0b3ff-126">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="0b3ff-127">风险的用户的唯一 id</span><span class="sxs-lookup"><span data-stu-id="0b3ff-127">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="0b3ff-128">指示是否删除用户。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-128">Indicates whether the user is deleted.</span></span> <span data-ttu-id="0b3ff-129">可能的值为： `true`，`false`</span><span class="sxs-lookup"><span data-stu-id="0b3ff-129">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="0b3ff-130">指示用户是否来宾用户。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-130">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="0b3ff-131">可取值为：`true`、`false`。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-131">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="0b3ff-132">如果用户的标识位于中考虑租户之外，则为 true。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-132">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="0b3ff-133">此用户可以在 Azure AD，MSA 中是 B2B 或 B2C 用户标识或第三方标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-133">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="0b3ff-134">如果用户的标识位于内部中考虑租户则为 false</span><span class="sxs-lookup"><span data-stu-id="0b3ff-134">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="0b3ff-135">提供原因后面的 risky 用户、 登录或风险事件特定状态。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-135">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="0b3ff-136">可能的值为： `none`， `adminGeneratedTemporaryPassword`， `userPerformedSecuredPasswordChange`， `userPerformedSecuredPasswordReset`， `adminConfirmedSigninSafe`， `aiConfirmedSigninSafe`， `userPassedMFADrivenByRiskBasedPolicy`， `adminDismissedAllRiskForUser`， `adminConfirmedSigninCompromised`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-136">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="0b3ff-137">值`none`是指的任何操作已执行上的用户或登录到目前为止。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-137">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="0b3ff-138">提供 risky 用户、 登录或风险事件的总体风险级别。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-138">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="0b3ff-139">可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-139">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="0b3ff-140">值`hidden`是指为 Azure AD 身份保护未启用的用户或登录。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-140">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="0b3ff-141">提供 risky 用户、 登录或风险事件的风险状态。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-141">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="0b3ff-142">可能的值为： `none`， `confirmedSafe`， `remediated`， `dismissed`， `atRisk`， `confirmedCompromised`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-142">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="0b3ff-143">日期和 risky 用户上次更新时间</span><span class="sxs-lookup"><span data-stu-id="0b3ff-143">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="0b3ff-144">Risky 的用户显示名称</span><span class="sxs-lookup"><span data-stu-id="0b3ff-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="0b3ff-145">Risky 的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="0b3ff-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b3ff-146">Relationships</span><span class="sxs-lookup"><span data-stu-id="0b3ff-146">Relationships</span></span>

| <span data-ttu-id="0b3ff-147">关系</span><span class="sxs-lookup"><span data-stu-id="0b3ff-147">Relationship</span></span> | <span data-ttu-id="0b3ff-148">类型</span><span class="sxs-lookup"><span data-stu-id="0b3ff-148">Type</span></span> |<span data-ttu-id="0b3ff-149">说明</span><span class="sxs-lookup"><span data-stu-id="0b3ff-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b3ff-150">ID</span><span class="sxs-lookup"><span data-stu-id="0b3ff-150">id</span></span>|<span data-ttu-id="0b3ff-151">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="0b3ff-151">UserObjectId</span></span>| <span data-ttu-id="0b3ff-152">与给定的风险事件相关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-152">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="0b3ff-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="0b3ff-153">isGuest</span></span>|<span data-ttu-id="0b3ff-154">isGuest</span><span class="sxs-lookup"><span data-stu-id="0b3ff-154">isGuest</span></span>| <span data-ttu-id="0b3ff-155">Risky 用户可以是家庭用户 (B2E) 或来宾用户 （B2B、 B2C）。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-155">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="0b3ff-156">被</span><span class="sxs-lookup"><span data-stu-id="0b3ff-156">isDeleted</span></span>|<span data-ttu-id="0b3ff-157">被</span><span class="sxs-lookup"><span data-stu-id="0b3ff-157">isDeleted</span></span>| <span data-ttu-id="0b3ff-158">用户可能也不能删除。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-158">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="0b3ff-159">riskState</span><span class="sxs-lookup"><span data-stu-id="0b3ff-159">riskState</span></span>|<span data-ttu-id="0b3ff-160">riskState</span><span class="sxs-lookup"><span data-stu-id="0b3ff-160">riskState</span></span>| <span data-ttu-id="0b3ff-161">Risky 用户可能存在多个状态之一。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-161">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="0b3ff-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0b3ff-162">riskDetail</span></span>|<span data-ttu-id="0b3ff-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0b3ff-163">riskDetail</span></span>| <span data-ttu-id="0b3ff-164">特定状态中，risky 用户可能会因多个原因。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-164">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="0b3ff-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0b3ff-165">riskLevel</span></span>|<span data-ttu-id="0b3ff-166">riskLevel</span><span class="sxs-lookup"><span data-stu-id="0b3ff-166">riskLevel</span></span>| <span data-ttu-id="0b3ff-167">Risky 用户可以被视为多个风险级别之一。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-167">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0b3ff-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b3ff-168">JSON representation</span></span>

<span data-ttu-id="0b3ff-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b3ff-169">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"}
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
