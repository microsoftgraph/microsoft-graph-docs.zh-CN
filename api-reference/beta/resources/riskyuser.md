---
title: riskyUsers 资源类型
description: 代表 Azure AD 用户面临危险。 Azure AD 不断计算用户根据各种信号和机器学习的风险。 此 API 在 Azure AD 中所有存在风险的用户提供编程访问。
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 27c189a81d6ba4e088c1242acfd2cf0d0f5c56c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515711"
---
# <a name="riskyusers-resource-type"></a><span data-ttu-id="8d4f0-105">riskyUsers 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d4f0-105">riskyUsers resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d4f0-106">代表 Azure AD 用户面临危险。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-106">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="8d4f0-107">Azure AD 不断计算用户根据各种信号和机器学习的风险。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-107">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="8d4f0-108">此 API 在 Azure AD 中所有存在风险的用户提供编程访问。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-108">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

> <span data-ttu-id="8d4f0-109">**注意：** 此 API 要求的 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-109">**Note:** This API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="8d4f0-110">有关风险事件的详细信息，请参阅[Azure Active Directory 标识保护](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/)。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).</span></span>

## <a name="methods"></a><span data-ttu-id="8d4f0-111">方法</span><span class="sxs-lookup"><span data-stu-id="8d4f0-111">Methods</span></span>

| <span data-ttu-id="8d4f0-112">方法</span><span class="sxs-lookup"><span data-stu-id="8d4f0-112">Method</span></span>   | <span data-ttu-id="8d4f0-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="8d4f0-113">Return Type</span></span>|<span data-ttu-id="8d4f0-114">说明</span><span class="sxs-lookup"><span data-stu-id="8d4f0-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d4f0-115">列表 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="8d4f0-115">List riskyUsers</span></span>](../api/riskyusers-list.md) | [<span data-ttu-id="8d4f0-116">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="8d4f0-116">riskyUsers</span></span>](riskyuser.md) |<span data-ttu-id="8d4f0-117">列出 risky 用户和及其属性。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-117">List risky users and their properties.</span></span>|
|[<span data-ttu-id="8d4f0-118">获取 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="8d4f0-118">Get riskyUsers</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="8d4f0-119">riskyUsers</span><span class="sxs-lookup"><span data-stu-id="8d4f0-119">riskyUsers</span></span>](riskyuser.md)|<span data-ttu-id="8d4f0-120">获取特定 risky 用户和其属性。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-120">Get a specific risky user and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d4f0-121">属性</span><span class="sxs-lookup"><span data-stu-id="8d4f0-121">Properties</span></span>

| <span data-ttu-id="8d4f0-122">属性</span><span class="sxs-lookup"><span data-stu-id="8d4f0-122">Property</span></span>   | <span data-ttu-id="8d4f0-123">类型</span><span class="sxs-lookup"><span data-stu-id="8d4f0-123">Type</span></span>|<span data-ttu-id="8d4f0-124">说明</span><span class="sxs-lookup"><span data-stu-id="8d4f0-124">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="8d4f0-125">风险的用户的唯一 id</span><span class="sxs-lookup"><span data-stu-id="8d4f0-125">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="8d4f0-126">指示是否删除用户。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-126">Indicates whether the user is deleted.</span></span> <span data-ttu-id="8d4f0-127">可能的值为： `true`，`false`</span><span class="sxs-lookup"><span data-stu-id="8d4f0-127">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="8d4f0-128">指示用户是否来宾用户。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-128">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="8d4f0-129">可取值为：`true`、`false`。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-129">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="8d4f0-130">如果用户的标识位于中考虑租户之外，则为 true。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-130">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="8d4f0-131">此用户可以在 Azure AD，MSA 中是 B2B 或 B2C 用户标识或第三方标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-131">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="8d4f0-132">如果用户的标识位于内部中考虑租户则为 false</span><span class="sxs-lookup"><span data-stu-id="8d4f0-132">False if user’s identity lies inside the tenant in consideration</span></span>|
|`riskDetail`|`riskDetail`|<span data-ttu-id="8d4f0-133">提供原因后面的 risky 用户、 登录或风险事件特定状态。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-133">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="8d4f0-134">可能的值为： `none`， `adminGeneratedTemporaryPassword`， `userPerformedSecuredPasswordChange`， `userPerformedSecuredPasswordReset`， `adminConfirmedSigninSafe`， `aiConfirmedSigninSafe`， `userPassedMFADrivenByRiskBasedPolicy`， `adminDismissedAllRiskForUser`， `adminConfirmedSigninCompromised`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-134">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="8d4f0-135">值`none`是指的任何操作已执行上的用户或登录到目前为止。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-135">The value `none` means that no action has been performed on the user or sign-in so far.</span></span>|
|`riskLevel`|`riskLevel`|<span data-ttu-id="8d4f0-136">提供 risky 用户、 登录或风险事件的总体风险级别。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-136">Provides the overall risk level of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="8d4f0-137">可能的值为： `none`， `low`， `medium`， `high`， `hidden`，和`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-137">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="8d4f0-138">值`hidden`是指为 Azure AD 身份保护未启用的用户或登录。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-138">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span>|
|`riskState`|`riskState`|<span data-ttu-id="8d4f0-139">提供 risky 用户、 登录或风险事件的风险状态。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-139">Provides the 'risk state' of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="8d4f0-140">可取值包括：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-140">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="8d4f0-141">日期和 risky 用户上次更新时间</span><span class="sxs-lookup"><span data-stu-id="8d4f0-141">The date and time that the risky user was last updated</span></span>|
|`userDisplayName`|`string`|<span data-ttu-id="8d4f0-142">Risky 的用户显示名称</span><span class="sxs-lookup"><span data-stu-id="8d4f0-142">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="8d4f0-143">Risky 的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="8d4f0-143">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d4f0-144">关系</span><span class="sxs-lookup"><span data-stu-id="8d4f0-144">Relationships</span></span>

