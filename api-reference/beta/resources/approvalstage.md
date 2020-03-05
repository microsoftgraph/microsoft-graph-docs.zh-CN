---
title: approvalStage 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性中的审批设置的 approvalStages 属性。 指定每个阶段的主、回退和升级审批者。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0edcb4af5ae6bbc154d0748b57ec83efcb3137f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508224"
---
# <a name="approvalstage-complex-type"></a><span data-ttu-id="0faa6-104">approvalStage 复杂类型</span><span class="sxs-lookup"><span data-stu-id="0faa6-104">approvalStage complex type</span></span>

<span data-ttu-id="0faa6-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0faa6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0faa6-106">用于[访问包分配策略](accesspackageassignmentpolicy.md)的**requestApprovalSettings**属性中的审批设置的**approvalStages**属性。</span><span class="sxs-lookup"><span data-stu-id="0faa6-106">Used for the **approvalStages** property of approval settings in the **requestApprovalSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="0faa6-107">指定每个阶段的主、回退和升级审批者。</span><span class="sxs-lookup"><span data-stu-id="0faa6-107">Specifies the primary, fallback, and escalation approvers of each stage.</span></span>

## <a name="properties"></a><span data-ttu-id="0faa6-108">属性</span><span class="sxs-lookup"><span data-stu-id="0faa6-108">Properties</span></span>

| <span data-ttu-id="0faa6-109">属性</span><span class="sxs-lookup"><span data-stu-id="0faa6-109">Property</span></span>                     | <span data-ttu-id="0faa6-110">类型</span><span class="sxs-lookup"><span data-stu-id="0faa6-110">Type</span></span>                      | <span data-ttu-id="0faa6-111">说明</span><span class="sxs-lookup"><span data-stu-id="0faa6-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="0faa6-112">approvalStageTimeOutInDays</span><span class="sxs-lookup"><span data-stu-id="0faa6-112">approvalStageTimeOutInDays</span></span> |<span data-ttu-id="0faa6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0faa6-113">Int32</span></span> | <span data-ttu-id="0faa6-114">请求在被自动拒绝前可等待响应的天数。</span><span class="sxs-lookup"><span data-stu-id="0faa6-114">The number of days that a request can be pending a response before it is automatically denied.</span></span> |
| <span data-ttu-id="0faa6-115">isApproverJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="0faa6-115">isApproverJustificationRequired</span></span> |<span data-ttu-id="0faa6-116">布尔</span><span class="sxs-lookup"><span data-stu-id="0faa6-116">Boolean</span></span> | <span data-ttu-id="0faa6-117">指示是否需要审批者提供审批请求的理由。</span><span class="sxs-lookup"><span data-stu-id="0faa6-117">Indicates whether the approver is required to provide a justification for approving a request.</span></span> |
| <span data-ttu-id="0faa6-118">isEscalationEnabled</span><span class="sxs-lookup"><span data-stu-id="0faa6-118">isEscalationEnabled</span></span> |<span data-ttu-id="0faa6-119">布尔</span><span class="sxs-lookup"><span data-stu-id="0faa6-119">Boolean</span></span> | <span data-ttu-id="0faa6-120">如果为 true，则在此审批阶段中配置一个或多个升级审批者。</span><span class="sxs-lookup"><span data-stu-id="0faa6-120">If true, then one or more escalation approvers are configured in this approval stage.</span></span> |
| <span data-ttu-id="0faa6-121">escalationTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="0faa6-121">escalationTimeInMinutes</span></span> |<span data-ttu-id="0faa6-122">Int32</span><span class="sxs-lookup"><span data-stu-id="0faa6-122">Int32</span></span> | <span data-ttu-id="0faa6-123">如果需要升级，请求可以挂起主审批者的响应。</span><span class="sxs-lookup"><span data-stu-id="0faa6-123">If escalation is required, the time a request can be pending a response from a primary approver.</span></span> |
| <span data-ttu-id="0faa6-124">primaryApprovers</span><span class="sxs-lookup"><span data-stu-id="0faa6-124">primaryApprovers</span></span> | <span data-ttu-id="0faa6-125">[userSet](userset.md)集合</span><span class="sxs-lookup"><span data-stu-id="0faa6-125">[userSet](userset.md) collection</span></span>| <span data-ttu-id="0faa6-126">将要求用户批准请求的用户。</span><span class="sxs-lookup"><span data-stu-id="0faa6-126">The users who will be asked to approve requests.</span></span> <span data-ttu-id="0faa6-127">[SingleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md)和[externalSponsors](externalsponsors.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="0faa6-127">A collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span> |
| <span data-ttu-id="0faa6-128">escalationApprovers</span><span class="sxs-lookup"><span data-stu-id="0faa6-128">escalationApprovers</span></span> | <span data-ttu-id="0faa6-129">[userSet](userset.md)集合</span><span class="sxs-lookup"><span data-stu-id="0faa6-129">[userSet](userset.md) collection</span></span>| <span data-ttu-id="0faa6-130">如果启用了升级，并且主审批者在升级时间之前没有响应，则 escalationApprovers 是将被要求批准请求的用户。</span><span class="sxs-lookup"><span data-stu-id="0faa6-130">If escalation is enabled and the primary approvers do not respond before the escalation time, the escalationApprovers are the users who will be asked to approve requests.</span></span> <span data-ttu-id="0faa6-131">它可以是[singleUser](singleuser.md)、 [groupMembers](groupmembers.md)、 [requestorManager](requestormanager.md)、 [internalSponsors](internalsponsors.md)和[externalSponsors](externalsponsors.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="0faa6-131">This can be a collection of [singleUser](singleuser.md), [groupMembers](groupmembers.md), [requestorManager](requestormanager.md), [internalSponsors](internalsponsors.md) and [externalSponsors](externalsponsors.md).</span></span>|



## <a name="json-representation"></a><span data-ttu-id="0faa6-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0faa6-132">JSON representation</span></span>

<span data-ttu-id="0faa6-133">以下是请求审批阶段的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0faa6-133">The following is a JSON representation of the request approval stage.</span></span>

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
