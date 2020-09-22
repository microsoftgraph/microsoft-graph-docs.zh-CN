---
title: approvalStage 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性中的审批设置的 approvalStages 属性。 指定每个阶段的主、回退和升级审批者。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: df7e9ce4491ea7a887b79f79d354c9099ea9f5d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050141"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="9a5ee-104">approvalStage 复杂类型</span><span class="sxs-lookup"><span data-stu-id="9a5ee-104">approvalStage complex type</span></span>

<span data-ttu-id="9a5ee-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a5ee-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a5ee-106">用于[访问包分配策略](accesspackageassignmentpolicy.md)的**requestApprovalSettings**属性中的审批设置的**approvalStages**属性。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-106">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="9a5ee-107">指定每个阶段的主、回退和升级审批者。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-107">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="9a5ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a5ee-108">Properties</span></span>

| <span data-ttu-id="9a5ee-109">属性</span><span class="sxs-lookup"><span data-stu-id="9a5ee-109">Property</span></span>                     | <span data-ttu-id="9a5ee-110">类型</span><span class="sxs-lookup"><span data-stu-id="9a5ee-110">Type</span></span>                      | <span data-ttu-id="9a5ee-111">说明</span><span class="sxs-lookup"><span data-stu-id="9a5ee-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="9a5ee-112">approvalStageTimeOutInDays</span><span class="sxs-lookup"><span data-stu-id="9a5ee-112">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="9a5ee-113">Int32</span><span class="sxs-lookup"><span data-stu-id="9a5ee-113">Int32</span></span> | <span data-ttu-id="9a5ee-114">请求在被自动拒绝前可等待响应的天数。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-114">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="9a5ee-115">isApproverJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="9a5ee-115">isApproverJustificationRequired</span></span> |<span data-ttu-id="9a5ee-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a5ee-116">Boolean</span></span> | <span data-ttu-id="9a5ee-117">指示是否需要审批者提供审批请求的理由。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-117">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="9a5ee-118">isEscalationEnabled</span><span class="sxs-lookup"><span data-stu-id="9a5ee-118">isEscalationEnabled</span></span> |<span data-ttu-id="9a5ee-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a5ee-119">Boolean</span></span> | <span data-ttu-id="9a5ee-120">如果为 true，则在此审批阶段中配置一个或多个升级审批者。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-120">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="9a5ee-121">escalationTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="9a5ee-121">escalationTimeInMinutes</span></span> |<span data-ttu-id="9a5ee-122">Int32</span><span class="sxs-lookup"><span data-stu-id="9a5ee-122">Int32</span></span> | <span data-ttu-id="9a5ee-123">如果需要升级，请求可以挂起主审批者的响应。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-123">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="9a5ee-124">primaryApprovers</span><span class="sxs-lookup"><span data-stu-id="9a5ee-124">primaryApprovers</span></span> | <span data-ttu-id="9a5ee-125">[userSet](userset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a5ee-125">[userSet](userset.md) collection</span></span>| <span data-ttu-id="9a5ee-126">将要求用户批准请求的用户。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-126">The users who will be asked to approve requests.</span></span> <span data-ttu-id="9a5ee-127">[SingleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md)和[externalSponsors](externalsponsors.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-127">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="9a5ee-128">escalationApprovers</span><span class="sxs-lookup"><span data-stu-id="9a5ee-128">escalationApprovers</span></span> | <span data-ttu-id="9a5ee-129">[userSet](userset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a5ee-129">[userSet](userset.md) collection</span></span>| <span data-ttu-id="9a5ee-130">如果启用了升级，并且主审批者在升级时间之前没有响应，则 escalationApprovers 是将被要求批准请求的用户。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-130">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="9a5ee-131">它可以是 [singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md) 和 [externalSponsors](externalsponsors.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-131">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="9a5ee-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a5ee-132">JSON representation</span></span>

<span data-ttu-id="9a5ee-133">以下是请求审批阶段的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a5ee-133">The following is a JSON representation of the request approval stage.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalStage",
  "baseType": ""
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


