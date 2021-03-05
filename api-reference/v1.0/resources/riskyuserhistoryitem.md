---
title: riskyUserHistoryItem 资源类型
description: 有风险的用户历史记录项
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2188a3a13d36a6d224b3c8ca2a7ac297c22712ce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443886"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="e5864-103">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5864-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="e5864-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5864-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5864-105">表示 Azure AD 用户的风险历史记录，由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="e5864-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span>


<span data-ttu-id="e5864-106">继承自 [riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="e5864-106">Inherits from [riskyUser](../resources/riskyuser.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e5864-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e5864-107">Methods</span></span>
|<span data-ttu-id="e5864-108">方法</span><span class="sxs-lookup"><span data-stu-id="e5864-108">Method</span></span>|<span data-ttu-id="e5864-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5864-109">Return type</span></span>|<span data-ttu-id="e5864-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5864-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5864-111">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="e5864-111">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="e5864-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5864-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="e5864-113">从历史记录导航属性获取 riskyUserHistoryItems。</span><span class="sxs-lookup"><span data-stu-id="e5864-113">Get the riskyUserHistoryItems from the history navigation property.</span></span>|
|[<span data-ttu-id="e5864-114">获取历史记录</span><span class="sxs-lookup"><span data-stu-id="e5864-114">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="e5864-115">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="e5864-115">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="e5864-116">读取 [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e5864-116">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5864-117">属性</span><span class="sxs-lookup"><span data-stu-id="e5864-117">Properties</span></span>
|<span data-ttu-id="e5864-118">属性</span><span class="sxs-lookup"><span data-stu-id="e5864-118">Property</span></span>|<span data-ttu-id="e5864-119">类型</span><span class="sxs-lookup"><span data-stu-id="e5864-119">Type</span></span>|<span data-ttu-id="e5864-120">说明</span><span class="sxs-lookup"><span data-stu-id="e5864-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5864-121">活动</span><span class="sxs-lookup"><span data-stu-id="e5864-121">activity</span></span>|[<span data-ttu-id="e5864-122">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="e5864-122">riskUserActivity</span></span>](../resources/riskuseractivity.md)|<span data-ttu-id="e5864-123">与用户风险级别相关的活动更改。</span><span class="sxs-lookup"><span data-stu-id="e5864-123">The activity related to user risk level change.</span></span>|
|<span data-ttu-id="e5864-124">id</span><span class="sxs-lookup"><span data-stu-id="e5864-124">id</span></span>|<span data-ttu-id="e5864-125">String</span><span class="sxs-lookup"><span data-stu-id="e5864-125">String</span></span>|<span data-ttu-id="e5864-126">继承自 [实体](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="e5864-126">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="e5864-127">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="e5864-127">initiatedBy</span></span>|<span data-ttu-id="e5864-128">String</span><span class="sxs-lookup"><span data-stu-id="e5864-128">String</span></span>|<span data-ttu-id="e5864-129">执行该操作的主角的 ID。</span><span class="sxs-lookup"><span data-stu-id="e5864-129">The id of actor that does the operation.</span></span>|
|<span data-ttu-id="e5864-130">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e5864-130">isDeleted</span></span>|<span data-ttu-id="e5864-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5864-131">Boolean</span></span>| <span data-ttu-id="e5864-132">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="e5864-132">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="e5864-133">isProcessing</span><span class="sxs-lookup"><span data-stu-id="e5864-133">isProcessing</span></span>|<span data-ttu-id="e5864-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5864-134">Boolean</span></span>| <span data-ttu-id="e5864-135">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="e5864-135">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="e5864-136">riskDetail</span><span class="sxs-lookup"><span data-stu-id="e5864-136">riskDetail</span></span>|<span data-ttu-id="e5864-137">riskDetail</span><span class="sxs-lookup"><span data-stu-id="e5864-137">riskDetail</span></span>|<span data-ttu-id="e5864-138">继承自 [riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="e5864-138">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="e5864-139">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e5864-139">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e5864-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5864-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="e5864-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5864-141">DateTimeOffset</span></span>|<span data-ttu-id="e5864-142">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="e5864-142">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="e5864-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e5864-143">riskLevel</span></span>|<span data-ttu-id="e5864-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e5864-144">riskLevel</span></span>|<span data-ttu-id="e5864-145">继承自 [riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="e5864-145">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="e5864-146">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e5864-146">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e5864-147">riskState</span><span class="sxs-lookup"><span data-stu-id="e5864-147">riskState</span></span>|<span data-ttu-id="e5864-148">riskState</span><span class="sxs-lookup"><span data-stu-id="e5864-148">riskState</span></span>|<span data-ttu-id="e5864-149">继承自 [riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="e5864-149">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="e5864-150">可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e5864-150">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e5864-151">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e5864-151">userDisplayName</span></span>|<span data-ttu-id="e5864-152">String</span><span class="sxs-lookup"><span data-stu-id="e5864-152">String</span></span>|<span data-ttu-id="e5864-153">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="e5864-153">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="e5864-154">userId</span><span class="sxs-lookup"><span data-stu-id="e5864-154">userId</span></span>|<span data-ttu-id="e5864-155">String</span><span class="sxs-lookup"><span data-stu-id="e5864-155">String</span></span>|<span data-ttu-id="e5864-156">用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="e5864-156">The id of the user.</span></span>|
|<span data-ttu-id="e5864-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e5864-157">userPrincipalName</span></span>|<span data-ttu-id="e5864-158">String</span><span class="sxs-lookup"><span data-stu-id="e5864-158">String</span></span>|<span data-ttu-id="e5864-159">有风险的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="e5864-159">Risky user principal name.</span></span> <span data-ttu-id="e5864-160">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="e5864-160">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5864-161">关系</span><span class="sxs-lookup"><span data-stu-id="e5864-161">Relationships</span></span>
|<span data-ttu-id="e5864-162">关系</span><span class="sxs-lookup"><span data-stu-id="e5864-162">Relationship</span></span>|<span data-ttu-id="e5864-163">类型</span><span class="sxs-lookup"><span data-stu-id="e5864-163">Type</span></span>|<span data-ttu-id="e5864-164">说明</span><span class="sxs-lookup"><span data-stu-id="e5864-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5864-165">历史记录</span><span class="sxs-lookup"><span data-stu-id="e5864-165">history</span></span>|<span data-ttu-id="e5864-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5864-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>| <span data-ttu-id="e5864-167">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="e5864-167">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5864-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5864-168">JSON representation</span></span>
<span data-ttu-id="e5864-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5864-169">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "String (identifier)",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "riskDetail": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "userId": "String",
  "initiatedBy": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  }
}
```


