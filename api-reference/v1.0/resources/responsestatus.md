---
title: responseStatus 资源类型
description: 会议请求的响应状态。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 69aae664c21290d00505997d5ff84658620d67e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967210"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="83dbc-103">responseStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="83dbc-103">responseStatus resource type</span></span>

<span data-ttu-id="83dbc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83dbc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83dbc-105">会议请求的响应状态。</span><span class="sxs-lookup"><span data-stu-id="83dbc-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="83dbc-106">属性</span><span class="sxs-lookup"><span data-stu-id="83dbc-106">Properties</span></span>

| <span data-ttu-id="83dbc-107">属性</span><span class="sxs-lookup"><span data-stu-id="83dbc-107">Property</span></span> | <span data-ttu-id="83dbc-108">类型</span><span class="sxs-lookup"><span data-stu-id="83dbc-108">Type</span></span>           | <span data-ttu-id="83dbc-109">说明</span><span class="sxs-lookup"><span data-stu-id="83dbc-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="83dbc-110">响应</span><span class="sxs-lookup"><span data-stu-id="83dbc-110">response</span></span> | <span data-ttu-id="83dbc-111">responseType</span><span class="sxs-lookup"><span data-stu-id="83dbc-111">responseType</span></span>   | <span data-ttu-id="83dbc-112">响应类型。</span><span class="sxs-lookup"><span data-stu-id="83dbc-112">The response type.</span></span> <span data-ttu-id="83dbc-113">可能的值包括 `None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。</span><span class="sxs-lookup"><span data-stu-id="83dbc-113">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="83dbc-114">时间</span><span class="sxs-lookup"><span data-stu-id="83dbc-114">time</span></span>     | <span data-ttu-id="83dbc-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83dbc-115">DateTimeOffset</span></span> | <span data-ttu-id="83dbc-p102">响应返回的日期和时间。它使用 ISO 8601 格式，并始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="83dbc-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="83dbc-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83dbc-119">JSON representation</span></span>

<span data-ttu-id="83dbc-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83dbc-120">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

