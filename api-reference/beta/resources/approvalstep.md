---
title: approvalStep 资源类型
description: 与 accessPackageAssignmentRequest 或 userConsentRequest 关联的 approvalStep 对象。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 94c37320d17a72e0734d856c24cdff49308c9463
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945709"
---
# <a name="approvalstep-resource-type"></a><span data-ttu-id="b598d-103">approvalStep 资源类型</span><span class="sxs-lookup"><span data-stu-id="b598d-103">approvalStep resource type</span></span>

<span data-ttu-id="b598d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b598d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b598d-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，与 关联的决策的 approvalStep 对象 `accessPackageAssignmentRequest` 。</span><span class="sxs-lookup"><span data-stu-id="b598d-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approvalStep object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="b598d-106">它用于区分审批者可以处理审批工作流的不同步骤的决策。</span><span class="sxs-lookup"><span data-stu-id="b598d-106">It is used to distinguish decisions for different steps of an approval workflow that approvers can act on.</span></span>

<span data-ttu-id="b598d-107">在 [userConsentRequests](../resources/userconsentrequest.md)中，与请求关联的审批决策。</span><span class="sxs-lookup"><span data-stu-id="b598d-107">In [userConsentRequests](../resources/userconsentrequest.md), the approval  decisions associated with a request.</span></span>

## <a name="methods"></a><span data-ttu-id="b598d-108">Methods</span><span class="sxs-lookup"><span data-stu-id="b598d-108">Methods</span></span>

