---
title: responseStatus 资源类型
description: 会议请求的响应状态。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 03deeabfd789fe3e8912d5a431af21bc2c8e5256
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034662"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="b70ec-103">responseStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="b70ec-103">responseStatus resource type</span></span>

<span data-ttu-id="b70ec-104">会议请求的响应状态。</span><span class="sxs-lookup"><span data-stu-id="b70ec-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="b70ec-105">属性</span><span class="sxs-lookup"><span data-stu-id="b70ec-105">Properties</span></span>

| <span data-ttu-id="b70ec-106">属性</span><span class="sxs-lookup"><span data-stu-id="b70ec-106">Property</span></span> | <span data-ttu-id="b70ec-107">类型</span><span class="sxs-lookup"><span data-stu-id="b70ec-107">Type</span></span>           | <span data-ttu-id="b70ec-108">说明</span><span class="sxs-lookup"><span data-stu-id="b70ec-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="b70ec-109">响应</span><span class="sxs-lookup"><span data-stu-id="b70ec-109">response</span></span> | <span data-ttu-id="b70ec-110">responseType</span><span class="sxs-lookup"><span data-stu-id="b70ec-110">responseType</span></span>   | <span data-ttu-id="b70ec-111">响应类型。</span><span class="sxs-lookup"><span data-stu-id="b70ec-111">The response type.</span></span> <span data-ttu-id="b70ec-112">可能的值包括 `None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。</span><span class="sxs-lookup"><span data-stu-id="b70ec-112">The possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="b70ec-113">时间</span><span class="sxs-lookup"><span data-stu-id="b70ec-113">time</span></span>     | <span data-ttu-id="b70ec-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b70ec-114">DateTimeOffset</span></span> | <span data-ttu-id="b70ec-p102">响应返回的日期和时间。它使用 ISO 8601 格式，并始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b70ec-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="b70ec-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b70ec-118">JSON representation</span></span>

<span data-ttu-id="b70ec-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b70ec-119">Here is a JSON representation of the resource</span></span>

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
