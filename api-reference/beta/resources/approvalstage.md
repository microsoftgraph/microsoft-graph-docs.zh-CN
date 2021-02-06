---
title: approvalStage 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性中审批设置的 approvalStages 属性。 指定每个阶段的主要、回退和升级审批者。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d24f8def3520cf2605f30dc47ab06f52e09fc163
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135253"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="33cca-104">approvalStage 复杂类型</span><span class="sxs-lookup"><span data-stu-id="33cca-104">approvalStage complex type</span></span>

<span data-ttu-id="33cca-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33cca-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33cca-106">用于访问包分配策略的 **requestApprovalSettings** 属性中审批设置的 **approvalStages** [属性](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="33cca-106">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="33cca-107">指定每个阶段的主要、回退和升级审批者。</span><span class="sxs-lookup"><span data-stu-id="33cca-107">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="33cca-108">属性</span><span class="sxs-lookup"><span data-stu-id="33cca-108">Properties</span></span>

| <span data-ttu-id="33cca-109">属性</span><span class="sxs-lookup"><span data-stu-id="33cca-109">Property</span></span>                     | <span data-ttu-id="33cca-110">类型</span><span class="sxs-lookup"><span data-stu-id="33cca-110">Type</span></span>                      | <span data-ttu-id="33cca-111">说明</span><span class="sxs-lookup"><span data-stu-id="33cca-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="33cca-112">approvalStageTimeOutInDays</span><span class="sxs-lookup"><span data-stu-id="33cca-112">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="33cca-113">Int32</span><span class="sxs-lookup"><span data-stu-id="33cca-113">Int32</span></span> | <span data-ttu-id="33cca-114">请求在被自动拒绝之前可以等待响应的天数。</span><span class="sxs-lookup"><span data-stu-id="33cca-114">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="33cca-115">isApproverJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="33cca-115">isApproverJustificationRequired</span></span> |<span data-ttu-id="33cca-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="33cca-116">Boolean</span></span> | <span data-ttu-id="33cca-117">指示是否需要审批者提供批准请求的理由。</span><span class="sxs-lookup"><span data-stu-id="33cca-117">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="33cca-118">isEscalationEnabled</span><span class="sxs-lookup"><span data-stu-id="33cca-118">isEscalationEnabled</span></span> |<span data-ttu-id="33cca-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="33cca-119">Boolean</span></span> | <span data-ttu-id="33cca-120">如果为 true，则在此审批阶段配置一个或多个升级审批者。</span><span class="sxs-lookup"><span data-stu-id="33cca-120">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="33cca-121">escalationTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="33cca-121">escalationTimeInMinutes</span></span> |<span data-ttu-id="33cca-122">Int32</span><span class="sxs-lookup"><span data-stu-id="33cca-122">Int32</span></span> | <span data-ttu-id="33cca-123">如果需要升级，则请求可以挂起主要审批者的响应的时间。</span><span class="sxs-lookup"><span data-stu-id="33cca-123">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="33cca-124">primaryApprovers</span><span class="sxs-lookup"><span data-stu-id="33cca-124">primaryApprovers</span></span> | <span data-ttu-id="33cca-125">[userSet](userset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="33cca-125">[userSet](userset.md) collection</span></span>| <span data-ttu-id="33cca-126">将要求其批准请求的用户。</span><span class="sxs-lookup"><span data-stu-id="33cca-126">The users who will be asked to approve requests.</span></span> <span data-ttu-id="33cca-127">[singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md)和[externalSponsors 的集合](externalsponsors.md)。</span><span class="sxs-lookup"><span data-stu-id="33cca-127">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="33cca-128">escalationApprovers</span><span class="sxs-lookup"><span data-stu-id="33cca-128">escalationApprovers</span></span> | <span data-ttu-id="33cca-129">[userSet](userset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="33cca-129">[userSet](userset.md) collection</span></span>| <span data-ttu-id="33cca-130">如果启用升级，并且主要审批者在升级时间之前未响应，则 escalationApprovers 是需要批准请求的用户。</span><span class="sxs-lookup"><span data-stu-id="33cca-130">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="33cca-131">它可以是 [singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md) 和 [externalSponsors 的集合](externalsponsors.md)。</span><span class="sxs-lookup"><span data-stu-id="33cca-131">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="33cca-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33cca-132">JSON representation</span></span>

<span data-ttu-id="33cca-133">以下是请求审批阶段的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33cca-133">The following is a JSON representation of the request approval stage.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage"
}-->

```json

{
    "approvalStageTimeOutInDays": 14,
    "isApproverJustificationRequired": true,
    "isEscalationEnabled": true,
    "escalationTimeInMinutes": 11520,
    "primaryApprovers": [{"@odata.type": "microsoft.graph.userSet"}],
    "escalationApprovers": [{"@odata.type": "microsoft.graph.userSet"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


