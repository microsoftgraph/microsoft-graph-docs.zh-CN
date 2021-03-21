---
title: riskyUser 资源类型
description: 有风险的用户项
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 82b622838ddd5e7fb8c00a969184bdd729926b23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961081"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="beb14-103">riskyUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="beb14-103">riskyUser resource type</span></span>

<span data-ttu-id="beb14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beb14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="beb14-105">表示处于风险中的 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="beb14-105">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="beb14-106">Azure AD 根据各种信号和机器学习持续评估用户风险。</span><span class="sxs-lookup"><span data-stu-id="beb14-106">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="beb14-107">此 API 为 Azure AD 中所有处于风险中的用户提供编程访问权限。</span><span class="sxs-lookup"><span data-stu-id="beb14-107">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="beb14-108">有关风险事件详细信息，请参阅 Azure [Active Directory Identity Protection。](/azure/active-directory/identity-protection/overview-identity-protection)</span><span class="sxs-lookup"><span data-stu-id="beb14-108">For more information about risk events, see [Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection).</span></span>

><span data-ttu-id="beb14-109">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="beb14-109">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="beb14-110">Methods</span><span class="sxs-lookup"><span data-stu-id="beb14-110">Methods</span></span>
|<span data-ttu-id="beb14-111">方法</span><span class="sxs-lookup"><span data-stu-id="beb14-111">Method</span></span>|<span data-ttu-id="beb14-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="beb14-112">Return type</span></span>|<span data-ttu-id="beb14-113">说明</span><span class="sxs-lookup"><span data-stu-id="beb14-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="beb14-114">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="beb14-114">List riskyUsers</span></span>](../api/riskyuser-list.md)|<span data-ttu-id="beb14-115">[riskyUser](../resources/riskyuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="beb14-115">[riskyUser](../resources/riskyuser.md) collection</span></span>|<span data-ttu-id="beb14-116">获取 **riskyUser** 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="beb14-116">Get a list of the **riskyUser** objects and their properties.</span></span>|
|[<span data-ttu-id="beb14-117">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="beb14-117">Get riskyUser</span></span>](../api/riskyuser-get.md)|[<span data-ttu-id="beb14-118">riskyUser</span><span class="sxs-lookup"><span data-stu-id="beb14-118">riskyUser</span></span>](../resources/riskyuser.md)|<span data-ttu-id="beb14-119">读取 **riskyUser** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="beb14-119">Read the properties and relationships of a **riskyUser** object.</span></span>|
|[<span data-ttu-id="beb14-120">消除 riskyUser</span><span class="sxs-lookup"><span data-stu-id="beb14-120">Dismiss a riskyUser</span></span>](../api/riskyuser-dismiss.md)|<span data-ttu-id="beb14-121">无</span><span class="sxs-lookup"><span data-stu-id="beb14-121">None</span></span>|<span data-ttu-id="beb14-122">消除一个或多个 **riskyUser 对象** 的风险。</span><span class="sxs-lookup"><span data-stu-id="beb14-122">Dismiss the risk of one or more **riskyUser** objects.</span></span> |
|[<span data-ttu-id="beb14-123">确认存在已泄露的 riskyUser</span><span class="sxs-lookup"><span data-stu-id="beb14-123">Confirm a riskyUser as compromised</span></span>](../api/riskyuser-confirmcompromised.md)|<span data-ttu-id="beb14-124">无</span><span class="sxs-lookup"><span data-stu-id="beb14-124">None</span></span>|<span data-ttu-id="beb14-125">确认一个或多个 **riskyUser** 对象受到威胁。</span><span class="sxs-lookup"><span data-stu-id="beb14-125">Confirm one or more **riskyUser** objects as compromised.</span></span>|
|[<span data-ttu-id="beb14-126">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="beb14-126">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="beb14-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="beb14-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="beb14-128">从 **历史记录导航属性获取 riskyUserHistoryItems。**</span><span class="sxs-lookup"><span data-stu-id="beb14-128">Get the **riskyUserHistoryItems** from the history navigation property.</span></span>|
|[<span data-ttu-id="beb14-129">获取历史记录</span><span class="sxs-lookup"><span data-stu-id="beb14-129">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="beb14-130">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="beb14-130">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="beb14-131">读取 [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="beb14-131">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="beb14-132">属性</span><span class="sxs-lookup"><span data-stu-id="beb14-132">Properties</span></span>
|<span data-ttu-id="beb14-133">属性</span><span class="sxs-lookup"><span data-stu-id="beb14-133">Property</span></span>|<span data-ttu-id="beb14-134">类型</span><span class="sxs-lookup"><span data-stu-id="beb14-134">Type</span></span>|<span data-ttu-id="beb14-135">说明</span><span class="sxs-lookup"><span data-stu-id="beb14-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb14-136">id</span><span class="sxs-lookup"><span data-stu-id="beb14-136">id</span></span>|<span data-ttu-id="beb14-137">String</span><span class="sxs-lookup"><span data-stu-id="beb14-137">String</span></span>|<span data-ttu-id="beb14-138">处于风险中的用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="beb14-138">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="beb14-139">isDeleted</span><span class="sxs-lookup"><span data-stu-id="beb14-139">isDeleted</span></span>|<span data-ttu-id="beb14-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="beb14-140">Boolean</span></span>|<span data-ttu-id="beb14-141">指示用户是否被删除。</span><span class="sxs-lookup"><span data-stu-id="beb14-141">Indicates whether the user is deleted.</span></span> <span data-ttu-id="beb14-142">可取值为：`true`、`false`。</span><span class="sxs-lookup"><span data-stu-id="beb14-142">Possible values are: `true`, `false`.</span></span>|
|<span data-ttu-id="beb14-143">isProcessing</span><span class="sxs-lookup"><span data-stu-id="beb14-143">isProcessing</span></span>|<span data-ttu-id="beb14-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="beb14-144">Boolean</span></span>|<span data-ttu-id="beb14-145">指示后端是否正在处理用户的风险状态。</span><span class="sxs-lookup"><span data-stu-id="beb14-145">Indicates whether a user's risky state is being processed by the backend.</span></span>|
|<span data-ttu-id="beb14-146">riskDetail</span><span class="sxs-lookup"><span data-stu-id="beb14-146">riskDetail</span></span>|<span data-ttu-id="beb14-147">riskDetail</span><span class="sxs-lookup"><span data-stu-id="beb14-147">riskDetail</span></span>|<span data-ttu-id="beb14-148">检测到的风险的详细信息。</span><span class="sxs-lookup"><span data-stu-id="beb14-148">Details of the detected risk.</span></span> <span data-ttu-id="beb14-149">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="beb14-149">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="beb14-150">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="beb14-150">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="beb14-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="beb14-151">DateTimeOffset</span></span>|<span data-ttu-id="beb14-152">上次更新有风险用户的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="beb14-152">The date and time that the risky user was last updated.</span></span>  <span data-ttu-id="beb14-153">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="beb14-153">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="beb14-154">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="beb14-154">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="beb14-155">riskLevel</span><span class="sxs-lookup"><span data-stu-id="beb14-155">riskLevel</span></span>|<span data-ttu-id="beb14-156">riskLevel</span><span class="sxs-lookup"><span data-stu-id="beb14-156">riskLevel</span></span>|<span data-ttu-id="beb14-157">检测到的风险用户级别。</span><span class="sxs-lookup"><span data-stu-id="beb14-157">Level of the detected risky user.</span></span> <span data-ttu-id="beb14-158">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="beb14-158">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="beb14-159">riskState</span><span class="sxs-lookup"><span data-stu-id="beb14-159">riskState</span></span>|<span data-ttu-id="beb14-160">riskState</span><span class="sxs-lookup"><span data-stu-id="beb14-160">riskState</span></span>|<span data-ttu-id="beb14-161">用户风险的状态。</span><span class="sxs-lookup"><span data-stu-id="beb14-161">State of the user's risk.</span></span> <span data-ttu-id="beb14-162">可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="beb14-162">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="beb14-163">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="beb14-163">userDisplayName</span></span>|<span data-ttu-id="beb14-164">String</span><span class="sxs-lookup"><span data-stu-id="beb14-164">String</span></span>|<span data-ttu-id="beb14-165">有风险的用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="beb14-165">Risky user display name.</span></span>|
|<span data-ttu-id="beb14-166">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="beb14-166">userPrincipalName</span></span>|<span data-ttu-id="beb14-167">String</span><span class="sxs-lookup"><span data-stu-id="beb14-167">String</span></span>|<span data-ttu-id="beb14-168">有风险的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="beb14-168">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="beb14-169">关系</span><span class="sxs-lookup"><span data-stu-id="beb14-169">Relationships</span></span>
|<span data-ttu-id="beb14-170">关系</span><span class="sxs-lookup"><span data-stu-id="beb14-170">Relationship</span></span>|<span data-ttu-id="beb14-171">类型</span><span class="sxs-lookup"><span data-stu-id="beb14-171">Type</span></span>|<span data-ttu-id="beb14-172">说明</span><span class="sxs-lookup"><span data-stu-id="beb14-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="beb14-173">history</span><span class="sxs-lookup"><span data-stu-id="beb14-173">history</span></span>|<span data-ttu-id="beb14-174">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="beb14-174">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|   <span data-ttu-id="beb14-175">与用户风险级别更改相关的活动</span><span class="sxs-lookup"><span data-stu-id="beb14-175">The activity related to user risk level change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="beb14-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="beb14-176">JSON representation</span></span>
<span data-ttu-id="beb14-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="beb14-177">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUser",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String"
}
```
