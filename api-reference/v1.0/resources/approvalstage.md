---
title: approvalStage 资源类型
description: 与 userConsentRequest 关联的 approvalStage 对象。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d6212553d9364c4352bf1d6796156a4020854bf1
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469527"
---
# <a name="approvalstage-resource-type"></a><span data-ttu-id="146af-103">approvalStage 资源类型</span><span class="sxs-lookup"><span data-stu-id="146af-103">approvalStage resource type</span></span>

<span data-ttu-id="146af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="146af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="146af-105">指定审批中的决策阶段。</span><span class="sxs-lookup"><span data-stu-id="146af-105">Specifies decision stages in the approval.</span></span>

## <a name="properties"></a><span data-ttu-id="146af-106">属性</span><span class="sxs-lookup"><span data-stu-id="146af-106">Properties</span></span>

|<span data-ttu-id="146af-107">属性</span><span class="sxs-lookup"><span data-stu-id="146af-107">Property</span></span>|<span data-ttu-id="146af-108">类型</span><span class="sxs-lookup"><span data-stu-id="146af-108">Type</span></span>|<span data-ttu-id="146af-109">说明</span><span class="sxs-lookup"><span data-stu-id="146af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="146af-110">assignedToMe</span><span class="sxs-lookup"><span data-stu-id="146af-110">assignedToMe</span></span>|<span data-ttu-id="146af-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="146af-111">Boolean</span></span>|<span data-ttu-id="146af-112">指示是否将阶段分配给呼叫用户进行审阅。</span><span class="sxs-lookup"><span data-stu-id="146af-112">Indicates whether the stage is assigned to the calling user to review.</span></span> <span data-ttu-id="146af-113">只读。</span><span class="sxs-lookup"><span data-stu-id="146af-113">Read-only.</span></span>|
|<span data-ttu-id="146af-114">displayName</span><span class="sxs-lookup"><span data-stu-id="146af-114">displayName</span></span>|<span data-ttu-id="146af-115">String</span><span class="sxs-lookup"><span data-stu-id="146af-115">String</span></span>|<span data-ttu-id="146af-116">策略创建者提供用于标识审批阶段的标签。</span><span class="sxs-lookup"><span data-stu-id="146af-116">The label provided by the policy creator to identify an approval stage.</span></span> <span data-ttu-id="146af-117">只读。</span><span class="sxs-lookup"><span data-stu-id="146af-117">Read-only.</span></span>|
|<span data-ttu-id="146af-118">id</span><span class="sxs-lookup"><span data-stu-id="146af-118">id</span></span>|<span data-ttu-id="146af-119">String</span><span class="sxs-lookup"><span data-stu-id="146af-119">String</span></span>|<span data-ttu-id="146af-120">与审批对象关联的阶段的标识符。</span><span class="sxs-lookup"><span data-stu-id="146af-120">The identifier of the stage associated with an approval object.</span></span> <span data-ttu-id="146af-121">只读。</span><span class="sxs-lookup"><span data-stu-id="146af-121">Read-only.</span></span>|
|<span data-ttu-id="146af-122">justification</span><span class="sxs-lookup"><span data-stu-id="146af-122">justification</span></span>|<span data-ttu-id="146af-123">String</span><span class="sxs-lookup"><span data-stu-id="146af-123">String</span></span>|<span data-ttu-id="146af-124">与审批阶段决策相关的理由。</span><span class="sxs-lookup"><span data-stu-id="146af-124">The justification associated with the approval stage decision.</span></span>|
|<span data-ttu-id="146af-125">reviewResult</span><span class="sxs-lookup"><span data-stu-id="146af-125">reviewResult</span></span>|<span data-ttu-id="146af-126">String</span><span class="sxs-lookup"><span data-stu-id="146af-126">String</span></span>|<span data-ttu-id="146af-127">此审批记录的结果。</span><span class="sxs-lookup"><span data-stu-id="146af-127">The result of this approval record.</span></span> <span data-ttu-id="146af-128">可能的值包括 `NotReviewed` `Approved` `Denied` ：、、。</span><span class="sxs-lookup"><span data-stu-id="146af-128">Possible values include: `NotReviewed`, `Approved`, `Denied`.</span></span>|
|<span data-ttu-id="146af-129">reviewedBy</span><span class="sxs-lookup"><span data-stu-id="146af-129">reviewedBy</span></span>|[<span data-ttu-id="146af-130">userIdentity</span><span class="sxs-lookup"><span data-stu-id="146af-130">userIdentity</span></span>](useridentity.md) | <span data-ttu-id="146af-131">审阅者的标识符。</span><span class="sxs-lookup"><span data-stu-id="146af-131">The identifier of the reviewer.</span></span> <span data-ttu-id="146af-132">只读。</span><span class="sxs-lookup"><span data-stu-id="146af-132">Read-only.</span></span>|
|<span data-ttu-id="146af-133">reviewedDateTime</span><span class="sxs-lookup"><span data-stu-id="146af-133">reviewedDateTime</span></span>|<span data-ttu-id="146af-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="146af-134">DateTimeOffset</span></span>|<span data-ttu-id="146af-135">记录决策的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="146af-135">The date and time when a decision was recorded.</span></span> <span data-ttu-id="146af-136">日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="146af-136">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="146af-137">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="146af-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="146af-138">只读。</span><span class="sxs-lookup"><span data-stu-id="146af-138">Read-only.</span></span>|
|<span data-ttu-id="146af-139">状态</span><span class="sxs-lookup"><span data-stu-id="146af-139">status</span></span>|<span data-ttu-id="146af-140">String</span><span class="sxs-lookup"><span data-stu-id="146af-140">String</span></span>|<span data-ttu-id="146af-141">阶段状态。</span><span class="sxs-lookup"><span data-stu-id="146af-141">The stage status.</span></span> <span data-ttu-id="146af-142">可能的值 `InProgress` `Initializing` `Completed` ：、、、。 `Expired`</span><span class="sxs-lookup"><span data-stu-id="146af-142">Possible values: `InProgress`, `Initializing`, `Completed`, `Expired`.</span></span> <span data-ttu-id="146af-143">只读。</span><span class="sxs-lookup"><span data-stu-id="146af-143">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="146af-144">关系</span><span class="sxs-lookup"><span data-stu-id="146af-144">Relationships</span></span>

<span data-ttu-id="146af-145">无。</span><span class="sxs-lookup"><span data-stu-id="146af-145">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="146af-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="146af-146">JSON representation</span></span>

<span data-ttu-id="146af-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="146af-147">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approvalStage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.approvalStage",
  "id": "String (identifier)",
  "displayName": "String",
  "status": "String",
  "assignedToMe": "Boolean",
  "reviewedBy": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewedDateTime": "String (timestamp)",
  "reviewResult": "String",
  "justification": "String"
}
```
