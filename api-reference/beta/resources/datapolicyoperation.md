---
title: dataPolicyOperation 资源类型
description: 表示已提交的数据策略操作。 它包含用于跟踪操作状态的必要信息。 例如, 公司管理员可以提交数据策略操作请求以导出员工的公司数据, 然后再跟踪该请求。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 07c708ac2d46e23cc4bdcea233587c910d30fc3e
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657712"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="c2a06-105">dataPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2a06-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="c2a06-106">表示已提交的数据策略操作。</span><span class="sxs-lookup"><span data-stu-id="c2a06-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="c2a06-107">它包含用于跟踪操作状态的必要信息。</span><span class="sxs-lookup"><span data-stu-id="c2a06-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="c2a06-108">例如, 公司管理员可以提交数据策略操作请求以导出员工的公司数据, 然后再跟踪该请求。</span><span class="sxs-lookup"><span data-stu-id="c2a06-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="c2a06-109">方法</span><span class="sxs-lookup"><span data-stu-id="c2a06-109">Methods</span></span>

| <span data-ttu-id="c2a06-110">方法</span><span class="sxs-lookup"><span data-stu-id="c2a06-110">Method</span></span>           | <span data-ttu-id="c2a06-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="c2a06-111">Return Type</span></span>    |<span data-ttu-id="c2a06-112">说明</span><span class="sxs-lookup"><span data-stu-id="c2a06-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2a06-113">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="c2a06-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="c2a06-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="c2a06-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="c2a06-115">读取 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c2a06-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2a06-116">属性</span><span class="sxs-lookup"><span data-stu-id="c2a06-116">Properties</span></span>

> <span data-ttu-id="c2a06-117">**注意:** 此资源的所有属性都是只读的。</span><span class="sxs-lookup"><span data-stu-id="c2a06-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="c2a06-118">属性</span><span class="sxs-lookup"><span data-stu-id="c2a06-118">Property</span></span>     | <span data-ttu-id="c2a06-119">类型</span><span class="sxs-lookup"><span data-stu-id="c2a06-119">Type</span></span>   |<span data-ttu-id="c2a06-120">说明</span><span class="sxs-lookup"><span data-stu-id="c2a06-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2a06-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2a06-121">completedDateTime</span></span>|<span data-ttu-id="c2a06-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2a06-122">DateTimeOffset</span></span>|<span data-ttu-id="c2a06-123">表示在 UTC 时间内使用 ISO 8601 格式完成此数据策略操作的请求的时间。</span><span class="sxs-lookup"><span data-stu-id="c2a06-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="c2a06-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="c2a06-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c2a06-125">空, 直到操作完成。</span><span class="sxs-lookup"><span data-stu-id="c2a06-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="c2a06-126">id</span><span class="sxs-lookup"><span data-stu-id="c2a06-126">id</span></span>|<span data-ttu-id="c2a06-127">String</span><span class="sxs-lookup"><span data-stu-id="c2a06-127">String</span></span>| <span data-ttu-id="c2a06-128">此操作的唯一键。</span><span class="sxs-lookup"><span data-stu-id="c2a06-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="c2a06-129">状态</span><span class="sxs-lookup"><span data-stu-id="c2a06-129">status</span></span>|<span data-ttu-id="c2a06-130">string</span><span class="sxs-lookup"><span data-stu-id="c2a06-130">string</span></span>| <span data-ttu-id="c2a06-131">可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c2a06-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c2a06-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="c2a06-132">storageLocation</span></span>|<span data-ttu-id="c2a06-133">String</span><span class="sxs-lookup"><span data-stu-id="c2a06-133">String</span></span>|<span data-ttu-id="c2a06-134">要为导出请求导出的数据的 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="c2a06-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="c2a06-135">userId</span><span class="sxs-lookup"><span data-stu-id="c2a06-135">userId</span></span>|<span data-ttu-id="c2a06-136">String</span><span class="sxs-lookup"><span data-stu-id="c2a06-136">String</span></span>|<span data-ttu-id="c2a06-137">对其执行操作的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="c2a06-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="c2a06-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2a06-138">submittedDateTime</span></span>|<span data-ttu-id="c2a06-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2a06-139">DateTimeOffset</span></span>|<span data-ttu-id="c2a06-140">表示在 UTC 时间内提交此数据操作的请求 (使用 ISO 8601 格式)。</span><span class="sxs-lookup"><span data-stu-id="c2a06-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="c2a06-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c2a06-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c2a06-142">progress</span><span class="sxs-lookup"><span data-stu-id="c2a06-142">progress</span></span>|<span data-ttu-id="c2a06-143">双精度</span><span class="sxs-lookup"><span data-stu-id="c2a06-143">Double</span></span>|<span data-ttu-id="c2a06-144">指定操作的进度。</span><span class="sxs-lookup"><span data-stu-id="c2a06-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2a06-145">关系</span><span class="sxs-lookup"><span data-stu-id="c2a06-145">Relationships</span></span>
<span data-ttu-id="c2a06-146">无</span><span class="sxs-lookup"><span data-stu-id="c2a06-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c2a06-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2a06-147">JSON representation</span></span>

<span data-ttu-id="c2a06-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2a06-148">Here is a JSON representation of the resource.</span></span>

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
