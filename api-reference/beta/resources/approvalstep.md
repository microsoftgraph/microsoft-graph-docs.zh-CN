---
title: approvalStep 资源类型
description: 与 accessPackageAssignmentRequest 关联的 approvalStep 对象。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 263e809e5858cdc23b34b8401171bb5fce668721
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761252"
---
# <a name="approvalstep-resource-type"></a><span data-ttu-id="b64a6-103">approvalStep 资源类型</span><span class="sxs-lookup"><span data-stu-id="b64a6-103">approvalStep resource type</span></span>

<span data-ttu-id="b64a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b64a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b64a6-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，与 关联的决策的 approvalStep 对象 `accessPackageAssignmentRequest` 。</span><span class="sxs-lookup"><span data-stu-id="b64a6-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approvalStep object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="b64a6-106">它用于区分审批者可以处理审批工作流的不同步骤的决策。</span><span class="sxs-lookup"><span data-stu-id="b64a6-106">It is used to distinguish decisions for different steps of an approval workflow that approvers can act on.</span></span>

## <a name="methods"></a><span data-ttu-id="b64a6-107">方法</span><span class="sxs-lookup"><span data-stu-id="b64a6-107">Methods</span></span>

| <span data-ttu-id="b64a6-108">方法</span><span class="sxs-lookup"><span data-stu-id="b64a6-108">Method</span></span>       | <span data-ttu-id="b64a6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b64a6-109">Return Type</span></span> | <span data-ttu-id="b64a6-110">说明</span><span class="sxs-lookup"><span data-stu-id="b64a6-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="b64a6-111">列出 approvalSteps</span><span class="sxs-lookup"><span data-stu-id="b64a6-111">List approvalSteps</span></span>](../api/approval-list-steps.md) | <span data-ttu-id="b64a6-112">[approvalStep](approvalstep.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b64a6-112">[approvalStep](approvalstep.md) collection</span></span> | <span data-ttu-id="b64a6-113">列出 **与审批对象关联的 approvalStep** **对象。**</span><span class="sxs-lookup"><span data-stu-id="b64a6-113">List the **approvalStep** objects associated with an **approval** object.</span></span> |
|[<span data-ttu-id="b64a6-114">获取审批步骤</span><span class="sxs-lookup"><span data-stu-id="b64a6-114">Get approvalStep</span></span>](../api/approvalstep-get.md) | [<span data-ttu-id="b64a6-115">approvalStep</span><span class="sxs-lookup"><span data-stu-id="b64a6-115">approvalStep</span></span>](approvalstep.md) | <span data-ttu-id="b64a6-116">检索 **approvalStep 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="b64a6-116">Retrieve the properties of an **approvalStep** object.</span></span> |
|[<span data-ttu-id="b64a6-117">更新 approvalStep</span><span class="sxs-lookup"><span data-stu-id="b64a6-117">Update approvalStep</span></span>](../api/approvalstep-update.md) | <span data-ttu-id="b64a6-118">无</span><span class="sxs-lookup"><span data-stu-id="b64a6-118">None</span></span> | <span data-ttu-id="b64a6-119">对 approvalStep 对象应用 **批准或拒绝** 决定。</span><span class="sxs-lookup"><span data-stu-id="b64a6-119">Apply approve or deny decision on an **approvalStep** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b64a6-120">属性</span><span class="sxs-lookup"><span data-stu-id="b64a6-120">Properties</span></span>
|<span data-ttu-id="b64a6-121">属性</span><span class="sxs-lookup"><span data-stu-id="b64a6-121">Property</span></span>|<span data-ttu-id="b64a6-122">类型</span><span class="sxs-lookup"><span data-stu-id="b64a6-122">Type</span></span>|<span data-ttu-id="b64a6-123">说明</span><span class="sxs-lookup"><span data-stu-id="b64a6-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b64a6-124">id</span><span class="sxs-lookup"><span data-stu-id="b64a6-124">id</span></span>|<span data-ttu-id="b64a6-125">String</span><span class="sxs-lookup"><span data-stu-id="b64a6-125">String</span></span>|<span data-ttu-id="b64a6-126">与审批对象关联的步骤的标识符。</span><span class="sxs-lookup"><span data-stu-id="b64a6-126">The identifier of the step associated with an approval object.</span></span> <span data-ttu-id="b64a6-127">只读。</span><span class="sxs-lookup"><span data-stu-id="b64a6-127">Read-only.</span></span>|
|<span data-ttu-id="b64a6-128">displayName</span><span class="sxs-lookup"><span data-stu-id="b64a6-128">displayName</span></span>|<span data-ttu-id="b64a6-129">String</span><span class="sxs-lookup"><span data-stu-id="b64a6-129">String</span></span>|<span data-ttu-id="b64a6-130">策略创建者提供的标签，用于标识审批步骤。</span><span class="sxs-lookup"><span data-stu-id="b64a6-130">The label provided by the policy creator to identify an approval step.</span></span> <span data-ttu-id="b64a6-131">只读</span><span class="sxs-lookup"><span data-stu-id="b64a6-131">Read-only</span></span>|
|<span data-ttu-id="b64a6-132">状态</span><span class="sxs-lookup"><span data-stu-id="b64a6-132">status</span></span>|<span data-ttu-id="b64a6-133">String</span><span class="sxs-lookup"><span data-stu-id="b64a6-133">String</span></span>|<span data-ttu-id="b64a6-134">步骤状态。</span><span class="sxs-lookup"><span data-stu-id="b64a6-134">The step status.</span></span> <span data-ttu-id="b64a6-135">可能的值： `InProgress` 或 `Completed` 。</span><span class="sxs-lookup"><span data-stu-id="b64a6-135">Possible values: `InProgress` or `Completed`.</span></span> <span data-ttu-id="b64a6-136">只读。</span><span class="sxs-lookup"><span data-stu-id="b64a6-136">Read-only.</span></span>|
|<span data-ttu-id="b64a6-137">assignedToMe</span><span class="sxs-lookup"><span data-stu-id="b64a6-137">assignedToMe</span></span>|<span data-ttu-id="b64a6-138">布尔</span><span class="sxs-lookup"><span data-stu-id="b64a6-138">Boolean</span></span>|<span data-ttu-id="b64a6-139">指示是否将步骤分配给呼叫用户进行审阅。</span><span class="sxs-lookup"><span data-stu-id="b64a6-139">Indicates whether the step is assigned to the calling user to review.</span></span> <span data-ttu-id="b64a6-140">只读。</span><span class="sxs-lookup"><span data-stu-id="b64a6-140">Read-only.</span></span>|
|<span data-ttu-id="b64a6-141">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="b64a6-141">reviewedBy</span></span>|<span data-ttu-id="b64a6-142">[userIdentity](useridentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b64a6-142">[userIdentity](useridentity.md) collection</span></span> | <span data-ttu-id="b64a6-143">审阅者的标识符。</span><span class="sxs-lookup"><span data-stu-id="b64a6-143">The identifier of the reviewer.</span></span> <span data-ttu-id="b64a6-144">只读。</span><span class="sxs-lookup"><span data-stu-id="b64a6-144">Read-only.</span></span>|
|<span data-ttu-id="b64a6-145">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="b64a6-145">reviewedDateTime</span></span>|<span data-ttu-id="b64a6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b64a6-146">DateTimeOffset</span></span>|<span data-ttu-id="b64a6-147">记录决策的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b64a6-147">The date and time when a decision was recorded.</span></span> <span data-ttu-id="b64a6-148">只读。</span><span class="sxs-lookup"><span data-stu-id="b64a6-148">Read-only.</span></span>|
|<span data-ttu-id="b64a6-149">reviewResult</span><span class="sxs-lookup"><span data-stu-id="b64a6-149">reviewResult</span></span>|<span data-ttu-id="b64a6-150">String</span><span class="sxs-lookup"><span data-stu-id="b64a6-150">String</span></span>|<span data-ttu-id="b64a6-151">此审批记录的结果。</span><span class="sxs-lookup"><span data-stu-id="b64a6-151">The result of this approval record.</span></span> <span data-ttu-id="b64a6-152">可能的值包括 `NotReviewed` `Approved` `Denied` ：、、。</span><span class="sxs-lookup"><span data-stu-id="b64a6-152">Possible values include: `NotReviewed`, `Approved`, `Denied`.</span></span>|
|<span data-ttu-id="b64a6-153">justification</span><span class="sxs-lookup"><span data-stu-id="b64a6-153">justification</span></span>|<span data-ttu-id="b64a6-154">String</span><span class="sxs-lookup"><span data-stu-id="b64a6-154">String</span></span>|<span data-ttu-id="b64a6-155">与审批步骤决策关联的理由。</span><span class="sxs-lookup"><span data-stu-id="b64a6-155">The justification associated with the approval step decision.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b64a6-156">关系</span><span class="sxs-lookup"><span data-stu-id="b64a6-156">Relationships</span></span>
|<span data-ttu-id="b64a6-157">关系</span><span class="sxs-lookup"><span data-stu-id="b64a6-157">Relationship</span></span>|<span data-ttu-id="b64a6-158">类型</span><span class="sxs-lookup"><span data-stu-id="b64a6-158">Type</span></span>|<span data-ttu-id="b64a6-159">说明</span><span class="sxs-lookup"><span data-stu-id="b64a6-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b64a6-160">审批</span><span class="sxs-lookup"><span data-stu-id="b64a6-160">approval</span></span>|<span data-ttu-id="b64a6-161">[审批](../resources/approval.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b64a6-161">[approval](../resources/approval.md) collection</span></span>|<span data-ttu-id="b64a6-162">与 关联的决策的审批对象 `accessPackageAssignmentRequest` 。</span><span class="sxs-lookup"><span data-stu-id="b64a6-162">The approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b64a6-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b64a6-163">JSON representation</span></span>
<span data-ttu-id="b64a6-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b64a6-164">The following is a JSON representation of the resource.</span></span>
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
