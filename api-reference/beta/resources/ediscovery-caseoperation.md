---
title: caseOperation 资源类型
description: 一个代表长时间运行电子数据展示过程的抽象实体。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b94aeba03a49f2c49cbf991f0046422a18b20b50
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446659"
---
# <a name="caseoperation-resource-type"></a><span data-ttu-id="3b39a-103">caseOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b39a-103">caseOperation resource type</span></span>

<span data-ttu-id="3b39a-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="3b39a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b39a-105">表示长时间运行电子数据展示过程的抽象实体。</span><span class="sxs-lookup"><span data-stu-id="3b39a-105">An abstract entity that represents a long-running eDiscovery process.</span></span> <span data-ttu-id="3b39a-106">它包含一组在继承实体之间共享的常见属性。</span><span class="sxs-lookup"><span data-stu-id="3b39a-106">It contains a common set of properties that are shared among inheriting entities.</span></span>  <span data-ttu-id="3b39a-107">从 **caseOperation** 派生的实体包括：</span><span class="sxs-lookup"><span data-stu-id="3b39a-107">Entities that derive from **caseOperation** include:</span></span>

- [<span data-ttu-id="3b39a-108">caseExportOperation</span><span class="sxs-lookup"><span data-stu-id="3b39a-108">caseExportOperation</span></span>](../resources/ediscovery-caseexportoperation.md)
- [<span data-ttu-id="3b39a-109">tagOperation</span><span class="sxs-lookup"><span data-stu-id="3b39a-109">tagOperation</span></span>](../resources/ediscovery-tagoperation.md)
- [<span data-ttu-id="3b39a-110">estimateStatisticsOperation</span><span class="sxs-lookup"><span data-stu-id="3b39a-110">estimateStatisticsOperation</span></span>](../resources/ediscovery-estimatestatisticsoperation.md)

<span data-ttu-id="3b39a-111">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="3b39a-111">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3b39a-112">Methods</span><span class="sxs-lookup"><span data-stu-id="3b39a-112">Methods</span></span>

<span data-ttu-id="3b39a-113">无。</span><span class="sxs-lookup"><span data-stu-id="3b39a-113">None.</span></span>

## <a name="properties"></a><span data-ttu-id="3b39a-114">属性</span><span class="sxs-lookup"><span data-stu-id="3b39a-114">Properties</span></span>

