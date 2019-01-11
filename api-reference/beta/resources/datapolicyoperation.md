---
title: dataPolicyOperation 资源类型
description: 代表提交的数据策略操作。 它包含跟踪操作的状态所需的信息。 例如，公司管理员可以提交数据策略操作请求员工的公司数据导出，然后更高版本跟踪该请求。
localization_priority: Normal
ms.openlocfilehash: b56cfe766bbfcae9339805dd61ce816e372d02f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876004"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="3c972-105">dataPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c972-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="3c972-106">代表提交的数据策略操作。</span><span class="sxs-lookup"><span data-stu-id="3c972-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="3c972-107">它包含跟踪操作的状态所需的信息。</span><span class="sxs-lookup"><span data-stu-id="3c972-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="3c972-108">例如，公司管理员可以提交数据策略操作请求员工的公司数据导出，然后更高版本跟踪该请求。</span><span class="sxs-lookup"><span data-stu-id="3c972-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="3c972-109">方法</span><span class="sxs-lookup"><span data-stu-id="3c972-109">Methods</span></span>

| <span data-ttu-id="3c972-110">方法</span><span class="sxs-lookup"><span data-stu-id="3c972-110">Method</span></span>           | <span data-ttu-id="3c972-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3c972-111">Return Type</span></span>    |<span data-ttu-id="3c972-112">说明</span><span class="sxs-lookup"><span data-stu-id="3c972-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c972-113">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="3c972-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="3c972-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="3c972-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="3c972-115">阅读 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3c972-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c972-116">属性</span><span class="sxs-lookup"><span data-stu-id="3c972-116">Properties</span></span>

> <span data-ttu-id="3c972-117">**注意：** 此资源的所有属性都是只读的。</span><span class="sxs-lookup"><span data-stu-id="3c972-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="3c972-118">属性</span><span class="sxs-lookup"><span data-stu-id="3c972-118">Property</span></span>     | <span data-ttu-id="3c972-119">类型</span><span class="sxs-lookup"><span data-stu-id="3c972-119">Type</span></span>   |<span data-ttu-id="3c972-120">说明</span><span class="sxs-lookup"><span data-stu-id="3c972-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c972-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c972-121">completedDateTime</span></span>|<span data-ttu-id="3c972-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c972-122">DateTimeOffset</span></span>|<span data-ttu-id="3c972-123">表示此数据策略操作的请求完成时，在 UTC 时间中，使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="3c972-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="3c972-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="3c972-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3c972-125">在操作完成前，则为 null。</span><span class="sxs-lookup"><span data-stu-id="3c972-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="3c972-126">id</span><span class="sxs-lookup"><span data-stu-id="3c972-126">id</span></span>|<span data-ttu-id="3c972-127">字符串</span><span class="sxs-lookup"><span data-stu-id="3c972-127">String</span></span>| <span data-ttu-id="3c972-128">此操作的唯一键。</span><span class="sxs-lookup"><span data-stu-id="3c972-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="3c972-129">status</span><span class="sxs-lookup"><span data-stu-id="3c972-129">status</span></span>|<span data-ttu-id="3c972-130">string</span><span class="sxs-lookup"><span data-stu-id="3c972-130">string</span></span>| <span data-ttu-id="3c972-131">可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3c972-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3c972-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="3c972-132">storageLocation</span></span>|<span data-ttu-id="3c972-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3c972-133">String</span></span>|<span data-ttu-id="3c972-134">到要从中导出数据的导出请求的 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="3c972-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="3c972-135">userId</span><span class="sxs-lookup"><span data-stu-id="3c972-135">userId</span></span>|<span data-ttu-id="3c972-136">String</span><span class="sxs-lookup"><span data-stu-id="3c972-136">String</span></span>|<span data-ttu-id="3c972-137">在其执行操作的用户 id。</span><span class="sxs-lookup"><span data-stu-id="3c972-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="3c972-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c972-138">submittedDateTime</span></span>|<span data-ttu-id="3c972-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c972-139">DateTimeOffset</span></span>|<span data-ttu-id="3c972-140">表示此数据操作的请求已提交时，在 UTC 时间中，使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="3c972-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="3c972-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3c972-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3c972-142">进度</span><span class="sxs-lookup"><span data-stu-id="3c972-142">progress</span></span>|<span data-ttu-id="3c972-143">Double</span><span class="sxs-lookup"><span data-stu-id="3c972-143">Double</span></span>|<span data-ttu-id="3c972-144">指定操作的进度。</span><span class="sxs-lookup"><span data-stu-id="3c972-144">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c972-145">Relationships</span><span class="sxs-lookup"><span data-stu-id="3c972-145">Relationships</span></span>
<span data-ttu-id="3c972-146">无</span><span class="sxs-lookup"><span data-stu-id="3c972-146">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3c972-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c972-147">JSON representation</span></span>

<span data-ttu-id="3c972-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c972-148">Here is a JSON representation of the resource.</span></span>

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
