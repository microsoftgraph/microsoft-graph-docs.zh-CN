---
title: riskyUsers 资源类型
description: 代表 Azure AD 用户面临危险。 Azure AD 不断计算用户根据各种信号和机器学习的风险。 此 API 在 Azure AD 中所有存在风险的用户提供编程访问。
author: cloudhandler
ms.openlocfilehash: bc8b64b93662511fffe709a18fb3e7210f3a941b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748260"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="3a5fb-105">riskyUsers 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a5fb-105">riskyUsers resource type</span></span>

> <span data-ttu-id="3a5fb-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a5fb-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a5fb-108">代表 Azure AD 用户面临危险。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-108">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="3a5fb-109">Azure AD 不断计算用户根据各种信号和机器学习的风险。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-109">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="3a5fb-110">此 API 在 Azure AD 中所有存在风险的用户提供编程访问。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-110">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="3a5fb-111">**注意：** 此 API 要求的 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-111">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="3a5fb-112">有关风险事件的详细信息，请参阅[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-112">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="3a5fb-113">方法</span><span class="sxs-lookup"><span data-stu-id="3a5fb-113">Methods</span></span>

| <span data-ttu-id="3a5fb-114">方法</span><span class="sxs-lookup"><span data-stu-id="3a5fb-114">Method</span></span>   | <span data-ttu-id="3a5fb-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="3a5fb-115">Return Type</span></span>|<span data-ttu-id="3a5fb-116">说明</span><span class="sxs-lookup"><span data-stu-id="3a5fb-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3a5fb-117">列表 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3a5fb-117">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="3a5fb-118">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3a5fb-118">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="3a5fb-119">列出 risky 用户和及其属性。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-119">List risky users and their properties.</span></span>|
|[<span data-ttu-id="3a5fb-120">获取 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3a5fb-120">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="3a5fb-121">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="3a5fb-121">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="3a5fb-122">获取特定 risky 用户和其属性。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-122">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="3a5fb-123">属性</span><span class="sxs-lookup"><span data-stu-id="3a5fb-123">Properties</span></span>

| <span data-ttu-id="3a5fb-124">属性</span><span class="sxs-lookup"><span data-stu-id="3a5fb-124">Property</span></span>   | <span data-ttu-id="3a5fb-125">类型</span><span class="sxs-lookup"><span data-stu-id="3a5fb-125">Type</span></span>|<span data-ttu-id="3a5fb-126">说明</span><span class="sxs-lookup"><span data-stu-id="3a5fb-126">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="3a5fb-127">风险的用户的唯一 id</span><span class="sxs-lookup"><span data-stu-id="3a5fb-127">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="3a5fb-128">指示是否删除用户。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-128">Indicates whether the user is deleted.</span></span> <span data-ttu-id="3a5fb-129">可能的值为： `true`，`false`</span><span class="sxs-lookup"><span data-stu-id="3a5fb-129">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="3a5fb-130">指示用户是否来宾用户。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-130">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="3a5fb-131">可取值为：`true`、`false`。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-131">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="3a5fb-132">如果用户的标识位于中考虑租户之外，则为 true。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-132">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="3a5fb-133">此用户可以在 Azure AD，MSA 中是 B2B 或 B2C 用户标识或第三方标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-133">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="3a5fb-134">如果用户的标识位于内部中考虑租户则为 false</span><span class="sxs-lookup"><span data-stu-id="3a5fb-134">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="3a5fb-135">提供原因后面的 risky 用户、 登录或风险事件特定状态。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-135">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3a5fb-136">可能的值为： `none`， `adminGeneratedTemporaryPassword`， `userPerformedSecuredPasswordChange`， `userPerformedSecuredPasswordReset`， `adminConfirmedSigninSafe`， `aiConfirmedSigninSafe`， `userPassedMFADrivenByRiskBasedPolicy`， `adminDismissedAllRiskForUser`， `adminConfirmedSigninCompromised`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-136">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="3a5fb-137">值`none`是指的任何操作已执行上的用户或登录到目前为止。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-137">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="3a5fb-138">提供 risky 用户、 登录或风险事件的总体风险级别。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-138">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3a5fb-139">可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-139">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="3a5fb-140">值`hidden`是指为 Azure AD 身份保护未启用的用户或登录。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-140">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="3a5fb-141">提供 risky 用户、 登录或风险事件的风险状态。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-141">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="3a5fb-142">可能的值为： `none`， `confirmedSafe`， `remediated`， `dismissed`， `atRisk`， `confirmedCompromised`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-142">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="3a5fb-143">日期和 risky 用户上次更新时间</span><span class="sxs-lookup"><span data-stu-id="3a5fb-143">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="3a5fb-144">Risky 的用户显示名称</span><span class="sxs-lookup"><span data-stu-id="3a5fb-144">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="3a5fb-145">Risky 的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="3a5fb-145">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a5fb-146">Relationships</span><span class="sxs-lookup"><span data-stu-id="3a5fb-146">Relationships</span></span>

| <span data-ttu-id="3a5fb-147">关系</span><span class="sxs-lookup"><span data-stu-id="3a5fb-147">Relationship</span></span> | <span data-ttu-id="3a5fb-148">类型</span><span class="sxs-lookup"><span data-stu-id="3a5fb-148">Type</span></span> |<span data-ttu-id="3a5fb-149">说明</span><span class="sxs-lookup"><span data-stu-id="3a5fb-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a5fb-150">ID</span><span class="sxs-lookup"><span data-stu-id="3a5fb-150">id</span></span>|<span data-ttu-id="3a5fb-151">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="3a5fb-151">UserObjectId</span></span>| <span data-ttu-id="3a5fb-152">与给定的风险事件相关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-152">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="3a5fb-153">isGuest</span><span class="sxs-lookup"><span data-stu-id="3a5fb-153">isGuest</span></span>|<span data-ttu-id="3a5fb-154">isGuest</span><span class="sxs-lookup"><span data-stu-id="3a5fb-154">isGuest</span></span>| <span data-ttu-id="3a5fb-155">Risky 用户可以是家庭用户 (B2E) 或来宾用户 （B2B、 B2C）。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-155">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="3a5fb-156">被</span><span class="sxs-lookup"><span data-stu-id="3a5fb-156">isDeleted</span></span>|<span data-ttu-id="3a5fb-157">被</span><span class="sxs-lookup"><span data-stu-id="3a5fb-157">isDeleted</span></span>| <span data-ttu-id="3a5fb-158">用户可能也不能删除。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-158">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="3a5fb-159">riskState</span><span class="sxs-lookup"><span data-stu-id="3a5fb-159">riskState</span></span>|<span data-ttu-id="3a5fb-160">riskState</span><span class="sxs-lookup"><span data-stu-id="3a5fb-160">riskState</span></span>| <span data-ttu-id="3a5fb-161">Risky 用户可能存在多个状态之一。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-161">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="3a5fb-162">riskDetail</span><span class="sxs-lookup"><span data-stu-id="3a5fb-162">riskDetail</span></span>|<span data-ttu-id="3a5fb-163">riskDetail</span><span class="sxs-lookup"><span data-stu-id="3a5fb-163">riskDetail</span></span>| <span data-ttu-id="3a5fb-164">特定状态中，risky 用户可能会因多个原因。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-164">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="3a5fb-165">riskLevel</span><span class="sxs-lookup"><span data-stu-id="3a5fb-165">riskLevel</span></span>|<span data-ttu-id="3a5fb-166">riskLevel</span><span class="sxs-lookup"><span data-stu-id="3a5fb-166">riskLevel</span></span>| <span data-ttu-id="3a5fb-167">Risky 用户可以被视为多个风险级别之一。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-167">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3a5fb-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a5fb-168">JSON representation</span></span>

<span data-ttu-id="3a5fb-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a5fb-169">Here is a JSON representation of the resource.</span></span>

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
"riskState":  {"@odata.type": "microsoft.graph.riskState"},
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
