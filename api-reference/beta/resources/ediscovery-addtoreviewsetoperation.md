---
title: addToReviewSetOperation 资源类型
description: 将 sourceCollection 的结果添加到 reviewSet
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: d7323fbd6d2d068888d556328fc3ea4e399ab2fe
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446674"
---
# <a name="addtoreviewsetoperation-resource-type"></a><span data-ttu-id="8990f-103">addToReviewSetOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="8990f-103">addToReviewSetOperation resource type</span></span>

<span data-ttu-id="8990f-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8990f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8990f-105">表示将 [sourceCollection](../resources/ediscovery-sourcecollection.md) 添加到 [reviewSet 的操作](../resources/ediscovery-reviewset.md)。</span><span class="sxs-lookup"><span data-stu-id="8990f-105">Represents an operation to add a [sourceCollection](../resources/ediscovery-sourcecollection.md) to a [reviewSet](../resources/ediscovery-reviewset.md).</span></span>

<span data-ttu-id="8990f-106">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="8990f-106">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8990f-107">Methods</span><span class="sxs-lookup"><span data-stu-id="8990f-107">Methods</span></span>

<span data-ttu-id="8990f-108">无。</span><span class="sxs-lookup"><span data-stu-id="8990f-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="8990f-109">属性</span><span class="sxs-lookup"><span data-stu-id="8990f-109">Properties</span></span>