|<span data-ttu-id="3b39a-115">属性</span><span class="sxs-lookup"><span data-stu-id="3b39a-115">Property</span></span>|<span data-ttu-id="3b39a-116">类型</span><span class="sxs-lookup"><span data-stu-id="3b39a-116">Type</span></span>|<span data-ttu-id="3b39a-117">说明</span><span class="sxs-lookup"><span data-stu-id="3b39a-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b39a-118">action</span><span class="sxs-lookup"><span data-stu-id="3b39a-118">action</span></span>|[<span data-ttu-id="3b39a-119">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="3b39a-119">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="3b39a-120">操作表示的操作类型。</span><span class="sxs-lookup"><span data-stu-id="3b39a-120">The type of action the operation represents.</span></span> <span data-ttu-id="3b39a-121">可能的值是： `addToReviewSet` `applyTags` ， ， ， `contentExport` `convertToPdf` ，`estimateStatistics`</span><span class="sxs-lookup"><span data-stu-id="3b39a-121">Possible values are: `addToReviewSet`,`applyTags`,`contentExport`,`convertToPdf`,`estimateStatistics`</span></span>|
|<span data-ttu-id="3b39a-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b39a-122">completedDateTime</span></span>|<span data-ttu-id="3b39a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b39a-123">DateTimeOffset</span></span>| <span data-ttu-id="3b39a-124">操作完成的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3b39a-124">The date and time the operation was completed.</span></span> |
|<span data-ttu-id="3b39a-125">createdBy</span><span class="sxs-lookup"><span data-stu-id="3b39a-125">createdBy</span></span>|[<span data-ttu-id="3b39a-126">identitySet</span><span class="sxs-lookup"><span data-stu-id="3b39a-126">identitySet</span></span>](../resources/identityset.md)| <span data-ttu-id="3b39a-127">创建操作的用户。</span><span class="sxs-lookup"><span data-stu-id="3b39a-127">The user that created the operation.</span></span> |
|<span data-ttu-id="3b39a-128">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b39a-128">createdDateTime</span></span>|<span data-ttu-id="3b39a-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b39a-129">DateTimeOffset</span></span>| <span data-ttu-id="3b39a-130">创建该操作的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3b39a-130">The date and time the operation was created.</span></span> |
|<span data-ttu-id="3b39a-131">id</span><span class="sxs-lookup"><span data-stu-id="3b39a-131">id</span></span>|<span data-ttu-id="3b39a-132">String</span><span class="sxs-lookup"><span data-stu-id="3b39a-132">String</span></span>| <span data-ttu-id="3b39a-133">操作 ID。</span><span class="sxs-lookup"><span data-stu-id="3b39a-133">The ID for the operation.</span></span> <span data-ttu-id="3b39a-134">只读。</span><span class="sxs-lookup"><span data-stu-id="3b39a-134">Read-only.</span></span> |
|<span data-ttu-id="3b39a-135">percentProgress</span><span class="sxs-lookup"><span data-stu-id="3b39a-135">percentProgress</span></span>|<span data-ttu-id="3b39a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="3b39a-136">Int32</span></span>| <span data-ttu-id="3b39a-137">操作的进度。</span><span class="sxs-lookup"><span data-stu-id="3b39a-137">The progress of the operation.</span></span> |
|<span data-ttu-id="3b39a-138">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3b39a-138">resultInfo</span></span>|[<span data-ttu-id="3b39a-139">resultInfo</span><span class="sxs-lookup"><span data-stu-id="3b39a-139">resultInfo</span></span>](../resources/resultinfo.md)| <span data-ttu-id="3b39a-140">包含特定于成功和失败的结果信息。</span><span class="sxs-lookup"><span data-stu-id="3b39a-140">Contains success and failure-specific result information.</span></span> |
|<span data-ttu-id="3b39a-141">status</span><span class="sxs-lookup"><span data-stu-id="3b39a-141">status</span></span>|[<span data-ttu-id="3b39a-142">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="3b39a-142">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)| <span data-ttu-id="3b39a-143">案例操作的状态。</span><span class="sxs-lookup"><span data-stu-id="3b39a-143">The status of the case operation.</span></span> <span data-ttu-id="3b39a-144">可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="3b39a-144">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

### <a name="caseaction-values"></a><span data-ttu-id="3b39a-145">caseAction 值</span><span class="sxs-lookup"><span data-stu-id="3b39a-145">caseAction values</span></span>

|<span data-ttu-id="3b39a-146">成员</span><span class="sxs-lookup"><span data-stu-id="3b39a-146">Member</span></span>|<span data-ttu-id="3b39a-147">说明</span><span class="sxs-lookup"><span data-stu-id="3b39a-147">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="3b39a-148">addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="3b39a-148">addToReviewSet</span></span> | <span data-ttu-id="3b39a-149">此操作表示从电子数据展示集合向审阅集添加数据。</span><span class="sxs-lookup"><span data-stu-id="3b39a-149">The operation represents adding data to a review set from an eDiscovery collection.</span></span> |
| <span data-ttu-id="3b39a-150">applyTags</span><span class="sxs-lookup"><span data-stu-id="3b39a-150">applyTags</span></span> | <span data-ttu-id="3b39a-151">此操作表示指定审阅集查询的审阅集中的批量标记文档。</span><span class="sxs-lookup"><span data-stu-id="3b39a-151">The operation represents bulk tagging documents in a review set for the specified review set query.</span></span> |
| <span data-ttu-id="3b39a-152">contentExport</span><span class="sxs-lookup"><span data-stu-id="3b39a-152">contentExport</span></span> | <span data-ttu-id="3b39a-153">此操作表示从审阅集导出的内容。</span><span class="sxs-lookup"><span data-stu-id="3b39a-153">The operation represents a content export from a review set.</span></span> |
| <span data-ttu-id="3b39a-154">convertToPdf</span><span class="sxs-lookup"><span data-stu-id="3b39a-154">convertToPdf</span></span> | <span data-ttu-id="3b39a-155">此操作表示使用修订将文档转换为 PDF。</span><span class="sxs-lookup"><span data-stu-id="3b39a-155">The operation represents converting documents to PDFs with redactions.</span></span> |
| <span data-ttu-id="3b39a-156">estimateStatistics</span><span class="sxs-lookup"><span data-stu-id="3b39a-156">estimateStatistics</span></span>  | <span data-ttu-id="3b39a-157">此操作表示针对 Microsoft 365 服务（如 Exchange、SharePoint 和 OneDrive for Business）进行搜索。</span><span class="sxs-lookup"><span data-stu-id="3b39a-157">The operation represents searching against Microsoft 365 services such as Exchange, SharePoint, and OneDrive for business.</span></span> |

### <a name="caseoperationstatus-values"></a><span data-ttu-id="3b39a-158">caseOperationStatus 值</span><span class="sxs-lookup"><span data-stu-id="3b39a-158">caseOperationStatus values</span></span>

|<span data-ttu-id="3b39a-159">成员</span><span class="sxs-lookup"><span data-stu-id="3b39a-159">Member</span></span>|<span data-ttu-id="3b39a-160">说明</span><span class="sxs-lookup"><span data-stu-id="3b39a-160">Description</span></span>|
|:----|-----------|
| <span data-ttu-id="3b39a-161">notStarted</span><span class="sxs-lookup"><span data-stu-id="3b39a-161">notStarted</span></span> | <span data-ttu-id="3b39a-162">操作尚未启动。</span><span class="sxs-lookup"><span data-stu-id="3b39a-162">The operation has not yet started.</span></span> |
| <span data-ttu-id="3b39a-163">submissionFailed</span><span class="sxs-lookup"><span data-stu-id="3b39a-163">submissionFailed</span></span> | <span data-ttu-id="3b39a-164">操作提交失败。</span><span class="sxs-lookup"><span data-stu-id="3b39a-164">Submission of the operation failed.</span></span> |
| <span data-ttu-id="3b39a-165">正在运行</span><span class="sxs-lookup"><span data-stu-id="3b39a-165">running</span></span> | <span data-ttu-id="3b39a-166">操作当前正在运行。</span><span class="sxs-lookup"><span data-stu-id="3b39a-166">The operation is currently running.</span></span> |
| <span data-ttu-id="3b39a-167">succeeded</span><span class="sxs-lookup"><span data-stu-id="3b39a-167">succeeded</span></span> | <span data-ttu-id="3b39a-168">操作成功完成，没有任何错误。</span><span class="sxs-lookup"><span data-stu-id="3b39a-168">The operation was successfully completed without any errors.</span></span> |
| <span data-ttu-id="3b39a-169">partiallySucceeded</span><span class="sxs-lookup"><span data-stu-id="3b39a-169">partiallySucceeded</span></span> | <span data-ttu-id="3b39a-170">操作已完成，但出现错误 - 有关错误详细信息，请参阅[resultInfo。](../resources/resultinfo.md)</span><span class="sxs-lookup"><span data-stu-id="3b39a-170">The operation completed, but there were errors - See [resultInfo](../resources/resultinfo.md) for error details.</span></span> |
| <span data-ttu-id="3b39a-171">failed</span><span class="sxs-lookup"><span data-stu-id="3b39a-171">failed</span></span> | <span data-ttu-id="3b39a-172">操作失败 - 有关错误详细信息，请参阅结果信息。</span><span class="sxs-lookup"><span data-stu-id="3b39a-172">The operation failed - See result info for error details.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3b39a-173">关系</span><span class="sxs-lookup"><span data-stu-id="3b39a-173">Relationships</span></span>

<span data-ttu-id="3b39a-174">无。</span><span class="sxs-lookup"><span data-stu-id="3b39a-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b39a-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b39a-175">JSON representation</span></span>

<span data-ttu-id="3b39a-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b39a-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseOperation",
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
