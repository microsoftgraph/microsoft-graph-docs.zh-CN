---
title: 审批资源类型
description: 与 accessPackageAssignmentRequest 或 userConsentRequest 关联的审批对象。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 6f6751807f0dcb042958104c4b3146a555b22189
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945716"
---
# <a name="approval-resource-type"></a><span data-ttu-id="1102d-103">审批资源类型</span><span class="sxs-lookup"><span data-stu-id="1102d-103">approval resource type</span></span>

<span data-ttu-id="1102d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1102d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1102d-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，与 关联的决策的审批对象 `accessPackageAssignmentRequest` 。</span><span class="sxs-lookup"><span data-stu-id="1102d-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="1102d-106">单个步骤请求可以有一个与它关联的步骤，审批者可以处理该步骤。</span><span class="sxs-lookup"><span data-stu-id="1102d-106">A single step request can have one step associated with it which approvers can act on.</span></span> <span data-ttu-id="1102d-107">同样，多步骤请求可以有多个与之关联的步骤，审批者可以执行这些步骤。</span><span class="sxs-lookup"><span data-stu-id="1102d-107">Similarly, a multi-step request can have multiple steps associated with it which approvers can act on.</span></span> <span data-ttu-id="1102d-108">但是，在多步骤审批中，将显示挂起的步骤和之前完成的步骤。</span><span class="sxs-lookup"><span data-stu-id="1102d-108">However, in multi-step approvals both pending and previously completed steps are shown.</span></span>

<span data-ttu-id="1102d-109">在 [userConsentRequests](../resources/userconsentrequest.md)中，与请求关联的决策的审批对象。</span><span class="sxs-lookup"><span data-stu-id="1102d-109">In [userConsentRequests](../resources/userconsentrequest.md), the approval object for decisions associated with a request.</span></span>

## <a name="methods"></a><span data-ttu-id="1102d-110">Methods</span><span class="sxs-lookup"><span data-stu-id="1102d-110">Methods</span></span>

| <span data-ttu-id="1102d-111">方法</span><span class="sxs-lookup"><span data-stu-id="1102d-111">Method</span></span>       | <span data-ttu-id="1102d-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="1102d-112">Return Type</span></span> | <span data-ttu-id="1102d-113">说明</span><span class="sxs-lookup"><span data-stu-id="1102d-113">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="1102d-114">获取审批</span><span class="sxs-lookup"><span data-stu-id="1102d-114">Get approval</span></span>](../api/approval-get.md) | [<span data-ttu-id="1102d-115">审批</span><span class="sxs-lookup"><span data-stu-id="1102d-115">approval</span></span>](approval.md) | <span data-ttu-id="1102d-116">检索 **审批对象的属性** 。</span><span class="sxs-lookup"><span data-stu-id="1102d-116">Retrieve the properties of an **approval** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="1102d-117">属性</span><span class="sxs-lookup"><span data-stu-id="1102d-117">Properties</span></span>
|<span data-ttu-id="1102d-118">属性</span><span class="sxs-lookup"><span data-stu-id="1102d-118">Property</span></span>|<span data-ttu-id="1102d-119">类型</span><span class="sxs-lookup"><span data-stu-id="1102d-119">Type</span></span>|<span data-ttu-id="1102d-120">说明</span><span class="sxs-lookup"><span data-stu-id="1102d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1102d-121">id</span><span class="sxs-lookup"><span data-stu-id="1102d-121">id</span></span>|<span data-ttu-id="1102d-122">String</span><span class="sxs-lookup"><span data-stu-id="1102d-122">String</span></span>|<span data-ttu-id="1102d-123">审批对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="1102d-123">The identifier of the approval object.</span></span>|
|<span data-ttu-id="1102d-124">步骤</span><span class="sxs-lookup"><span data-stu-id="1102d-124">steps</span></span>|<span data-ttu-id="1102d-125">[approvalStep](../resources/approvalstep.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1102d-125">[approvalStep](../resources/approvalstep.md) collection</span></span>|<span data-ttu-id="1102d-126">用于表示与在 approvalStage 中配置的审批过程中的单步 [相关的决定](../resources/approvalstage.md)。</span><span class="sxs-lookup"><span data-stu-id="1102d-126">Used to represent the decision associated with a single step in the approval process configured in [approvalStage](../resources/approvalstage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1102d-127">关系</span><span class="sxs-lookup"><span data-stu-id="1102d-127">Relationships</span></span>
|<span data-ttu-id="1102d-128">关系</span><span class="sxs-lookup"><span data-stu-id="1102d-128">Relationship</span></span>|<span data-ttu-id="1102d-129">类型</span><span class="sxs-lookup"><span data-stu-id="1102d-129">Type</span></span>|<span data-ttu-id="1102d-130">说明</span><span class="sxs-lookup"><span data-stu-id="1102d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1102d-131">stages</span><span class="sxs-lookup"><span data-stu-id="1102d-131">stages</span></span>|<span data-ttu-id="1102d-132">[approvalStage](../resources/approvalstage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1102d-132">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="1102d-133">用于访问包分配策略 的 **requestApprovalSettings** 属性中审批设置的 **approvalStages** [属性](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="1102d-133">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="1102d-134">指定每个阶段的主要、回退和升级审批者。</span><span class="sxs-lookup"><span data-stu-id="1102d-134">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1102d-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1102d-135">JSON representation</span></span>
<span data-ttu-id="1102d-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1102d-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "steps": [{
        "@odata.type": "#microsoft.graph.approvalStep"
    }]
}
```
