---
title: riskyUser 资源类型
description: 表示有风险的 Azure AD 用户。 Azure AD 会根据各种信号和机器学习持续评估用户风险。 此 API 提供对 Azure AD 中所有风险用户的编程访问。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7759a9c42ca9178dc95266ffa4630ef891832ecd
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062635"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="aa43d-105">riskyUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa43d-105">riskyUser resource type</span></span>

<span data-ttu-id="aa43d-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa43d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa43d-107">表示有风险的 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="aa43d-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="aa43d-108">Azure AD 会根据各种信号和机器学习持续评估用户风险。</span><span class="sxs-lookup"><span data-stu-id="aa43d-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="aa43d-109">此 API 提供对 Azure AD 中所有风险用户的编程访问。</span><span class="sxs-lookup"><span data-stu-id="aa43d-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="aa43d-110">有关风险事件的详细信息，请参阅[Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)。</span><span class="sxs-lookup"><span data-stu-id="aa43d-110">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="aa43d-111">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="aa43d-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="aa43d-112">方法</span><span class="sxs-lookup"><span data-stu-id="aa43d-112">Methods</span></span>

| <span data-ttu-id="aa43d-113">方法</span><span class="sxs-lookup"><span data-stu-id="aa43d-113">Method</span></span>   | <span data-ttu-id="aa43d-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa43d-114">Return Type</span></span>|<span data-ttu-id="aa43d-115">说明</span><span class="sxs-lookup"><span data-stu-id="aa43d-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa43d-116">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="aa43d-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="aa43d-117">[riskyUser](riskyuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="aa43d-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="aa43d-118">列出有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="aa43d-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="aa43d-119">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="aa43d-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="aa43d-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="aa43d-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="aa43d-121">获取特定的有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="aa43d-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="aa43d-122">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="aa43d-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="aa43d-123">[riskyUserHistoryItem](riskyuserhistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="aa43d-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="aa43d-124">获取 Azure AD 用户的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="aa43d-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="aa43d-125">确认 riskyUsers 已泄露</span><span class="sxs-lookup"><span data-stu-id="aa43d-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="aa43d-126">无</span><span class="sxs-lookup"><span data-stu-id="aa43d-126">None</span></span> |<span data-ttu-id="aa43d-127">确认有风险的用户受到威胁。</span><span class="sxs-lookup"><span data-stu-id="aa43d-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="aa43d-128">消除 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="aa43d-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="aa43d-129">无</span><span class="sxs-lookup"><span data-stu-id="aa43d-129">None</span></span> | <span data-ttu-id="aa43d-130">消除有风险的用户的风险。</span><span class="sxs-lookup"><span data-stu-id="aa43d-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa43d-131">属性</span><span class="sxs-lookup"><span data-stu-id="aa43d-131">Properties</span></span>

| <span data-ttu-id="aa43d-132">属性</span><span class="sxs-lookup"><span data-stu-id="aa43d-132">Property</span></span>   | <span data-ttu-id="aa43d-133">类型</span><span class="sxs-lookup"><span data-stu-id="aa43d-133">Type</span></span>|<span data-ttu-id="aa43d-134">说明</span><span class="sxs-lookup"><span data-stu-id="aa43d-134">Description</span></span>|
|:---------------|:--------|:----------|
|`id`|`string`|<span data-ttu-id="aa43d-135">用户面临风险的唯一 id</span><span class="sxs-lookup"><span data-stu-id="aa43d-135">Unique id of the user at risk</span></span>|
|`isDeleted`|`bool`|<span data-ttu-id="aa43d-136">指示是否删除用户。</span><span class="sxs-lookup"><span data-stu-id="aa43d-136">Indicates whether the user is deleted.</span></span> <span data-ttu-id="aa43d-137">可能的值包括`true`：、`false`</span><span class="sxs-lookup"><span data-stu-id="aa43d-137">Possible values are: `true`, `false`</span></span>|
|`isGuest`|`bool`|<span data-ttu-id="aa43d-138">指示用户是否为来宾用户。</span><span class="sxs-lookup"><span data-stu-id="aa43d-138">Indicates whether the user is a guest user.</span></span> <span data-ttu-id="aa43d-139">可取值为：`true`、`false`。</span><span class="sxs-lookup"><span data-stu-id="aa43d-139">Possible values are: `true`, `false`.</span></span> <span data-ttu-id="aa43d-140">如此如果用户的标识位于租户外部，请考虑。</span><span class="sxs-lookup"><span data-stu-id="aa43d-140">True if user’s identity lies outside of the tenant in consideration.</span></span> <span data-ttu-id="aa43d-141">此用户可以是在 Azure AD、MSA 或第三方标识提供程序中具有标识的 B2B 或 B2C 用户。</span><span class="sxs-lookup"><span data-stu-id="aa43d-141">This user could be a B2B or a B2C user with identity in Azure AD, MSA or 3rd party identity provider.</span></span> <span data-ttu-id="aa43d-142">假如果用户的标识位于租户内部，则考虑</span><span class="sxs-lookup"><span data-stu-id="aa43d-142">False if user’s identity lies inside the tenant in consideration</span></span>|
|`isProcessing`|`bool`|<span data-ttu-id="aa43d-143">指示后端正在处理用户的危险状态 wehther</span><span class="sxs-lookup"><span data-stu-id="aa43d-143">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|`riskLastUpdatedDateTime`|`datetime`|<span data-ttu-id="aa43d-144">上次更新有风险的用户的日期和时间</span><span class="sxs-lookup"><span data-stu-id="aa43d-144">The date and time that the risky user was last updated</span></span>|
|`riskLevel`|`riskLevel`| <span data-ttu-id="aa43d-145">可能的值为 low、medium、high、hidden、none、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="aa43d-145">The possible values are low, medium, high, hidden, none, unknownFutureValue.</span></span>  |
|`riskState`|`riskState`| <span data-ttu-id="aa43d-146">可能的值为 none、confirmedSafe、修正、atRisk、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="aa43d-146">The possible values are none, confirmedSafe, remediated, atRisk, unknownFutureValue.</span></span>  |
|`riskDetail`|`riskDetail`| <span data-ttu-id="aa43d-147">可能的值为 none、adminGeneratedTemporaryPassword、userPerformedSecuredPasswordChange、userPerformedSecuredPasswordReset、adminConfirmedSigninSafe、aiConfirmedSigninSafe、userPassedMFADrivenByRiskBasedPolicy、adminDismissedAllRiskForUser、adminConfirmedSigninCompromised、hidden、adminConfirmedUserCompromised、向 unknownfuturevalue。</span><span class="sxs-lookup"><span data-stu-id="aa43d-147">The possible values are none, adminGeneratedTemporaryPassword, userPerformedSecuredPasswordChange, userPerformedSecuredPasswordReset, adminConfirmedSigninSafe, aiConfirmedSigninSafe, userPassedMFADrivenByRiskBasedPolicy, adminDismissedAllRiskForUser, adminConfirmedSigninCompromised, hidden, adminConfirmedUserCompromised, unknownFutureValue.</span></span>  |
|`userDisplayName`|`string`|<span data-ttu-id="aa43d-148">有风险的用户显示名称</span><span class="sxs-lookup"><span data-stu-id="aa43d-148">Risky user display name</span></span>|
|`userPrincipalName`|`string`|<span data-ttu-id="aa43d-149">有风险的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="aa43d-149">Risky user principal name</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa43d-150">关系</span><span class="sxs-lookup"><span data-stu-id="aa43d-150">Relationships</span></span>

<span data-ttu-id="aa43d-151">无。</span><span class="sxs-lookup"><span data-stu-id="aa43d-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa43d-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa43d-152">JSON representation</span></span>

<span data-ttu-id="aa43d-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa43d-153">The following is a JSON representation of the resource.</span></span>

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
