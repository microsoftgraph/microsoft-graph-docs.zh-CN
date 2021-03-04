---
title: dataPolicyOperation 资源类型
description: 表示提交的数据策略操作。 它包含跟踪操作状态的必要信息。 例如，公司管理员可以提交数据策略操作请求以导出员工的公司数据，然后跟踪该请求。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a1d1b1adb9a7de73ecefc6a4290b386d299d784e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440505"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="144a6-105">dataPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="144a6-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="144a6-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="144a6-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="144a6-107">表示提交的数据策略操作。</span><span class="sxs-lookup"><span data-stu-id="144a6-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="144a6-108">它包含跟踪操作状态的必要信息。</span><span class="sxs-lookup"><span data-stu-id="144a6-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="144a6-109">例如，公司管理员可以提交数据策略操作请求以导出员工的公司数据，然后跟踪该请求。</span><span class="sxs-lookup"><span data-stu-id="144a6-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="144a6-110">Methods</span><span class="sxs-lookup"><span data-stu-id="144a6-110">Methods</span></span>

| <span data-ttu-id="144a6-111">方法</span><span class="sxs-lookup"><span data-stu-id="144a6-111">Method</span></span>           | <span data-ttu-id="144a6-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="144a6-112">Return Type</span></span>    |<span data-ttu-id="144a6-113">说明</span><span class="sxs-lookup"><span data-stu-id="144a6-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="144a6-114">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="144a6-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="144a6-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="144a6-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="144a6-116">读取 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="144a6-116">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="144a6-117">属性</span><span class="sxs-lookup"><span data-stu-id="144a6-117">Properties</span></span>

> <span data-ttu-id="144a6-118">**注意：** 此资源的所有属性都是只读的。</span><span class="sxs-lookup"><span data-stu-id="144a6-118">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="144a6-119">属性</span><span class="sxs-lookup"><span data-stu-id="144a6-119">Property</span></span>     | <span data-ttu-id="144a6-120">类型</span><span class="sxs-lookup"><span data-stu-id="144a6-120">Type</span></span>   |<span data-ttu-id="144a6-121">说明</span><span class="sxs-lookup"><span data-stu-id="144a6-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="144a6-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="144a6-122">completedDateTime</span></span>|<span data-ttu-id="144a6-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="144a6-123">DateTimeOffset</span></span>|<span data-ttu-id="144a6-124">表示使用 ISO 8601 格式完成此数据策略操作的请求的时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="144a6-124">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="144a6-125">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="144a6-125">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="144a6-126">Null，直到操作完成。</span><span class="sxs-lookup"><span data-stu-id="144a6-126">Null until the operation completes.</span></span>|
|<span data-ttu-id="144a6-127">id</span><span class="sxs-lookup"><span data-stu-id="144a6-127">id</span></span>|<span data-ttu-id="144a6-128">String</span><span class="sxs-lookup"><span data-stu-id="144a6-128">String</span></span>| <span data-ttu-id="144a6-129">此操作的唯一键。</span><span class="sxs-lookup"><span data-stu-id="144a6-129">Unique key for this operation.</span></span> |
|<span data-ttu-id="144a6-130">状态</span><span class="sxs-lookup"><span data-stu-id="144a6-130">status</span></span>|<span data-ttu-id="144a6-131">string</span><span class="sxs-lookup"><span data-stu-id="144a6-131">string</span></span>| <span data-ttu-id="144a6-132">可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="144a6-132">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="144a6-133">storageLocation</span><span class="sxs-lookup"><span data-stu-id="144a6-133">storageLocation</span></span>|<span data-ttu-id="144a6-134">String</span><span class="sxs-lookup"><span data-stu-id="144a6-134">String</span></span>|<span data-ttu-id="144a6-135">导出数据以用于导出请求的 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="144a6-135">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="144a6-136">userId</span><span class="sxs-lookup"><span data-stu-id="144a6-136">userId</span></span>|<span data-ttu-id="144a6-137">String</span><span class="sxs-lookup"><span data-stu-id="144a6-137">String</span></span>|<span data-ttu-id="144a6-138">要执行该操作的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="144a6-138">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="144a6-139">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="144a6-139">submittedDateTime</span></span>|<span data-ttu-id="144a6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="144a6-140">DateTimeOffset</span></span>|<span data-ttu-id="144a6-141">表示使用 ISO 8601 格式提交此数据操作请求的时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="144a6-141">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="144a6-142">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="144a6-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="144a6-143">progress</span><span class="sxs-lookup"><span data-stu-id="144a6-143">progress</span></span>|<span data-ttu-id="144a6-144">双精度</span><span class="sxs-lookup"><span data-stu-id="144a6-144">Double</span></span>|<span data-ttu-id="144a6-145">指定操作的进度。</span><span class="sxs-lookup"><span data-stu-id="144a6-145">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="144a6-146">关系</span><span class="sxs-lookup"><span data-stu-id="144a6-146">Relationships</span></span>
<span data-ttu-id="144a6-147">无</span><span class="sxs-lookup"><span data-stu-id="144a6-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="144a6-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="144a6-148">JSON representation</span></span>

<span data-ttu-id="144a6-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="144a6-149">Here is a JSON representation of the resource.</span></span>

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


