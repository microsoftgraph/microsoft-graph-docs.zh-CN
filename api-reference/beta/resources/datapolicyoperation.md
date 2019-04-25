---
title: dataPolicyOperation 资源类型
description: 表示已提交的数据策略操作。 它包含用于跟踪操作状态的必要信息。 例如, 公司管理员可以提交数据策略操作请求以导出员工的公司数据, 然后再跟踪该请求。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d3ec392bb30614346d2726262851eebc29ee779
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543175"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="d4fd7-105">dataPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4fd7-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="d4fd7-106">表示已提交的数据策略操作。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="d4fd7-107">它包含用于跟踪操作状态的必要信息。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="d4fd7-108">例如, 公司管理员可以提交数据策略操作请求以导出员工的公司数据, 然后再跟踪该请求。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="d4fd7-109">方法</span><span class="sxs-lookup"><span data-stu-id="d4fd7-109">Methods</span></span>

| <span data-ttu-id="d4fd7-110">方法</span><span class="sxs-lookup"><span data-stu-id="d4fd7-110">Method</span></span>           | <span data-ttu-id="d4fd7-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4fd7-111">Return Type</span></span>    |<span data-ttu-id="d4fd7-112">说明</span><span class="sxs-lookup"><span data-stu-id="d4fd7-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4fd7-113">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d4fd7-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="d4fd7-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d4fd7-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="d4fd7-115">读取 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4fd7-116">属性</span><span class="sxs-lookup"><span data-stu-id="d4fd7-116">Properties</span></span>

> <span data-ttu-id="d4fd7-117">**注意:** 此资源的所有属性都是只读的。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="d4fd7-118">属性</span><span class="sxs-lookup"><span data-stu-id="d4fd7-118">Property</span></span>     | <span data-ttu-id="d4fd7-119">类型</span><span class="sxs-lookup"><span data-stu-id="d4fd7-119">Type</span></span>   |<span data-ttu-id="d4fd7-120">说明</span><span class="sxs-lookup"><span data-stu-id="d4fd7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4fd7-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4fd7-121">completedDateTime</span></span>|<span data-ttu-id="d4fd7-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4fd7-122">DateTimeOffset</span></span>|<span data-ttu-id="d4fd7-123">表示在 UTC 时间内使用 ISO 8601 格式完成此数据策略操作的请求的时间。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="d4fd7-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d4fd7-125">空, 直到操作完成。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="d4fd7-126">id</span><span class="sxs-lookup"><span data-stu-id="d4fd7-126">id</span></span>|<span data-ttu-id="d4fd7-127">String</span><span class="sxs-lookup"><span data-stu-id="d4fd7-127">String</span></span>| <span data-ttu-id="d4fd7-128">此操作的唯一键。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="d4fd7-129">status</span><span class="sxs-lookup"><span data-stu-id="d4fd7-129">status</span></span>|<span data-ttu-id="d4fd7-130">string</span><span class="sxs-lookup"><span data-stu-id="d4fd7-130">string</span></span>| <span data-ttu-id="d4fd7-131">可取值为：`notStarted`、`running`、`complete`、`failed` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d4fd7-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="d4fd7-132">storageLocation</span></span>|<span data-ttu-id="d4fd7-133">String</span><span class="sxs-lookup"><span data-stu-id="d4fd7-133">String</span></span>|<span data-ttu-id="d4fd7-134">要为导出请求导出的数据的 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="d4fd7-135">userId</span><span class="sxs-lookup"><span data-stu-id="d4fd7-135">userId</span></span>|<span data-ttu-id="d4fd7-136">String</span><span class="sxs-lookup"><span data-stu-id="d4fd7-136">String</span></span>|<span data-ttu-id="d4fd7-137">对其执行操作的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="d4fd7-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4fd7-138">submittedDateTime</span></span>|<span data-ttu-id="d4fd7-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4fd7-139">DateTimeOffset</span></span>|<span data-ttu-id="d4fd7-140">表示在 UTC 时间内提交此数据操作的请求 (使用 ISO 8601 格式)。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="d4fd7-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d4fd7-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d4fd7-142">progress</span><span class="sxs-lookup"><span data-stu-id="d4fd7-142">progress</span></span>|<span data-ttu-id="d4fd7-143">双精度</span><span class="sxs-lookup"><span data-stu-id="d4fd7-143">Double</span></span>|<span data-ttu-id="d4fd7-144">指定操作的进度。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4fd7-145">关系</span><span class="sxs-lookup"><span data-stu-id="d4fd7-145">Relationships</span></span>
<span data-ttu-id="d4fd7-146">无</span><span class="sxs-lookup"><span data-stu-id="d4fd7-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d4fd7-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4fd7-147">JSON representation</span></span>

<span data-ttu-id="d4fd7-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4fd7-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