|<span data-ttu-id="8990f-110">属性</span><span class="sxs-lookup"><span data-stu-id="8990f-110">Property</span></span>|<span data-ttu-id="8990f-111">类型</span><span class="sxs-lookup"><span data-stu-id="8990f-111">Type</span></span>|<span data-ttu-id="8990f-112">说明</span><span class="sxs-lookup"><span data-stu-id="8990f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8990f-113">action</span><span class="sxs-lookup"><span data-stu-id="8990f-113">action</span></span>|[<span data-ttu-id="8990f-114">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="8990f-114">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="8990f-115">此实体的大小写操作将始终为 `addToReviewSet` 。</span><span class="sxs-lookup"><span data-stu-id="8990f-115">The case action for this entity will always be `addToReviewSet`.</span></span> <span data-ttu-id="8990f-116">只读。</span><span class="sxs-lookup"><span data-stu-id="8990f-116">Read-only.</span></span> <span data-ttu-id="8990f-117">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="8990f-117">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="8990f-118">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="8990f-118">completedDateTime</span></span>|<span data-ttu-id="8990f-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8990f-119">DateTimeOffset</span></span>|<span data-ttu-id="8990f-120">操作完成的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8990f-120">The date and time the operation was completed.</span></span> <span data-ttu-id="8990f-121">只读。</span><span class="sxs-lookup"><span data-stu-id="8990f-121">Read-only.</span></span> <span data-ttu-id="8990f-122">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="8990f-122">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="8990f-123">createdBy</span><span class="sxs-lookup"><span data-stu-id="8990f-123">createdBy</span></span>|[<span data-ttu-id="8990f-124">identitySet</span><span class="sxs-lookup"><span data-stu-id="8990f-124">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="8990f-125">创建操作的用户。</span><span class="sxs-lookup"><span data-stu-id="8990f-125">The user who created the operation.</span></span> <span data-ttu-id="8990f-126">只读。</span><span class="sxs-lookup"><span data-stu-id="8990f-126">Read-only.</span></span> <span data-ttu-id="8990f-127">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="8990f-127">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="8990f-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8990f-128">createdDateTime</span></span>|<span data-ttu-id="8990f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8990f-129">DateTimeOffset</span></span>|<span data-ttu-id="8990f-130">操作开始的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8990f-130">The date and time the operation was started.</span></span> <span data-ttu-id="8990f-131">只读。</span><span class="sxs-lookup"><span data-stu-id="8990f-131">Read-only.</span></span> <span data-ttu-id="8990f-132">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="8990f-132">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="8990f-133">id</span><span class="sxs-lookup"><span data-stu-id="8990f-133">id</span></span>|<span data-ttu-id="8990f-134">String</span><span class="sxs-lookup"><span data-stu-id="8990f-134">String</span></span>| <span data-ttu-id="8990f-135">操作 ID。</span><span class="sxs-lookup"><span data-stu-id="8990f-135">The ID for the operation.</span></span> <span data-ttu-id="8990f-136">只读。</span><span class="sxs-lookup"><span data-stu-id="8990f-136">Read-only.</span></span> <span data-ttu-id="8990f-137">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="8990f-137">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="8990f-138">percentProgress</span><span class="sxs-lookup"><span data-stu-id="8990f-138">percentProgress</span></span>|<span data-ttu-id="8990f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8990f-139">Int32</span></span>|<span data-ttu-id="8990f-140">操作的进度。</span><span class="sxs-lookup"><span data-stu-id="8990f-140">The progress of the operation.</span></span> <span data-ttu-id="8990f-141">只读。</span><span class="sxs-lookup"><span data-stu-id="8990f-141">Read-only.</span></span> <span data-ttu-id="8990f-142">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="8990f-142">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="8990f-143">resultInfo</span><span class="sxs-lookup"><span data-stu-id="8990f-143">resultInfo</span></span>|[<span data-ttu-id="8990f-144">resultInfo</span><span class="sxs-lookup"><span data-stu-id="8990f-144">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="8990f-145">包含特定于成功和失败的结果信息。</span><span class="sxs-lookup"><span data-stu-id="8990f-145">Contains success and failure-specific result information.</span></span> <span data-ttu-id="8990f-146">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="8990f-146">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="8990f-147">status</span><span class="sxs-lookup"><span data-stu-id="8990f-147">status</span></span>|[<span data-ttu-id="8990f-148">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="8990f-148">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="8990f-149">案例操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8990f-149">The status of the case operation.</span></span> <span data-ttu-id="8990f-150">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="8990f-150">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="8990f-151">可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="8990f-151">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

### <a name="datacollectionscope-values"></a><span data-ttu-id="8990f-152">dataCollectionScope 值</span><span class="sxs-lookup"><span data-stu-id="8990f-152">dataCollectionScope values</span></span>

|<span data-ttu-id="8990f-153">成员</span><span class="sxs-lookup"><span data-stu-id="8990f-153">Member</span></span>|<span data-ttu-id="8990f-154">说明</span><span class="sxs-lookup"><span data-stu-id="8990f-154">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="8990f-155">allVersions</span><span class="sxs-lookup"><span data-stu-id="8990f-155">allVersions</span></span>|<span data-ttu-id="8990f-156">包含网站中文件的所有版本。</span><span class="sxs-lookup"><span data-stu-id="8990f-156">Include all versions of files from sites.</span></span>|
|<span data-ttu-id="8990f-157">linkedFiles</span><span class="sxs-lookup"><span data-stu-id="8990f-157">linkedFiles</span></span>|<span data-ttu-id="8990f-158">将 **云附件** 与电子邮件一起包括在集合中。</span><span class="sxs-lookup"><span data-stu-id="8990f-158">Include **cloud attachment** with emails in the collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8990f-159">关系</span><span class="sxs-lookup"><span data-stu-id="8990f-159">Relationships</span></span>

|<span data-ttu-id="8990f-160">关系</span><span class="sxs-lookup"><span data-stu-id="8990f-160">Relationship</span></span>|<span data-ttu-id="8990f-161">类型</span><span class="sxs-lookup"><span data-stu-id="8990f-161">Type</span></span>|<span data-ttu-id="8990f-162">说明</span><span class="sxs-lookup"><span data-stu-id="8990f-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8990f-163">reviewSet</span><span class="sxs-lookup"><span data-stu-id="8990f-163">reviewSet</span></span>|[<span data-ttu-id="8990f-164">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="8990f-164">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md)| <span data-ttu-id="8990f-165">与源集合查询匹配的项添加到的审阅集。</span><span class="sxs-lookup"><span data-stu-id="8990f-165">The review set to which items matching the source collection query are added to.</span></span> |
|<span data-ttu-id="8990f-166">sourceCollection</span><span class="sxs-lookup"><span data-stu-id="8990f-166">sourceCollection</span></span>|[<span data-ttu-id="8990f-167">microsoft.graph.ediscovery.sourceCollection</span><span class="sxs-lookup"><span data-stu-id="8990f-167">microsoft.graph.ediscovery.sourceCollection</span></span>](../resources/ediscovery-sourceCollection.md)| <span data-ttu-id="8990f-168">正在从中添加项目的 sourceCollection。</span><span class="sxs-lookup"><span data-stu-id="8990f-168">The sourceCollection that items are being added from.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8990f-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8990f-169">JSON representation</span></span>

<span data-ttu-id="8990f-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8990f-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.addToReviewSetOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.addToReviewSetOperation",
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
