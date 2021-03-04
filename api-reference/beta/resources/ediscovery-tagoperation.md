---
title: tagOperation 资源类型
description: 表示基于审阅集查询处理对审阅集内文档应用标记的操作。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2af9b255e643a46f5f065b3caf62fda0ae9967a4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446654"
---
# <a name="tagoperation-resource-type"></a><span data-ttu-id="aae10-103">tagOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="aae10-103">tagOperation resource type</span></span>

<span data-ttu-id="aae10-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="aae10-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aae10-105">表示基于审阅集查询处理对审阅集内文档应用标记的操作。</span><span class="sxs-lookup"><span data-stu-id="aae10-105">Represents the operation that handles applying tags to documents in a review set based on a review set query.</span></span>

<span data-ttu-id="aae10-106">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="aae10-106">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="aae10-107">Methods</span><span class="sxs-lookup"><span data-stu-id="aae10-107">Methods</span></span>

<span data-ttu-id="aae10-108">无。</span><span class="sxs-lookup"><span data-stu-id="aae10-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="aae10-109">属性</span><span class="sxs-lookup"><span data-stu-id="aae10-109">Properties</span></span>

|<span data-ttu-id="aae10-110">属性</span><span class="sxs-lookup"><span data-stu-id="aae10-110">Property</span></span>|<span data-ttu-id="aae10-111">类型</span><span class="sxs-lookup"><span data-stu-id="aae10-111">Type</span></span>|<span data-ttu-id="aae10-112">说明</span><span class="sxs-lookup"><span data-stu-id="aae10-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aae10-113">action</span><span class="sxs-lookup"><span data-stu-id="aae10-113">action</span></span>|[<span data-ttu-id="aae10-114">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="aae10-114">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="aae10-115">此实体的大小写操作将始终为 `applyTags` 。</span><span class="sxs-lookup"><span data-stu-id="aae10-115">The case action for this entity will always be `applyTags`.</span></span> <span data-ttu-id="aae10-116">只读。</span><span class="sxs-lookup"><span data-stu-id="aae10-116">Read-only.</span></span> <span data-ttu-id="aae10-117">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="aae10-117">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="aae10-118">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="aae10-118">completedDateTime</span></span>|<span data-ttu-id="aae10-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae10-119">DateTimeOffset</span></span>|<span data-ttu-id="aae10-120">操作完成的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="aae10-120">The date and time the operation was completed.</span></span> <span data-ttu-id="aae10-121">只读。</span><span class="sxs-lookup"><span data-stu-id="aae10-121">Read-only.</span></span> <span data-ttu-id="aae10-122">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="aae10-122">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="aae10-123">createdBy</span><span class="sxs-lookup"><span data-stu-id="aae10-123">createdBy</span></span>|[<span data-ttu-id="aae10-124">identitySet</span><span class="sxs-lookup"><span data-stu-id="aae10-124">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="aae10-125">创建操作的用户。</span><span class="sxs-lookup"><span data-stu-id="aae10-125">The user who created the operation.</span></span> <span data-ttu-id="aae10-126">只读。</span><span class="sxs-lookup"><span data-stu-id="aae10-126">Read-only.</span></span> <span data-ttu-id="aae10-127">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="aae10-127">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="aae10-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aae10-128">createdDateTime</span></span>|<span data-ttu-id="aae10-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aae10-129">DateTimeOffset</span></span>|<span data-ttu-id="aae10-130">操作开始的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="aae10-130">The date and time the operation was started.</span></span> <span data-ttu-id="aae10-131">只读。</span><span class="sxs-lookup"><span data-stu-id="aae10-131">Read-only.</span></span> <span data-ttu-id="aae10-132">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="aae10-132">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="aae10-133">id</span><span class="sxs-lookup"><span data-stu-id="aae10-133">id</span></span>|<span data-ttu-id="aae10-134">String</span><span class="sxs-lookup"><span data-stu-id="aae10-134">String</span></span>| <span data-ttu-id="aae10-135">操作 ID。</span><span class="sxs-lookup"><span data-stu-id="aae10-135">The ID for the operation.</span></span> <span data-ttu-id="aae10-136">只读。</span><span class="sxs-lookup"><span data-stu-id="aae10-136">Read-only.</span></span> <span data-ttu-id="aae10-137">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="aae10-137">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="aae10-138">percentProgress</span><span class="sxs-lookup"><span data-stu-id="aae10-138">percentProgress</span></span>|<span data-ttu-id="aae10-139">Int32</span><span class="sxs-lookup"><span data-stu-id="aae10-139">Int32</span></span>|<span data-ttu-id="aae10-140">操作的进度。</span><span class="sxs-lookup"><span data-stu-id="aae10-140">The progress of the operation.</span></span> <span data-ttu-id="aae10-141">只读。</span><span class="sxs-lookup"><span data-stu-id="aae10-141">Read-only.</span></span> <span data-ttu-id="aae10-142">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="aae10-142">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="aae10-143">resultInfo</span><span class="sxs-lookup"><span data-stu-id="aae10-143">resultInfo</span></span>|[<span data-ttu-id="aae10-144">resultInfo</span><span class="sxs-lookup"><span data-stu-id="aae10-144">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="aae10-145">包含特定于成功和失败的结果信息。</span><span class="sxs-lookup"><span data-stu-id="aae10-145">Contains success and failure-specific result information.</span></span> <span data-ttu-id="aae10-146">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="aae10-146">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="aae10-147">status</span><span class="sxs-lookup"><span data-stu-id="aae10-147">status</span></span>|[<span data-ttu-id="aae10-148">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="aae10-148">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="aae10-149">案例操作的状态。</span><span class="sxs-lookup"><span data-stu-id="aae10-149">The status of the case operation.</span></span> <span data-ttu-id="aae10-150">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="aae10-150">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="aae10-151">可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="aae10-151">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aae10-152">关系</span><span class="sxs-lookup"><span data-stu-id="aae10-152">Relationships</span></span>

<span data-ttu-id="aae10-153">无。</span><span class="sxs-lookup"><span data-stu-id="aae10-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aae10-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aae10-154">JSON representation</span></span>

<span data-ttu-id="aae10-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aae10-155">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tagOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tagOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```
