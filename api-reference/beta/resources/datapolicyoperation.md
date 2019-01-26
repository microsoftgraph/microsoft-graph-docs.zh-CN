---
title: dataPolicyOperation 资源类型
description: 代表提交的数据策略操作。 它包含跟踪操作的状态所需的信息。 例如，公司管理员可以提交数据策略操作请求员工的公司数据导出，然后更高版本跟踪该请求。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4547221c8c1b859d4738a5468603ac6890246263
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570923"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="0dcdc-105">dataPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="0dcdc-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="0dcdc-106">代表提交的数据策略操作。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="0dcdc-107">它包含跟踪操作的状态所需的信息。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="0dcdc-108">例如，公司管理员可以提交数据策略操作请求员工的公司数据导出，然后更高版本跟踪该请求。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="0dcdc-109">方法</span><span class="sxs-lookup"><span data-stu-id="0dcdc-109">Methods</span></span>

| <span data-ttu-id="0dcdc-110">方法</span><span class="sxs-lookup"><span data-stu-id="0dcdc-110">Method</span></span>           | <span data-ttu-id="0dcdc-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="0dcdc-111">Return Type</span></span>    |<span data-ttu-id="0dcdc-112">说明</span><span class="sxs-lookup"><span data-stu-id="0dcdc-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0dcdc-113">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0dcdc-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="0dcdc-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0dcdc-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="0dcdc-115">阅读 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-115">Read properties of the dataPolicyOperation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0dcdc-116">属性</span><span class="sxs-lookup"><span data-stu-id="0dcdc-116">Properties</span></span>

> <span data-ttu-id="0dcdc-117">**注意：** 此资源的所有属性都是只读的。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-117">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="0dcdc-118">属性</span><span class="sxs-lookup"><span data-stu-id="0dcdc-118">Property</span></span>     | <span data-ttu-id="0dcdc-119">类型</span><span class="sxs-lookup"><span data-stu-id="0dcdc-119">Type</span></span>   |<span data-ttu-id="0dcdc-120">说明</span><span class="sxs-lookup"><span data-stu-id="0dcdc-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0dcdc-121">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0dcdc-121">completedDateTime</span></span>|<span data-ttu-id="0dcdc-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dcdc-122">DateTimeOffset</span></span>|<span data-ttu-id="0dcdc-123">表示此数据策略操作的请求完成时，在 UTC 时间中，使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-123">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="0dcdc-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0dcdc-125">在操作完成前，则为 null。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-125">Null until the operation completes.</span></span>|
|<span data-ttu-id="0dcdc-126">id</span><span class="sxs-lookup"><span data-stu-id="0dcdc-126">id</span></span>|<span data-ttu-id="0dcdc-127">String</span><span class="sxs-lookup"><span data-stu-id="0dcdc-127">String</span></span>| <span data-ttu-id="0dcdc-128">此操作的唯一键。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-128">Unique key for this operation.</span></span> |
|<span data-ttu-id="0dcdc-129">status</span><span class="sxs-lookup"><span data-stu-id="0dcdc-129">status</span></span>|<span data-ttu-id="0dcdc-130">string</span><span class="sxs-lookup"><span data-stu-id="0dcdc-130">string</span></span>| <span data-ttu-id="0dcdc-131">可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-131">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0dcdc-132">storageLocation</span><span class="sxs-lookup"><span data-stu-id="0dcdc-132">storageLocation</span></span>|<span data-ttu-id="0dcdc-133">String</span><span class="sxs-lookup"><span data-stu-id="0dcdc-133">String</span></span>|<span data-ttu-id="0dcdc-134">到要从中导出数据的导出请求的 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-134">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="0dcdc-135">userId</span><span class="sxs-lookup"><span data-stu-id="0dcdc-135">userId</span></span>|<span data-ttu-id="0dcdc-136">String</span><span class="sxs-lookup"><span data-stu-id="0dcdc-136">String</span></span>|<span data-ttu-id="0dcdc-137">在其执行操作的用户 id。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-137">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="0dcdc-138">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="0dcdc-138">submittedDateTime</span></span>|<span data-ttu-id="0dcdc-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dcdc-139">DateTimeOffset</span></span>|<span data-ttu-id="0dcdc-140">表示此数据操作的请求已提交时，在 UTC 时间中，使用 ISO 8601 格式。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-140">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="0dcdc-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0dcdc-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dcdc-142">关系</span><span class="sxs-lookup"><span data-stu-id="0dcdc-142">Relationships</span></span>
<span data-ttu-id="0dcdc-143">无</span><span class="sxs-lookup"><span data-stu-id="0dcdc-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0dcdc-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0dcdc-144">JSON representation</span></span>

<span data-ttu-id="0dcdc-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0dcdc-145">Here is a JSON representation of the resource.</span></span>

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
  "submittedDateTime": "String (timestamp)"
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
