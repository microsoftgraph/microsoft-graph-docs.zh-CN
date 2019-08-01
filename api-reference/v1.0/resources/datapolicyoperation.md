---
title: dataPolicyOperation 资源类型
description: 表示已提交的数据策略操作。 它包含用于跟踪操作状态的必要信息。 例如, 公司管理员可以提交数据策略操作请求以导出员工的公司数据, 然后再跟踪该请求。
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c73bef8a640c950b6d85eb74ad93089aaad4f74
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029552"
---
# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="97db7-105">dataPolicyOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="97db7-105">dataPolicyOperation resource type</span></span>

<span data-ttu-id="97db7-106">表示已提交的数据策略操作。</span><span class="sxs-lookup"><span data-stu-id="97db7-106">Represents a submitted data policy operation.</span></span> <span data-ttu-id="97db7-107">它包含用于跟踪操作状态的必要信息。</span><span class="sxs-lookup"><span data-stu-id="97db7-107">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="97db7-108">例如, 公司管理员可以提交数据策略操作请求以导出员工的公司数据, 然后再跟踪该请求。</span><span class="sxs-lookup"><span data-stu-id="97db7-108">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="97db7-109">方法</span><span class="sxs-lookup"><span data-stu-id="97db7-109">Methods</span></span>

| <span data-ttu-id="97db7-110">方法</span><span class="sxs-lookup"><span data-stu-id="97db7-110">Method</span></span>           | <span data-ttu-id="97db7-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="97db7-111">Return Type</span></span>    |<span data-ttu-id="97db7-112">说明</span><span class="sxs-lookup"><span data-stu-id="97db7-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97db7-113">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="97db7-113">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="97db7-114">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="97db7-114">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="97db7-115">检索**dataPolicyOperation**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="97db7-115">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="97db7-116">导出个人数据</span><span class="sxs-lookup"><span data-stu-id="97db7-116">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="97db7-117">无</span><span class="sxs-lookup"><span data-stu-id="97db7-117">None</span></span> |<span data-ttu-id="97db7-118">提交数据策略操作请求以导出可稍后使用[Get dataPolicyOperation](../api/datapolicyoperation-get.md)读取的组织用户的数据。</span><span class="sxs-lookup"><span data-stu-id="97db7-118">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="97db7-119">属性</span><span class="sxs-lookup"><span data-stu-id="97db7-119">Properties</span></span>

> <span data-ttu-id="97db7-120">**注意:** 此资源的所有属性都是只读的。</span><span class="sxs-lookup"><span data-stu-id="97db7-120">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="97db7-121">属性</span><span class="sxs-lookup"><span data-stu-id="97db7-121">Property</span></span>     | <span data-ttu-id="97db7-122">类型</span><span class="sxs-lookup"><span data-stu-id="97db7-122">Type</span></span>   |<span data-ttu-id="97db7-123">说明</span><span class="sxs-lookup"><span data-stu-id="97db7-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97db7-124">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="97db7-124">completedDateTime</span></span>|<span data-ttu-id="97db7-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97db7-125">DateTimeOffset</span></span>|<span data-ttu-id="97db7-126">表示在 UTC 时间内使用 ISO 8601 格式完成此数据策略操作的请求的时间。</span><span class="sxs-lookup"><span data-stu-id="97db7-126">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="97db7-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="97db7-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="97db7-128">空, 直到操作完成。</span><span class="sxs-lookup"><span data-stu-id="97db7-128">Null until the operation completes.</span></span>|
|<span data-ttu-id="97db7-129">id</span><span class="sxs-lookup"><span data-stu-id="97db7-129">id</span></span>|<span data-ttu-id="97db7-130">String</span><span class="sxs-lookup"><span data-stu-id="97db7-130">String</span></span>| <span data-ttu-id="97db7-131">此操作的唯一键。</span><span class="sxs-lookup"><span data-stu-id="97db7-131">Unique key for this operation.</span></span> |
|<span data-ttu-id="97db7-132">状态</span><span class="sxs-lookup"><span data-stu-id="97db7-132">status</span></span>|<span data-ttu-id="97db7-133">string</span><span class="sxs-lookup"><span data-stu-id="97db7-133">string</span></span>| <span data-ttu-id="97db7-134">可取值为：`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="97db7-134">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="97db7-135">storageLocation</span><span class="sxs-lookup"><span data-stu-id="97db7-135">storageLocation</span></span>|<span data-ttu-id="97db7-136">String</span><span class="sxs-lookup"><span data-stu-id="97db7-136">String</span></span>|<span data-ttu-id="97db7-137">要为导出请求导出的数据的 URL 位置。</span><span class="sxs-lookup"><span data-stu-id="97db7-137">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="97db7-138">userId</span><span class="sxs-lookup"><span data-stu-id="97db7-138">userId</span></span>|<span data-ttu-id="97db7-139">String</span><span class="sxs-lookup"><span data-stu-id="97db7-139">String</span></span>|<span data-ttu-id="97db7-140">对其执行操作的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="97db7-140">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="97db7-141">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="97db7-141">submittedDateTime</span></span>|<span data-ttu-id="97db7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97db7-142">DateTimeOffset</span></span>|<span data-ttu-id="97db7-143">表示在 UTC 时间内提交此数据操作的请求 (使用 ISO 8601 格式)。</span><span class="sxs-lookup"><span data-stu-id="97db7-143">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="97db7-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="97db7-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="97db7-145">progress</span><span class="sxs-lookup"><span data-stu-id="97db7-145">progress</span></span>|<span data-ttu-id="97db7-146">String</span><span class="sxs-lookup"><span data-stu-id="97db7-146">String</span></span>|<span data-ttu-id="97db7-147">指定操作的进度。</span><span class="sxs-lookup"><span data-stu-id="97db7-147">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97db7-148">关系</span><span class="sxs-lookup"><span data-stu-id="97db7-148">Relationships</span></span>
<span data-ttu-id="97db7-149">无。</span><span class="sxs-lookup"><span data-stu-id="97db7-149">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="97db7-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97db7-150">JSON representation</span></span>

<span data-ttu-id="97db7-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97db7-151">The following is a JSON representation of the resource.</span></span>

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
