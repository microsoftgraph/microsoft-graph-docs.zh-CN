---
title: riskyUserHistoryItem 资源类型
description: 有风险的用户历史记录项
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 551f008696b3c9507f1cae414c34de5a8779ab24
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984157"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="7df0e-103">riskyUserHistoryItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="7df0e-103">riskyUserHistoryItem resource type</span></span>

<span data-ttu-id="7df0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7df0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7df0e-105">表示 azure AD 用户的风险历史记录，由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="7df0e-105">Represents the risk history of an Azure AD user as determined by Azure AD Identity Protection.</span></span>


<span data-ttu-id="7df0e-106">继承自 [riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="7df0e-106">Inherits from [riskyUser](../resources/riskyuser.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7df0e-107">方法</span><span class="sxs-lookup"><span data-stu-id="7df0e-107">Methods</span></span>
|<span data-ttu-id="7df0e-108">方法</span><span class="sxs-lookup"><span data-stu-id="7df0e-108">Method</span></span>|<span data-ttu-id="7df0e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7df0e-109">Return type</span></span>|<span data-ttu-id="7df0e-110">说明</span><span class="sxs-lookup"><span data-stu-id="7df0e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7df0e-111">列表历史记录</span><span class="sxs-lookup"><span data-stu-id="7df0e-111">List history</span></span>](../api/riskyuser-list-history.md)|<span data-ttu-id="7df0e-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7df0e-112">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>|<span data-ttu-id="7df0e-113">从 "历史记录" 导航属性中获取 riskyUserHistoryItems。</span><span class="sxs-lookup"><span data-stu-id="7df0e-113">Get the riskyUserHistoryItems from the history navigation property.</span></span>|
|[<span data-ttu-id="7df0e-114">获取历史记录</span><span class="sxs-lookup"><span data-stu-id="7df0e-114">Get history</span></span>](../api/riskyuser-get-riskyuserhistoryitem.md)|[<span data-ttu-id="7df0e-115">riskyUserHistoryItem</span><span class="sxs-lookup"><span data-stu-id="7df0e-115">riskyUserHistoryItem</span></span>](../resources/riskyuserhistoryitem.md)|<span data-ttu-id="7df0e-116">读取 [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7df0e-116">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7df0e-117">属性</span><span class="sxs-lookup"><span data-stu-id="7df0e-117">Properties</span></span>
|<span data-ttu-id="7df0e-118">属性</span><span class="sxs-lookup"><span data-stu-id="7df0e-118">Property</span></span>|<span data-ttu-id="7df0e-119">类型</span><span class="sxs-lookup"><span data-stu-id="7df0e-119">Type</span></span>|<span data-ttu-id="7df0e-120">说明</span><span class="sxs-lookup"><span data-stu-id="7df0e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df0e-121">activity</span><span class="sxs-lookup"><span data-stu-id="7df0e-121">activity</span></span>|[<span data-ttu-id="7df0e-122">riskUserActivity</span><span class="sxs-lookup"><span data-stu-id="7df0e-122">riskUserActivity</span></span>](../resources/riskuseractivity.md)|<span data-ttu-id="7df0e-123">与用户风险级别更改相关的活动。</span><span class="sxs-lookup"><span data-stu-id="7df0e-123">The activity related to user risk level change.</span></span>|
|<span data-ttu-id="7df0e-124">id</span><span class="sxs-lookup"><span data-stu-id="7df0e-124">id</span></span>|<span data-ttu-id="7df0e-125">String</span><span class="sxs-lookup"><span data-stu-id="7df0e-125">String</span></span>|<span data-ttu-id="7df0e-126">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="7df0e-126">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="7df0e-127">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="7df0e-127">initiatedBy</span></span>|<span data-ttu-id="7df0e-128">String</span><span class="sxs-lookup"><span data-stu-id="7df0e-128">String</span></span>|<span data-ttu-id="7df0e-129">执行此操作的主角的 id。</span><span class="sxs-lookup"><span data-stu-id="7df0e-129">The id of actor that does the operation.</span></span>|
|<span data-ttu-id="7df0e-130">isDeleted</span><span class="sxs-lookup"><span data-stu-id="7df0e-130">isDeleted</span></span>|<span data-ttu-id="7df0e-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df0e-131">Boolean</span></span>| <span data-ttu-id="7df0e-132">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7df0e-132">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="7df0e-133">isProcessing</span><span class="sxs-lookup"><span data-stu-id="7df0e-133">isProcessing</span></span>|<span data-ttu-id="7df0e-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="7df0e-134">Boolean</span></span>| <span data-ttu-id="7df0e-135">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7df0e-135">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="7df0e-136">riskDetail</span><span class="sxs-lookup"><span data-stu-id="7df0e-136">riskDetail</span></span>|<span data-ttu-id="7df0e-137">riskDetail</span><span class="sxs-lookup"><span data-stu-id="7df0e-137">riskDetail</span></span>|<span data-ttu-id="7df0e-138">继承自 [riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="7df0e-138">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="7df0e-139">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7df0e-139">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7df0e-140">riskLastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7df0e-140">riskLastUpdatedDateTime</span></span>|<span data-ttu-id="7df0e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7df0e-141">DateTimeOffset</span></span>|<span data-ttu-id="7df0e-142">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7df0e-142">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="7df0e-143">riskLevel</span><span class="sxs-lookup"><span data-stu-id="7df0e-143">riskLevel</span></span>|<span data-ttu-id="7df0e-144">riskLevel</span><span class="sxs-lookup"><span data-stu-id="7df0e-144">riskLevel</span></span>|<span data-ttu-id="7df0e-145">继承自 [riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="7df0e-145">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="7df0e-146">可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7df0e-146">Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7df0e-147">riskState</span><span class="sxs-lookup"><span data-stu-id="7df0e-147">riskState</span></span>|<span data-ttu-id="7df0e-148">riskState</span><span class="sxs-lookup"><span data-stu-id="7df0e-148">riskState</span></span>|<span data-ttu-id="7df0e-149">继承自 [riskyUser](../resources/riskyuser.md)。</span><span class="sxs-lookup"><span data-stu-id="7df0e-149">Inherited from [riskyUser](../resources/riskyuser.md).</span></span> <span data-ttu-id="7df0e-150">可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7df0e-150">Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7df0e-151">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7df0e-151">userDisplayName</span></span>|<span data-ttu-id="7df0e-152">String</span><span class="sxs-lookup"><span data-stu-id="7df0e-152">String</span></span>|<span data-ttu-id="7df0e-153">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7df0e-153">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|
|<span data-ttu-id="7df0e-154">userId</span><span class="sxs-lookup"><span data-stu-id="7df0e-154">userId</span></span>|<span data-ttu-id="7df0e-155">String</span><span class="sxs-lookup"><span data-stu-id="7df0e-155">String</span></span>|<span data-ttu-id="7df0e-156">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="7df0e-156">The id of the user.</span></span>|
|<span data-ttu-id="7df0e-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7df0e-157">userPrincipalName</span></span>|<span data-ttu-id="7df0e-158">String</span><span class="sxs-lookup"><span data-stu-id="7df0e-158">String</span></span>|<span data-ttu-id="7df0e-159">有风险的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="7df0e-159">Risky user principal name.</span></span> <span data-ttu-id="7df0e-160">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7df0e-160">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7df0e-161">关系</span><span class="sxs-lookup"><span data-stu-id="7df0e-161">Relationships</span></span>
|<span data-ttu-id="7df0e-162">关系</span><span class="sxs-lookup"><span data-stu-id="7df0e-162">Relationship</span></span>|<span data-ttu-id="7df0e-163">类型</span><span class="sxs-lookup"><span data-stu-id="7df0e-163">Type</span></span>|<span data-ttu-id="7df0e-164">说明</span><span class="sxs-lookup"><span data-stu-id="7df0e-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df0e-165">日志</span><span class="sxs-lookup"><span data-stu-id="7df0e-165">history</span></span>|<span data-ttu-id="7df0e-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7df0e-166">[riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) collection</span></span>| <span data-ttu-id="7df0e-167">继承自 [riskyUser](../resources/riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7df0e-167">Inherited from [riskyUser](../resources/riskyuser.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7df0e-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7df0e-168">JSON representation</span></span>
<span data-ttu-id="7df0e-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7df0e-169">The following is a JSON representation of the resource.</span></span>
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


