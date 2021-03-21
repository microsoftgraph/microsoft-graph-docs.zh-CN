---
title: riskyUser 资源类型
description: 表示处于风险中的 Azure AD 用户。 Azure AD 根据各种信号和机器学习持续评估用户风险。 此 API 为 Azure AD 中所有处于风险中的用户提供编程访问权限。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
ms.openlocfilehash: d2e0942e92b1dcd648812503a923dac51a640be1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960318"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="55810-105">riskyUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="55810-105">riskyUser resource type</span></span>

<span data-ttu-id="55810-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55810-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55810-107">表示处于风险中的 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="55810-107">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="55810-108">Azure AD 根据各种信号和机器学习持续评估用户风险。</span><span class="sxs-lookup"><span data-stu-id="55810-108">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="55810-109">此 API 为 Azure AD 中所有处于风险中的用户提供编程访问权限。</span><span class="sxs-lookup"><span data-stu-id="55810-109">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="55810-110">有关风险事件详细信息，请参阅 Azure [Active Directory Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="55810-110">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="55810-111">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="55810-111">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="55810-112">Methods</span><span class="sxs-lookup"><span data-stu-id="55810-112">Methods</span></span>

| <span data-ttu-id="55810-113">方法</span><span class="sxs-lookup"><span data-stu-id="55810-113">Method</span></span>   | <span data-ttu-id="55810-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="55810-114">Return Type</span></span>|<span data-ttu-id="55810-115">说明</span><span class="sxs-lookup"><span data-stu-id="55810-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55810-116">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="55810-116">List riskyUsers</span></span>](../api/riskyusers-list.md) | <span data-ttu-id="55810-117">[riskyUser](riskyuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55810-117">[riskyUser](riskyuser.md) collection</span></span>|<span data-ttu-id="55810-118">列出有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="55810-118">List risky users and their properties.</span></span>|
|[<span data-ttu-id="55810-119">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="55810-119">Get riskyUser</span></span>](../api/riskyusers-get.md) | [<span data-ttu-id="55810-120">riskyUser</span><span class="sxs-lookup"><span data-stu-id="55810-120">riskyUser</span></span>](riskyuser.md)|<span data-ttu-id="55810-121">获取特定有风险的用户及其属性。</span><span class="sxs-lookup"><span data-stu-id="55810-121">Get a specific risky user and its properties.</span></span>|
|[<span data-ttu-id="55810-122">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="55810-122">List history</span></span>](../api/riskyuser-list-history.md) | <span data-ttu-id="55810-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="55810-123">[riskyUserHistoryItem](riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="55810-124">获取 Azure AD 用户的风险历史记录。</span><span class="sxs-lookup"><span data-stu-id="55810-124">Get the risk history of an Azure AD user.</span></span>|
|[<span data-ttu-id="55810-125">确认 riskyUsers 遭到入侵</span><span class="sxs-lookup"><span data-stu-id="55810-125">Confirm riskyUsers compromised</span></span>](../api/riskyusers-confirmcompromised.md)|<span data-ttu-id="55810-126">无</span><span class="sxs-lookup"><span data-stu-id="55810-126">None</span></span> |<span data-ttu-id="55810-127">确认存在风险的用户是否遭到入侵。</span><span class="sxs-lookup"><span data-stu-id="55810-127">Confirm a risky user as compromised.</span></span>|
|[<span data-ttu-id="55810-128">消除 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="55810-128">Dismiss riskyUsers</span></span>](../api/riskyusers-dismiss.md)|<span data-ttu-id="55810-129">无</span><span class="sxs-lookup"><span data-stu-id="55810-129">None</span></span> | <span data-ttu-id="55810-130">消除风险用户的风险。</span><span class="sxs-lookup"><span data-stu-id="55810-130">Dismiss the risk of a risky user.</span></span>|

## <a name="properties"></a><span data-ttu-id="55810-131">属性</span><span class="sxs-lookup"><span data-stu-id="55810-131">Properties</span></span>

| <span data-ttu-id="55810-132">属性</span><span class="sxs-lookup"><span data-stu-id="55810-132">Property</span></span>   | <span data-ttu-id="55810-133">类型</span><span class="sxs-lookup"><span data-stu-id="55810-133">Type</span></span>|<span data-ttu-id="55810-134">说明</span><span class="sxs-lookup"><span data-stu-id="55810-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55810-135">id</span><span class="sxs-lookup"><span data-stu-id="55810-135">id</span></span>|<span data-ttu-id="55810-136">string</span><span class="sxs-lookup"><span data-stu-id="55810-136">string</span></span>|<span data-ttu-id="55810-137">处于风险中的用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="55810-137">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="55810-138">isDeleted</span><span class="sxs-lookup"><span data-stu-id="55810-138">isDeleted</span></span>|<span data-ttu-id="55810-139">boolean</span><span class="sxs-lookup"><span data-stu-id="55810-139">boolean</span></span>|<span data-ttu-id="55810-140">指示用户是否被删除。</span><span class="sxs-lookup"><span data-stu-id="55810-140">Indicates whether the user is deleted.</span></span> <span data-ttu-id="55810-141">可取值为：`true`、`false`。</span><span class="sxs-lookup"><span data-stu-id="55810-141">Possible values are: `true`, `false`.</span></span>|
|<span data-ttu-id="55810-142">isProcessing</span><span class="sxs-lookup"><span data-stu-id="55810-142">isProcessing</span></span>|<span data-ttu-id="55810-143">boolean</span><span class="sxs-lookup"><span data-stu-id="55810-143">boolean</span></span>|<span data-ttu-id="55810-144">指示后端是否正在处理用户的风险状态。</span><span class="sxs-lookup"><span data-stu-id="55810-144">Indicates whether a user's risky state is being processed by the backend.</span></span>|
|<span data-ttu-id="55810-145">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="55810-145">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="55810-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55810-146">DateTimeOffset</span></span>|<span data-ttu-id="55810-147">上次更新有风险用户的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="55810-147">The date and time that the risky user was last updated.</span></span>  <span data-ttu-id="55810-148">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="55810-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="55810-149">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="55810-149">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="55810-150">riskLevel</span><span class="sxs-lookup"><span data-stu-id="55810-150">riskLevel</span></span>|<span data-ttu-id="55810-151">riskLevel</span><span class="sxs-lookup"><span data-stu-id="55810-151">riskLevel</span></span>| <span data-ttu-id="55810-152">检测到的风险用户级别。</span><span class="sxs-lookup"><span data-stu-id="55810-152">Level of the detected risky user.</span></span> <span data-ttu-id="55810-153">可能的值为 `low` `medium` `high` `hidden` `none` `unknownFutureValue` 、、、。</span><span class="sxs-lookup"><span data-stu-id="55810-153">The possible values are `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="55810-154">riskState</span><span class="sxs-lookup"><span data-stu-id="55810-154">riskState</span></span>|<span data-ttu-id="55810-155">riskState</span><span class="sxs-lookup"><span data-stu-id="55810-155">riskState</span></span>| <span data-ttu-id="55810-156">用户风险的状态。</span><span class="sxs-lookup"><span data-stu-id="55810-156">State of the user's risk.</span></span> <span data-ttu-id="55810-157">可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="55810-157">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="55810-158">riskDetail</span><span class="sxs-lookup"><span data-stu-id="55810-158">riskDetail</span></span>|<span data-ttu-id="55810-159">riskDetail</span><span class="sxs-lookup"><span data-stu-id="55810-159">riskDetail</span></span>| <span data-ttu-id="55810-160">可能的值为 `none` `adminGeneratedTemporaryPassword` `userPerformedSecuredPasswordChange` `userPerformedSecuredPasswordReset` `adminConfirmedSigninSafe` `aiConfirmedSigninSafe` 、、、、、、、、、 `userPassedMFADrivenByRiskBasedPolicy` `adminDismissedAllRiskForUser` `adminConfirmedSigninCompromised` `hidden` `adminConfirmedUserCompromised` `unknownFutureValue` 。</span><span class="sxs-lookup"><span data-stu-id="55810-160">The possible values are `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>  |
|<span data-ttu-id="55810-161">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="55810-161">userDisplayName</span></span>|<span data-ttu-id="55810-162">string</span><span class="sxs-lookup"><span data-stu-id="55810-162">string</span></span>|<span data-ttu-id="55810-163">有风险的用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="55810-163">Risky user display name.</span></span>|
|<span data-ttu-id="55810-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="55810-164">userPrincipalName</span></span>|<span data-ttu-id="55810-165">string</span><span class="sxs-lookup"><span data-stu-id="55810-165">string</span></span>|<span data-ttu-id="55810-166">有风险的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="55810-166">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55810-167">关系</span><span class="sxs-lookup"><span data-stu-id="55810-167">Relationships</span></span>

<span data-ttu-id="55810-168">无。</span><span class="sxs-lookup"><span data-stu-id="55810-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55810-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55810-169">JSON representation</span></span>

<span data-ttu-id="55810-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55810-170">The following is a JSON representation of the resource.</span></span>

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
