---
title: riskyUserHistoryItem 资源类型
description: 有风险的用户历史记录项
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4bcf9e1834e8fff48a148095ffe7ddbd459ee23e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895998"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="af127-103">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="af127-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="af127-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af127-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af127-105">表示 azure AD 用户的风险历史记录，由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="af127-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span>


<span data-ttu-id="af127-106">继承自[riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="af127-106">Inherits from [riskyUser](../resources/riskyuser.md).</span></span>

## <a name="methods"></a><span data-ttu-id="af127-107">方法</span><span class="sxs-lookup"><span data-stu-id="af127-107">Methods</span></span>
|<span data-ttu-id="af127-108">方法</span><span class="sxs-lookup"><span data-stu-id="af127-108">Method</span></span>|<span data-ttu-id="af127-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="af127-109">Return type</span></span>|<span data-ttu-id="af127-110">说明</span><span class="sxs-lookup"><span data-stu-id="af127-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af127-111">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="af127-111">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="af127-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="af127-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="af127-113">从 "历史记录" 导航属性中获取 riskyUserHistoryItems。</span><span class="sxs-lookup"><span data-stu-id="af127-113">Get the riskyUserHistoryItems from the history navigation property.</span></span>|
|[<span data-ttu-id="af127-114">获取历史记录</span><span class="sxs-lookup"><span data-stu-id="af127-114">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="af127-115">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="af127-115">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="af127-116">读取[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="af127-116">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af127-117">属性</span><span class="sxs-lookup"><span data-stu-id="af127-117">Properties</span></span>
|<span data-ttu-id="af127-118">属性</span><span class="sxs-lookup"><span data-stu-id="af127-118">Property</span></span>|<span data-ttu-id="af127-119">类型</span><span class="sxs-lookup"><span data-stu-id="af127-119">Type</span></span>|<span data-ttu-id="af127-120">说明</span><span class="sxs-lookup"><span data-stu-id="af127-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af127-121">activity</span><span class="sxs-lookup"><span data-stu-id="af127-121">activity</span></span>|[<span data-ttu-id="af127-122">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="af127-122">riskUserActivity</span></span>](../resources/riskuseractivity.md)|<span data-ttu-id="af127-123">与用户风险级别更改相关的活动。</span><span class="sxs-lookup"><span data-stu-id="af127-123">The activity related to user risk level change.</span></span>|
|<span data-ttu-id="af127-124">id</span><span class="sxs-lookup"><span data-stu-id="af127-124">id</span></span>|<span data-ttu-id="af127-125">String</span><span class="sxs-lookup"><span data-stu-id="af127-125">String</span></span>|<span data-ttu-id="af127-126">继承自[entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="af127-126">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="af127-127">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="af127-127">initiatedBy</span></span>|<span data-ttu-id="af127-128">String</span><span class="sxs-lookup"><span data-stu-id="af127-128">String</span></span>|<span data-ttu-id="af127-129">执行此操作的主角的 id。</span><span class="sxs-lookup"><span data-stu-id="af127-129">The id of actor that does the operation.</span></span>|
|<span data-ttu-id="af127-130">isDeleted</span><span class="sxs-lookup"><span data-stu-id="af127-130">isDeleted</span></span>|<span data-ttu-id="af127-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="af127-131">Boolean</span></span>| <span data-ttu-id="af127-132">继承自[riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="af127-132">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="af127-133">isProcessing</span><span class="sxs-lookup"><span data-stu-id="af127-133">isProcessing</span></span>|<span data-ttu-id="af127-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="af127-134">Boolean</span></span>| <span data-ttu-id="af127-135">继承自[riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="af127-135">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="af127-136">riskDetail</span><span class="sxs-lookup"><span data-stu-id="af127-136">riskDetail</span></span>|<span data-ttu-id="af127-137">riskDetail</span><span class="sxs-lookup"><span data-stu-id="af127-137">riskDetail</span></span>|<span data-ttu-id="af127-138">继承自[riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="af127-138">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="af127-139">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="af127-139">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="af127-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="af127-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="af127-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af127-141">DateTimeOffset</span></span>|<span data-ttu-id="af127-142">继承自[riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="af127-142">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="af127-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="af127-143">riskLevel</span></span>|<span data-ttu-id="af127-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="af127-144">riskLevel</span></span>|<span data-ttu-id="af127-145">继承自[riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="af127-145">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="af127-146">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="af127-146">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="af127-147">riskState</span><span class="sxs-lookup"><span data-stu-id="af127-147">riskState</span></span>|<span data-ttu-id="af127-148">riskState</span><span class="sxs-lookup"><span data-stu-id="af127-148">riskState</span></span>|<span data-ttu-id="af127-149">继承自[riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="af127-149">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="af127-150">可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="af127-150">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="af127-151">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="af127-151">userDisplayName</span></span>|<span data-ttu-id="af127-152">String</span><span class="sxs-lookup"><span data-stu-id="af127-152">String</span></span>|<span data-ttu-id="af127-153">继承自[riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="af127-153">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="af127-154">userId</span><span class="sxs-lookup"><span data-stu-id="af127-154">userId</span></span>|<span data-ttu-id="af127-155">String</span><span class="sxs-lookup"><span data-stu-id="af127-155">String</span></span>|<span data-ttu-id="af127-156">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="af127-156">The id of the user.</span></span>|
|<span data-ttu-id="af127-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af127-157">userPrincipalName</span></span>|<span data-ttu-id="af127-158">字符串</span><span class="sxs-lookup"><span data-stu-id="af127-158">String</span></span>|<span data-ttu-id="af127-159">有风险的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="af127-159">Risky user principal name.</span></span> <span data-ttu-id="af127-160">继承自[riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="af127-160">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="af127-161">关系</span><span class="sxs-lookup"><span data-stu-id="af127-161">Relationships</span></span>
|<span data-ttu-id="af127-162">关系</span><span class="sxs-lookup"><span data-stu-id="af127-162">Relationship</span></span>|<span data-ttu-id="af127-163">类型</span><span class="sxs-lookup"><span data-stu-id="af127-163">Type</span></span>|<span data-ttu-id="af127-164">说明</span><span class="sxs-lookup"><span data-stu-id="af127-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af127-165">日志</span><span class="sxs-lookup"><span data-stu-id="af127-165">history</span></span>|<span data-ttu-id="af127-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="af127-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>| <span data-ttu-id="af127-167">继承自[riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="af127-167">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af127-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af127-168">JSON representation</span></span>
<span data-ttu-id="af127-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af127-169">The following is a JSON representation of the resource.</span></span>
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

