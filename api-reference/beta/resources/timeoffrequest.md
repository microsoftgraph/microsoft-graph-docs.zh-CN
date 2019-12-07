---
title: timeOffRequest 资源类型
description: 表示要采用 timeoff 的班次请求的类型。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 28be6904b64b89c6386bd25a4ced71f76fdc4088
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895620"
---
# <a name="timeoffrequest-resource-type"></a><span data-ttu-id="b8202-103">timeOffRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8202-103">timeOffRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8202-104">表示要采用[timeoff](../resources/timeoff.md)的班次请求的类型。</span><span class="sxs-lookup"><span data-stu-id="b8202-104">Represents a type of shift request to take [timeoff](../resources/timeoff.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b8202-105">方法</span><span class="sxs-lookup"><span data-stu-id="b8202-105">Methods</span></span>

| <span data-ttu-id="b8202-106">方法</span><span class="sxs-lookup"><span data-stu-id="b8202-106">Method</span></span>       | <span data-ttu-id="b8202-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b8202-107">Return Type</span></span> | <span data-ttu-id="b8202-108">说明</span><span class="sxs-lookup"><span data-stu-id="b8202-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b8202-109">获取</span><span class="sxs-lookup"><span data-stu-id="b8202-109">Get</span></span>](../api/timeoffrequest-get.md) | [<span data-ttu-id="b8202-110">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="b8202-110">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="b8202-111">读取**timeOffRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b8202-111">Read the properties and relationships of a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="b8202-112">更新</span><span class="sxs-lookup"><span data-stu-id="b8202-112">Update</span></span>](../api/timeoffrequest-update.md) | [<span data-ttu-id="b8202-113">timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="b8202-113">timeOffRequest</span></span>](timeoffrequest.md) | <span data-ttu-id="b8202-114">更新**timeOffRequest**对象。</span><span class="sxs-lookup"><span data-stu-id="b8202-114">Update a **timeOffRequest** object.</span></span> |
| [<span data-ttu-id="b8202-115">删除</span><span class="sxs-lookup"><span data-stu-id="b8202-115">Delete</span></span>](../api/timeoffrequest-delete.md) | <span data-ttu-id="b8202-116">None</span><span class="sxs-lookup"><span data-stu-id="b8202-116">None</span></span> | <span data-ttu-id="b8202-117">删除**timeOffRequest**对象。</span><span class="sxs-lookup"><span data-stu-id="b8202-117">Delete a **timeOffRequest** object.</span></span> |
|[<span data-ttu-id="b8202-118">批准</span><span class="sxs-lookup"><span data-stu-id="b8202-118">Approve</span></span>](../api/timeoffrequest-approve.md)|<span data-ttu-id="b8202-119">None</span><span class="sxs-lookup"><span data-stu-id="b8202-119">None</span></span>|<span data-ttu-id="b8202-120">批准请假时间请求。</span><span class="sxs-lookup"><span data-stu-id="b8202-120">Approve a time off request.</span></span>|
|[<span data-ttu-id="b8202-121">拒绝</span><span class="sxs-lookup"><span data-stu-id="b8202-121">Decline</span></span>](../api/timeoffrequest-decline.md)|<span data-ttu-id="b8202-122">None</span><span class="sxs-lookup"><span data-stu-id="b8202-122">None</span></span>|<span data-ttu-id="b8202-123">拒绝休息时间请求。</span><span class="sxs-lookup"><span data-stu-id="b8202-123">Decline a time off request.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8202-124">属性</span><span class="sxs-lookup"><span data-stu-id="b8202-124">Properties</span></span>

| <span data-ttu-id="b8202-125">属性</span><span class="sxs-lookup"><span data-stu-id="b8202-125">Property</span></span>     | <span data-ttu-id="b8202-126">类型</span><span class="sxs-lookup"><span data-stu-id="b8202-126">Type</span></span>        | <span data-ttu-id="b8202-127">说明</span><span class="sxs-lookup"><span data-stu-id="b8202-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8202-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b8202-128">endDateTime</span></span>|<span data-ttu-id="b8202-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8202-129">DateTimeOffset</span></span>|<span data-ttu-id="b8202-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b8202-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b8202-132">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b8202-132">startDateTime</span></span>|<span data-ttu-id="b8202-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8202-133">DateTimeOffset</span></span>|<span data-ttu-id="b8202-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b8202-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b8202-136">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="b8202-136">timeOffReasonId</span></span>|<span data-ttu-id="b8202-137">字符串</span><span class="sxs-lookup"><span data-stu-id="b8202-137">String</span></span>|<span data-ttu-id="b8202-138">休息时间的原因。</span><span class="sxs-lookup"><span data-stu-id="b8202-138">The reason for the time off.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8202-139">关系</span><span class="sxs-lookup"><span data-stu-id="b8202-139">Relationships</span></span>

<span data-ttu-id="b8202-140">无。</span><span class="sxs-lookup"><span data-stu-id="b8202-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8202-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8202-141">JSON representation</span></span>

<span data-ttu-id="b8202-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8202-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeOffRequest",
  "baseType": ""
}-->

```json
{
  "endDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