| <span data-ttu-id="b598d-109">方法</span><span class="sxs-lookup"><span data-stu-id="b598d-109">Method</span></span>       | <span data-ttu-id="b598d-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="b598d-110">Return Type</span></span> | <span data-ttu-id="b598d-111">说明</span><span class="sxs-lookup"><span data-stu-id="b598d-111">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="b598d-112">列出 approvalSteps</span><span class="sxs-lookup"><span data-stu-id="b598d-112">List approvalSteps</span></span>](../api/approval-list-steps.md) | <span data-ttu-id="b598d-113">[approvalStep](approvalstep.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b598d-113">[approvalStep](approvalstep.md) collection</span></span> | <span data-ttu-id="b598d-114">列出 **与审批对象关联的 approvalStep** **对象。**</span><span class="sxs-lookup"><span data-stu-id="b598d-114">List the **approvalStep** objects associated with an **approval** object.</span></span> |
|[<span data-ttu-id="b598d-115">获取审批步骤</span><span class="sxs-lookup"><span data-stu-id="b598d-115">Get approvalStep</span></span>](../api/approvalstep-get.md) | [<span data-ttu-id="b598d-116">approvalStep</span><span class="sxs-lookup"><span data-stu-id="b598d-116">approvalStep</span></span>](approvalstep.md) | <span data-ttu-id="b598d-117">检索 **approvalStep 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="b598d-117">Retrieve the properties of an **approvalStep** object.</span></span> |
|[<span data-ttu-id="b598d-118">更新 approvalStep</span><span class="sxs-lookup"><span data-stu-id="b598d-118">Update approvalStep</span></span>](../api/approvalstep-update.md) | <span data-ttu-id="b598d-119">无</span><span class="sxs-lookup"><span data-stu-id="b598d-119">None</span></span> | <span data-ttu-id="b598d-120">对 approvalStep 对象应用 **批准或拒绝** 决定。</span><span class="sxs-lookup"><span data-stu-id="b598d-120">Apply approve or deny decision on an **approvalStep** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b598d-121">属性</span><span class="sxs-lookup"><span data-stu-id="b598d-121">Properties</span></span>
|<span data-ttu-id="b598d-122">属性</span><span class="sxs-lookup"><span data-stu-id="b598d-122">Property</span></span>|<span data-ttu-id="b598d-123">类型</span><span class="sxs-lookup"><span data-stu-id="b598d-123">Type</span></span>|<span data-ttu-id="b598d-124">说明</span><span class="sxs-lookup"><span data-stu-id="b598d-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b598d-125">assignedToMe</span><span class="sxs-lookup"><span data-stu-id="b598d-125">assignedToMe</span></span>|<span data-ttu-id="b598d-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="b598d-126">Boolean</span></span>|<span data-ttu-id="b598d-127">指示是否将步骤分配给呼叫用户进行审阅。</span><span class="sxs-lookup"><span data-stu-id="b598d-127">Indicates whether the step is assigned to the calling user to review.</span></span> <span data-ttu-id="b598d-128">只读。</span><span class="sxs-lookup"><span data-stu-id="b598d-128">Read-only.</span></span>|
|<span data-ttu-id="b598d-129">displayName</span><span class="sxs-lookup"><span data-stu-id="b598d-129">displayName</span></span>|<span data-ttu-id="b598d-130">String</span><span class="sxs-lookup"><span data-stu-id="b598d-130">String</span></span>|<span data-ttu-id="b598d-131">策略创建者提供的标签，用于标识审批步骤。</span><span class="sxs-lookup"><span data-stu-id="b598d-131">The label provided by the policy creator to identify an approval step.</span></span> <span data-ttu-id="b598d-132">只读。</span><span class="sxs-lookup"><span data-stu-id="b598d-132">Read-only.</span></span>|
|<span data-ttu-id="b598d-133">id</span><span class="sxs-lookup"><span data-stu-id="b598d-133">id</span></span>|<span data-ttu-id="b598d-134">String</span><span class="sxs-lookup"><span data-stu-id="b598d-134">String</span></span>|<span data-ttu-id="b598d-135">与审批对象关联的步骤的标识符。</span><span class="sxs-lookup"><span data-stu-id="b598d-135">The identifier of the step associated with an approval object.</span></span> <span data-ttu-id="b598d-136">只读。</span><span class="sxs-lookup"><span data-stu-id="b598d-136">Read-only.</span></span>|
|<span data-ttu-id="b598d-137">justification</span><span class="sxs-lookup"><span data-stu-id="b598d-137">justification</span></span>|<span data-ttu-id="b598d-138">String</span><span class="sxs-lookup"><span data-stu-id="b598d-138">String</span></span>|<span data-ttu-id="b598d-139">与审批步骤决策关联的理由。</span><span class="sxs-lookup"><span data-stu-id="b598d-139">The justification associated with the approval step decision.</span></span>|
|<span data-ttu-id="b598d-140">reviewResult</span><span class="sxs-lookup"><span data-stu-id="b598d-140">reviewResult</span></span>|<span data-ttu-id="b598d-141">String</span><span class="sxs-lookup"><span data-stu-id="b598d-141">String</span></span>|<span data-ttu-id="b598d-142">此审批记录的结果。</span><span class="sxs-lookup"><span data-stu-id="b598d-142">The result of this approval record.</span></span> <span data-ttu-id="b598d-143">可能的值包括 `NotReviewed` `Approved` `Denied` ：、、。</span><span class="sxs-lookup"><span data-stu-id="b598d-143">Possible values include: `NotReviewed`, `Approved`, `Denied`.</span></span>|
|<span data-ttu-id="b598d-144">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="b598d-144">reviewedBy</span></span>|<span data-ttu-id="b598d-145">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b598d-145">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="b598d-146">审阅者的标识符。</span><span class="sxs-lookup"><span data-stu-id="b598d-146">The identifier of the reviewer.</span></span> <span data-ttu-id="b598d-147">只读。</span><span class="sxs-lookup"><span data-stu-id="b598d-147">Read-only.</span></span>|
|<span data-ttu-id="b598d-148">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="b598d-148">reviewedDateTime</span></span>|<span data-ttu-id="b598d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b598d-149">DateTimeOffset</span></span>|<span data-ttu-id="b598d-150">记录决策的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b598d-150">The date and time when a decision was recorded.</span></span> <span data-ttu-id="b598d-151">日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b598d-151">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b598d-152">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="b598d-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="b598d-153">只读。</span><span class="sxs-lookup"><span data-stu-id="b598d-153">Read-only.</span></span>|
|<span data-ttu-id="b598d-154">状态</span><span class="sxs-lookup"><span data-stu-id="b598d-154">status</span></span>|<span data-ttu-id="b598d-155">String</span><span class="sxs-lookup"><span data-stu-id="b598d-155">String</span></span>|<span data-ttu-id="b598d-156">步骤状态。</span><span class="sxs-lookup"><span data-stu-id="b598d-156">The step status.</span></span> <span data-ttu-id="b598d-157">可能的值 `InProgress` `Initializing` `Completed` ：、、、。 `Expired`</span><span class="sxs-lookup"><span data-stu-id="b598d-157">Possible values: `InProgress`, `Initializing`, `Completed`, `Expired`.</span></span> <span data-ttu-id="b598d-158">只读。</span><span class="sxs-lookup"><span data-stu-id="b598d-158">Read-only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b598d-159">关系</span><span class="sxs-lookup"><span data-stu-id="b598d-159">Relationships</span></span>
|<span data-ttu-id="b598d-160">关系</span><span class="sxs-lookup"><span data-stu-id="b598d-160">Relationship</span></span>|<span data-ttu-id="b598d-161">类型</span><span class="sxs-lookup"><span data-stu-id="b598d-161">Type</span></span>|<span data-ttu-id="b598d-162">说明</span><span class="sxs-lookup"><span data-stu-id="b598d-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b598d-163">审批</span><span class="sxs-lookup"><span data-stu-id="b598d-163">approval</span></span>|<span data-ttu-id="b598d-164">[审批](../resources/approval.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b598d-164">[approval](../resources/approval.md) collection</span></span>|<span data-ttu-id="b598d-165">与 关联的决策的审批对象 `accessPackageAssignmentRequest` 。</span><span class="sxs-lookup"><span data-stu-id="b598d-165">The approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b598d-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b598d-166">JSON representation</span></span>
<span data-ttu-id="b598d-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b598d-167">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStep",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approvalStep",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": true,
  "reviewedBy": [{"@odata.type": "microsoft.graph.userIdentity"}],
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String",
}
```
