---
title: 审批资源类型
description: 与 accessPackageAssignmentRequest 关联的审批对象。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d46630b563674153ef687a8e8f86dce70eec9985
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761259"
---
# <a name="approval-resource-type"></a><span data-ttu-id="65bd9-103">审批资源类型</span><span class="sxs-lookup"><span data-stu-id="65bd9-103">approval resource type</span></span>

<span data-ttu-id="65bd9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65bd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65bd9-105">在 [Azure AD 权利管理](entitlementmanagement-root.md)中，与 关联的决策的审批对象 `accessPackageAssignmentRequest` 。</span><span class="sxs-lookup"><span data-stu-id="65bd9-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), the approval object for decisions associated with the `accessPackageAssignmentRequest`.</span></span> <span data-ttu-id="65bd9-106">单个步骤请求可以有一个与它关联的步骤，审批者可以处理该步骤。</span><span class="sxs-lookup"><span data-stu-id="65bd9-106">A single step request can have one step associated with it which approvers can act on.</span></span> <span data-ttu-id="65bd9-107">同样，多步骤请求可以有多个与之关联的步骤，审批者可以执行这些步骤。</span><span class="sxs-lookup"><span data-stu-id="65bd9-107">Similarly, a multi-step request can have multiple steps associated with it which approvers can act on.</span></span> <span data-ttu-id="65bd9-108">但是，在多步骤审批中，将显示挂起的步骤和之前完成的步骤。</span><span class="sxs-lookup"><span data-stu-id="65bd9-108">However, in multi-step approvals both pending and previously completed steps are shown.</span></span>

## <a name="methods"></a><span data-ttu-id="65bd9-109">方法</span><span class="sxs-lookup"><span data-stu-id="65bd9-109">Methods</span></span>

| <span data-ttu-id="65bd9-110">方法</span><span class="sxs-lookup"><span data-stu-id="65bd9-110">Method</span></span>       | <span data-ttu-id="65bd9-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="65bd9-111">Return Type</span></span> | <span data-ttu-id="65bd9-112">说明</span><span class="sxs-lookup"><span data-stu-id="65bd9-112">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="65bd9-113">获取审批</span><span class="sxs-lookup"><span data-stu-id="65bd9-113">Get approval</span></span>](../api/approval-get.md) | [<span data-ttu-id="65bd9-114">审批</span><span class="sxs-lookup"><span data-stu-id="65bd9-114">approval</span></span>](approval.md) | <span data-ttu-id="65bd9-115">检索 **审批对象的属性** 。</span><span class="sxs-lookup"><span data-stu-id="65bd9-115">Retrieve the properties of an **approval** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="65bd9-116">属性</span><span class="sxs-lookup"><span data-stu-id="65bd9-116">Properties</span></span>
|<span data-ttu-id="65bd9-117">属性</span><span class="sxs-lookup"><span data-stu-id="65bd9-117">Property</span></span>|<span data-ttu-id="65bd9-118">类型</span><span class="sxs-lookup"><span data-stu-id="65bd9-118">Type</span></span>|<span data-ttu-id="65bd9-119">说明</span><span class="sxs-lookup"><span data-stu-id="65bd9-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65bd9-120">id</span><span class="sxs-lookup"><span data-stu-id="65bd9-120">id</span></span>|<span data-ttu-id="65bd9-121">String</span><span class="sxs-lookup"><span data-stu-id="65bd9-121">String</span></span>|<span data-ttu-id="65bd9-122">审批对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="65bd9-122">The identifier of the approval object.</span></span>|
|<span data-ttu-id="65bd9-123">步骤</span><span class="sxs-lookup"><span data-stu-id="65bd9-123">steps</span></span>|<span data-ttu-id="65bd9-124">[approvalStep](../resources/approvalstep.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65bd9-124">[approvalStep](../resources/approvalstep.md) collection</span></span>|<span data-ttu-id="65bd9-125">用于表示与在 approvalStage 中配置的审批过程中的单步 [相关的决定](../resources/approvalstage.md)。</span><span class="sxs-lookup"><span data-stu-id="65bd9-125">Used to represent the decision associated with a single step in the approval process configured in [approvalStage](../resources/approvalstage.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="65bd9-126">关系</span><span class="sxs-lookup"><span data-stu-id="65bd9-126">Relationships</span></span>
|<span data-ttu-id="65bd9-127">关系</span><span class="sxs-lookup"><span data-stu-id="65bd9-127">Relationship</span></span>|<span data-ttu-id="65bd9-128">类型</span><span class="sxs-lookup"><span data-stu-id="65bd9-128">Type</span></span>|<span data-ttu-id="65bd9-129">说明</span><span class="sxs-lookup"><span data-stu-id="65bd9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65bd9-130">stages</span><span class="sxs-lookup"><span data-stu-id="65bd9-130">stages</span></span>|<span data-ttu-id="65bd9-131">[approvalStage](../resources/approvalstage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65bd9-131">[approvalStage](../resources/approvalstage.md) collection</span></span>|<span data-ttu-id="65bd9-132">用于访问包分配策略 的 **requestApprovalSettings** 属性中审批设置的 **approvalStages** [属性](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="65bd9-132">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="65bd9-133">指定每个阶段的主要、回退和升级审批者。</span><span class="sxs-lookup"><span data-stu-id="65bd9-133">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="65bd9-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65bd9-134">JSON representation</span></span>
<span data-ttu-id="65bd9-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65bd9-135">The following is a JSON representation of the resource.</span></span>
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