| <span data-ttu-id="8d4f0-145">关系</span><span class="sxs-lookup"><span data-stu-id="8d4f0-145">Relationship</span></span> | <span data-ttu-id="8d4f0-146">类型</span><span class="sxs-lookup"><span data-stu-id="8d4f0-146">Type</span></span> |<span data-ttu-id="8d4f0-147">说明</span><span class="sxs-lookup"><span data-stu-id="8d4f0-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d4f0-148">id</span><span class="sxs-lookup"><span data-stu-id="8d4f0-148">id</span></span>|<span data-ttu-id="8d4f0-149">UserObjectId</span><span class="sxs-lookup"><span data-stu-id="8d4f0-149">UserObjectId</span></span>| <span data-ttu-id="8d4f0-150">与给定的风险事件相关联的用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-150">The unique identifier of the user with which a given risk event is associated with.</span></span>|
|<span data-ttu-id="8d4f0-151">isGuest</span><span class="sxs-lookup"><span data-stu-id="8d4f0-151">isGuest</span></span>|<span data-ttu-id="8d4f0-152">isGuest</span><span class="sxs-lookup"><span data-stu-id="8d4f0-152">isGuest</span></span>| <span data-ttu-id="8d4f0-153">Risky 用户可以是家庭用户 (B2E) 或来宾用户 （B2B、 B2C）。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-153">A risky user could be either a Home user (B2E) or a Guest user (B2B, B2C).</span></span>|
|<span data-ttu-id="8d4f0-154">被</span><span class="sxs-lookup"><span data-stu-id="8d4f0-154">isDeleted</span></span>|<span data-ttu-id="8d4f0-155">被</span><span class="sxs-lookup"><span data-stu-id="8d4f0-155">isDeleted</span></span>| <span data-ttu-id="8d4f0-156">用户可能也不能删除。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-156">A user may or may not be deleted.</span></span> |
|<span data-ttu-id="8d4f0-157">riskState</span><span class="sxs-lookup"><span data-stu-id="8d4f0-157">riskState</span></span>|<span data-ttu-id="8d4f0-158">riskState</span><span class="sxs-lookup"><span data-stu-id="8d4f0-158">riskState</span></span>| <span data-ttu-id="8d4f0-159">Risky 用户可能存在多个状态之一。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-159">A risky user could exist in one of multiple states.</span></span> |
|<span data-ttu-id="8d4f0-160">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8d4f0-160">riskDetail</span></span>|<span data-ttu-id="8d4f0-161">riskDetail</span><span class="sxs-lookup"><span data-stu-id="8d4f0-161">riskDetail</span></span>| <span data-ttu-id="8d4f0-162">特定状态中，risky 用户可能会因多个原因。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-162">A risky user could be in a certain state because of multiple reasons.</span></span> |
|<span data-ttu-id="8d4f0-163">riskLevel</span><span class="sxs-lookup"><span data-stu-id="8d4f0-163">riskLevel</span></span>|<span data-ttu-id="8d4f0-164">riskLevel</span><span class="sxs-lookup"><span data-stu-id="8d4f0-164">riskLevel</span></span>| <span data-ttu-id="8d4f0-165">Risky 用户可以被视为多个风险级别之一。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-165">A risky user could be considered one of multiple risk levels.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8d4f0-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d4f0-166">JSON representation</span></span>

<span data-ttu-id="8d4f0-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d4f0-167">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/riskyuser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
