---
title: responseStatus 资源类型
description: 会议请求的响应状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 0ee9c70baa5cdea45868feb1517623081f2b62b2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718461"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="53a12-103">responseStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="53a12-103">responseStatus resource type</span></span>

<span data-ttu-id="53a12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53a12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53a12-105">会议请求的响应状态。</span><span class="sxs-lookup"><span data-stu-id="53a12-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="53a12-106">属性</span><span class="sxs-lookup"><span data-stu-id="53a12-106">Properties</span></span>

| <span data-ttu-id="53a12-107">属性</span><span class="sxs-lookup"><span data-stu-id="53a12-107">Property</span></span> | <span data-ttu-id="53a12-108">类型</span><span class="sxs-lookup"><span data-stu-id="53a12-108">Type</span></span>           | <span data-ttu-id="53a12-109">说明</span><span class="sxs-lookup"><span data-stu-id="53a12-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="53a12-110">响应</span><span class="sxs-lookup"><span data-stu-id="53a12-110">response</span></span> | <span data-ttu-id="53a12-111">String</span><span class="sxs-lookup"><span data-stu-id="53a12-111">String</span></span>         | <span data-ttu-id="53a12-112">响应类型。</span><span class="sxs-lookup"><span data-stu-id="53a12-112">The response type.</span></span> <span data-ttu-id="53a12-113">可取值为：`None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。</span><span class="sxs-lookup"><span data-stu-id="53a12-113">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="53a12-114">时间</span><span class="sxs-lookup"><span data-stu-id="53a12-114">time</span></span>     | <span data-ttu-id="53a12-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a12-115">DateTimeOffset</span></span> | <span data-ttu-id="53a12-116">响应返回的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="53a12-116">The date and time that the response was returned.</span></span> <span data-ttu-id="53a12-117">它使用 ISO 8601 格式，并始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="53a12-117">It uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53a12-118">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="53a12-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>

## <a name="json-representation"></a><span data-ttu-id="53a12-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53a12-119">JSON representation</span></span>

<span data-ttu-id="53a12-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53a12-120">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


