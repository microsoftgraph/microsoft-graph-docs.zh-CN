---
title: riskyUser 资源类型
description: 有风险的用户项目
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0584a0c1c36428cac735f33eb690821e5d045ae3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896005"
---
# <a name="riskyuser-resource-type"></a><span data-ttu-id="b9623-103">riskyUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9623-103">riskyUser resource type</span></span>

<span data-ttu-id="b9623-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9623-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9623-105">表示有风险的 Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="b9623-105">Represents Azure AD users who are at risk.</span></span> <span data-ttu-id="b9623-106">Azure AD 会根据各种信号和机器学习持续评估用户风险。</span><span class="sxs-lookup"><span data-stu-id="b9623-106">Azure AD continually evaluates user risk based on various signals and machine learning.</span></span> <span data-ttu-id="b9623-107">此 API 提供对 Azure AD 中所有风险用户的编程访问。</span><span class="sxs-lookup"><span data-stu-id="b9623-107">This API provides programmatic access to all at-risk users in your Azure AD.</span></span>

<span data-ttu-id="b9623-108">有关风险事件的详细信息，请参阅[Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/)。</span><span class="sxs-lookup"><span data-stu-id="b9623-108">For more information about risk events, see [Azure Active Directory Identity Protection](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/).</span></span>

><span data-ttu-id="b9623-109">**注意：** 使用 riskyUsers API 需要 Azure AD Premium P2 许可证。</span><span class="sxs-lookup"><span data-stu-id="b9623-109">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="methods"></a><span data-ttu-id="b9623-110">方法</span><span class="sxs-lookup"><span data-stu-id="b9623-110">Methods</span></span>
|<span data-ttu-id="b9623-111">方法</span><span class="sxs-lookup"><span data-stu-id="b9623-111">Method</span></span>|<span data-ttu-id="b9623-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="b9623-112">Return type</span></span>|<span data-ttu-id="b9623-113">说明</span><span class="sxs-lookup"><span data-stu-id="b9623-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b9623-114">列出 riskyUsers</span><span class="sxs-lookup"><span data-stu-id="b9623-114">List riskyUsers</span></span>](../api/riskyuser-list.md)|<span data-ttu-id="b9623-115">[riskyUser](../resources/riskyuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9623-115">[riskyUser](../resources/riskyuser.md) collection</span></span>|<span data-ttu-id="b9623-116">获取**riskyUser**对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="b9623-116">Get a list of the **riskyUser** objects and their properties.</span></span>|
|[<span data-ttu-id="b9623-117">获取 riskyUser</span><span class="sxs-lookup"><span data-stu-id="b9623-117">Get riskyUser</span></span>](../api/riskyuser-get.md)|[<span data-ttu-id="b9623-118">riskyUser</span><span class="sxs-lookup"><span data-stu-id="b9623-118">riskyUser</span></span>](../resources/riskyuser.md)|<span data-ttu-id="b9623-119">读取**riskyUser**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9623-119">Read the properties and relationships of a **riskyUser** object.</span></span>|
|[<span data-ttu-id="b9623-120">消除 riskyUser</span><span class="sxs-lookup"><span data-stu-id="b9623-120">Dismiss a riskyUser</span></span>](../api/riskyuser-dismiss.md)|<span data-ttu-id="b9623-121">无</span><span class="sxs-lookup"><span data-stu-id="b9623-121">None</span></span>|<span data-ttu-id="b9623-122">消除一个或多个**riskyUser**对象的风险。</span><span class="sxs-lookup"><span data-stu-id="b9623-122">Dismiss the risk of one or more **riskyUser** objects.</span></span> |
|[<span data-ttu-id="b9623-123">确认 riskyUser 是否已损坏</span><span class="sxs-lookup"><span data-stu-id="b9623-123">Confirm a riskyUser as compromised</span></span>](../api/riskyuser-confirmcompromised.md)|<span data-ttu-id="b9623-124">无</span><span class="sxs-lookup"><span data-stu-id="b9623-124">None</span></span>|<span data-ttu-id="b9623-125">确认一个或多个**riskyUser**对象已泄露。</span><span class="sxs-lookup"><span data-stu-id="b9623-125">Confirm one or more **riskyUser** objects as compromised.</span></span>|
|[<span data-ttu-id="b9623-126">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="b9623-126">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="b9623-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9623-127">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="b9623-128">从 "历史记录" 导航属性中获取**riskyUserHistoryItems** 。</span><span class="sxs-lookup"><span data-stu-id="b9623-128">Get the **riskyUserHistoryItems** from the history navigation property.</span></span>|
|[<span data-ttu-id="b9623-129">获取历史记录</span><span class="sxs-lookup"><span data-stu-id="b9623-129">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="b9623-130">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="b9623-130">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="b9623-131">读取[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9623-131">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="b9623-132">属性</span><span class="sxs-lookup"><span data-stu-id="b9623-132">Properties</span></span>
|<span data-ttu-id="b9623-133">属性</span><span class="sxs-lookup"><span data-stu-id="b9623-133">Property</span></span>|<span data-ttu-id="b9623-134">类型</span><span class="sxs-lookup"><span data-stu-id="b9623-134">Type</span></span>|<span data-ttu-id="b9623-135">说明</span><span class="sxs-lookup"><span data-stu-id="b9623-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9623-136">id</span><span class="sxs-lookup"><span data-stu-id="b9623-136">id</span></span>|<span data-ttu-id="b9623-137">String</span><span class="sxs-lookup"><span data-stu-id="b9623-137">String</span></span>|<span data-ttu-id="b9623-138">用户存在风险的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b9623-138">Unique ID of the user at risk.</span></span>|
|<span data-ttu-id="b9623-139">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b9623-139">isDeleted</span></span>|<span data-ttu-id="b9623-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9623-140">Boolean</span></span>|<span data-ttu-id="b9623-141">指示是否删除用户。</span><span class="sxs-lookup"><span data-stu-id="b9623-141">Indicates whether the user is deleted.</span></span> <span data-ttu-id="b9623-142">可能的值包括： `true` 、`false`</span><span class="sxs-lookup"><span data-stu-id="b9623-142">Possible values are: `true`, `false`</span></span>|
|<span data-ttu-id="b9623-143">isProcessing</span><span class="sxs-lookup"><span data-stu-id="b9623-143">isProcessing</span></span>|<span data-ttu-id="b9623-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9623-144">Boolean</span></span>|<span data-ttu-id="b9623-145">指示后端正在处理用户的危险状态 wehther</span><span class="sxs-lookup"><span data-stu-id="b9623-145">Indicates wehther a user's risky state is being processed by the backend</span></span>|
|<span data-ttu-id="b9623-146">riskDetail</span><span class="sxs-lookup"><span data-stu-id="b9623-146">riskDetail</span></span>|<span data-ttu-id="b9623-147">riskDetail</span><span class="sxs-lookup"><span data-stu-id="b9623-147">riskDetail</span></span>|<span data-ttu-id="b9623-148">检测到的风险的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b9623-148">Details of the detected risk.</span></span> <span data-ttu-id="b9623-149">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b9623-149">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b9623-150">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9623-150">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="b9623-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9623-151">DateTimeOffset</span></span>|<span data-ttu-id="b9623-152">上次更新有风险的用户的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b9623-152">The date and time that the risky user was last updated.</span></span>|
|<span data-ttu-id="b9623-153">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b9623-153">riskLevel</span></span>|<span data-ttu-id="b9623-154">riskLevel</span><span class="sxs-lookup"><span data-stu-id="b9623-154">riskLevel</span></span>|<span data-ttu-id="b9623-155">检测到的有风险的用户的级别。</span><span class="sxs-lookup"><span data-stu-id="b9623-155">Level of the detected risky user.</span></span> <span data-ttu-id="b9623-156">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b9623-156">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b9623-157">riskState</span><span class="sxs-lookup"><span data-stu-id="b9623-157">riskState</span></span>|<span data-ttu-id="b9623-158">riskState</span><span class="sxs-lookup"><span data-stu-id="b9623-158">riskState</span></span>|<span data-ttu-id="b9623-159">用户风险的状态。</span><span class="sxs-lookup"><span data-stu-id="b9623-159">State of the user's risk.</span></span> <span data-ttu-id="b9623-160">可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b9623-160">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b9623-161">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b9623-161">userDisplayName</span></span>|<span data-ttu-id="b9623-162">String</span><span class="sxs-lookup"><span data-stu-id="b9623-162">String</span></span>|<span data-ttu-id="b9623-163">有风险的用户显示名称。</span><span class="sxs-lookup"><span data-stu-id="b9623-163">Risky user display name.</span></span>|
|<span data-ttu-id="b9623-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9623-164">userPrincipalName</span></span>|<span data-ttu-id="b9623-165">字符串</span><span class="sxs-lookup"><span data-stu-id="b9623-165">String</span></span>|<span data-ttu-id="b9623-166">有风险的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="b9623-166">Risky user principal name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9623-167">关系</span><span class="sxs-lookup"><span data-stu-id="b9623-167">Relationships</span></span>
|<span data-ttu-id="b9623-168">关系</span><span class="sxs-lookup"><span data-stu-id="b9623-168">Relationship</span></span>|<span data-ttu-id="b9623-169">类型</span><span class="sxs-lookup"><span data-stu-id="b9623-169">Type</span></span>|<span data-ttu-id="b9623-170">说明</span><span class="sxs-lookup"><span data-stu-id="b9623-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9623-171">日志</span><span class="sxs-lookup"><span data-stu-id="b9623-171">history</span></span>|<span data-ttu-id="b9623-172">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="b9623-172">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|   <span data-ttu-id="b9623-173">与用户风险级别更改相关的活动</span><span class="sxs-lookup"><span data-stu-id="b9623-173">The activity related to user risk level change</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9623-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9623-174">JSON representation</span></span>
<span data-ttu-id="b9623-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9623-175">The following is a JSON representation of the resource.</span></span>
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

