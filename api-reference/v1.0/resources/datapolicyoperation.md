---
title: dataPolicyOperation 资源类型
description: 表示提交的数据策略操作。 它包含跟踪操作状态的必要信息。 例如，公司管理员可以提交数据策略操作请求以导出员工的公司数据，然后跟踪该请求。
author: dkershaw10
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 18294905754cd962ec1c18136b61ca20799eee3d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718441"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="e8c6d-105">dataPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8c6d-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="e8c6d-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8c6d-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e8c6d-107">表示提交的数据策略操作。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-107">Represents a submitted data policy operation.</span></span> <span data-ttu-id="e8c6d-108">它包含跟踪操作状态的必要信息。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-108">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="e8c6d-109">例如，公司管理员可以提交数据策略操作请求以导出员工的公司数据，然后跟踪该请求。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-109">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="e8c6d-110">Methods</span><span class="sxs-lookup"><span data-stu-id="e8c6d-110">Methods</span></span>

| <span data-ttu-id="e8c6d-111">方法</span><span class="sxs-lookup"><span data-stu-id="e8c6d-111">Method</span></span>           | <span data-ttu-id="e8c6d-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="e8c6d-112">Return Type</span></span>    |<span data-ttu-id="e8c6d-113">说明</span><span class="sxs-lookup"><span data-stu-id="e8c6d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e8c6d-114">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="e8c6d-114">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="e8c6d-115">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="e8c6d-115">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="e8c6d-116">检索 **dataPolicyOperation 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-116">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="e8c6d-117">导出个人数据</span><span class="sxs-lookup"><span data-stu-id="e8c6d-117">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="e8c6d-118">无</span><span class="sxs-lookup"><span data-stu-id="e8c6d-118">None</span></span> |<span data-ttu-id="e8c6d-119">提交数据策略操作请求以导出组织用户的数据，稍后可以使用[Get dataPolicyOperation](../api/datapolicyoperation-get.md)读取该数据</span><span class="sxs-lookup"><span data-stu-id="e8c6d-119">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="e8c6d-120">属性</span><span class="sxs-lookup"><span data-stu-id="e8c6d-120">Properties</span></span>

> <span data-ttu-id="e8c6d-121">**注意：** 此资源的所有属性都是只读的。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-121">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="e8c6d-122">属性</span><span class="sxs-lookup"><span data-stu-id="e8c6d-122">Property</span></span>     | <span data-ttu-id="e8c6d-123">类型</span><span class="sxs-lookup"><span data-stu-id="e8c6d-123">Type</span></span>   |<span data-ttu-id="e8c6d-124">说明</span><span class="sxs-lookup"><span data-stu-id="e8c6d-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8c6d-125">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8c6d-125">completedDateTime</span></span>|<span data-ttu-id="e8c6d-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8c6d-126">DateTimeOffset</span></span>|<span data-ttu-id="e8c6d-127">表示此数据策略操作的请求使用 ISO 8601 格式以 UTC 时间完成的时间。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-127">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="e8c6d-128">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="e8c6d-129">Null，直到操作完成。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-129">Null until the operation completes.</span></span>|
|<span data-ttu-id="e8c6d-130">id</span><span class="sxs-lookup"><span data-stu-id="e8c6d-130">id</span></span>|<span data-ttu-id="e8c6d-131">字符串</span><span class="sxs-lookup"><span data-stu-id="e8c6d-131">String</span></span>| <span data-ttu-id="e8c6d-132">此操作的唯一键。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-132">Unique key for this operation.</span></span> |
|<span data-ttu-id="e8c6d-133">状态</span><span class="sxs-lookup"><span data-stu-id="e8c6d-133">status</span></span>|<span data-ttu-id="e8c6d-134">string</span><span class="sxs-lookup"><span data-stu-id="e8c6d-134">string</span></span>| <span data-ttu-id="e8c6d-135">可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-135">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e8c6d-136">storageLocation</span><span class="sxs-lookup"><span data-stu-id="e8c6d-136">storageLocation</span></span>|<span data-ttu-id="e8c6d-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e8c6d-137">String</span></span>|<span data-ttu-id="e8c6d-138">导出请求将数据导出到的 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-138">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="e8c6d-139">userId</span><span class="sxs-lookup"><span data-stu-id="e8c6d-139">userId</span></span>|<span data-ttu-id="e8c6d-140">字符串</span><span class="sxs-lookup"><span data-stu-id="e8c6d-140">String</span></span>|<span data-ttu-id="e8c6d-141">操作所针对的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-141">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="e8c6d-142">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8c6d-142">submittedDateTime</span></span>|<span data-ttu-id="e8c6d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8c6d-143">DateTimeOffset</span></span>|<span data-ttu-id="e8c6d-144">表示使用 ISO 8601 格式提交此数据操作请求的时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-144">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="e8c6d-145">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="e8c6d-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e8c6d-146">progress</span><span class="sxs-lookup"><span data-stu-id="e8c6d-146">progress</span></span>|<span data-ttu-id="e8c6d-147">字符串</span><span class="sxs-lookup"><span data-stu-id="e8c6d-147">String</span></span>|<span data-ttu-id="e8c6d-148">指定操作的进度。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-148">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8c6d-149">关系</span><span class="sxs-lookup"><span data-stu-id="e8c6d-149">Relationships</span></span>
<span data-ttu-id="e8c6d-150">无。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-150">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e8c6d-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8c6d-151">JSON representation</span></span>

<span data-ttu-id="e8c6d-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8c6d-152">The following is a JSON representation of the resource.</span></span>

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
  "progress": "String (double)"
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

