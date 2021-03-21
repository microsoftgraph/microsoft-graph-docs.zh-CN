---
title: dataPolicyOperation 资源类型
description: 表示提交的数据策略操作。 它包含跟踪操作状态的必要信息。 例如，公司管理员可以提交数据策略操作请求以导出员工的公司数据，然后跟踪该请求。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f12d83ace221a64754e4227ff292e780abf7ea82
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962628"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="1392c-105">dataPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="1392c-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="1392c-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1392c-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1392c-107">表示提交的数据策略操作。</span><span class="sxs-lookup"><span data-stu-id="1392c-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="1392c-108">它包含跟踪操作状态的必要信息。</span><span class="sxs-lookup"><span data-stu-id="1392c-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="1392c-109">例如，公司管理员可以提交数据策略操作请求以导出员工的公司数据，然后跟踪该请求。</span><span class="sxs-lookup"><span data-stu-id="1392c-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="1392c-110">Methods</span><span class="sxs-lookup"><span data-stu-id="1392c-110">Methods</span></span>

| <span data-ttu-id="1392c-111">方法</span><span class="sxs-lookup"><span data-stu-id="1392c-111">Method</span></span>           | <span data-ttu-id="1392c-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="1392c-112">Return Type</span></span>    |<span data-ttu-id="1392c-113">说明</span><span class="sxs-lookup"><span data-stu-id="1392c-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1392c-114">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="1392c-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="1392c-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="1392c-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="1392c-116">读取 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1392c-116">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1392c-117">属性</span><span class="sxs-lookup"><span data-stu-id="1392c-117">Properties</span></span>

> <span data-ttu-id="1392c-118">**注意：** 此资源的所有属性都是只读的。</span><span class="sxs-lookup"><span data-stu-id="1392c-118">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="1392c-119">属性</span><span class="sxs-lookup"><span data-stu-id="1392c-119">Property</span></span>     | <span data-ttu-id="1392c-120">类型</span><span class="sxs-lookup"><span data-stu-id="1392c-120">Type</span></span>   |<span data-ttu-id="1392c-121">说明</span><span class="sxs-lookup"><span data-stu-id="1392c-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1392c-122">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="1392c-122">completedDateTime</span></span>|<span data-ttu-id="1392c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1392c-123">DateTimeOffset</span></span>|<span data-ttu-id="1392c-124">表示此数据策略操作的请求使用 ISO 8601 格式以 UTC 时间完成的时间。</span><span class="sxs-lookup"><span data-stu-id="1392c-124">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="1392c-125">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="1392c-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="1392c-126">Null，直到操作完成。</span><span class="sxs-lookup"><span data-stu-id="1392c-126">Null until the operation completes.</span></span>|
|<span data-ttu-id="1392c-127">id</span><span class="sxs-lookup"><span data-stu-id="1392c-127">id</span></span>|<span data-ttu-id="1392c-128">String</span><span class="sxs-lookup"><span data-stu-id="1392c-128">String</span></span>| <span data-ttu-id="1392c-129">此操作的唯一键。</span><span class="sxs-lookup"><span data-stu-id="1392c-129">Unique key for this operation.</span></span> |
|<span data-ttu-id="1392c-130">状态</span><span class="sxs-lookup"><span data-stu-id="1392c-130">status</span></span>|<span data-ttu-id="1392c-131">dataPolicyOperationStatus</span><span class="sxs-lookup"><span data-stu-id="1392c-131">dataPolicyOperationStatus</span></span>| <span data-ttu-id="1392c-132">可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1392c-132">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1392c-133">storageLocation</span><span class="sxs-lookup"><span data-stu-id="1392c-133">storageLocation</span></span>|<span data-ttu-id="1392c-134">String</span><span class="sxs-lookup"><span data-stu-id="1392c-134">String</span></span>|<span data-ttu-id="1392c-135">导出请求将数据导出到的 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="1392c-135">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="1392c-136">userId</span><span class="sxs-lookup"><span data-stu-id="1392c-136">userId</span></span>|<span data-ttu-id="1392c-137">String</span><span class="sxs-lookup"><span data-stu-id="1392c-137">String</span></span>|<span data-ttu-id="1392c-138">操作所针对的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="1392c-138">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="1392c-139">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="1392c-139">submittedDateTime</span></span>|<span data-ttu-id="1392c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1392c-140">DateTimeOffset</span></span>|<span data-ttu-id="1392c-141">表示使用 ISO 8601 格式提交此数据操作请求的时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="1392c-141">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="1392c-142">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="1392c-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="1392c-143">progress</span><span class="sxs-lookup"><span data-stu-id="1392c-143">progress</span></span>|<span data-ttu-id="1392c-144">双精度</span><span class="sxs-lookup"><span data-stu-id="1392c-144">Double</span></span>|<span data-ttu-id="1392c-145">指定操作的进度。</span><span class="sxs-lookup"><span data-stu-id="1392c-145">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1392c-146">关系</span><span class="sxs-lookup"><span data-stu-id="1392c-146">Relationships</span></span>
<span data-ttu-id="1392c-147">无</span><span class="sxs-lookup"><span data-stu-id="1392c-147">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1392c-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1392c-148">JSON representation</span></span>

<span data-ttu-id="1392c-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1392c-149">Here is a JSON representation of the resource.</span></span>

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


