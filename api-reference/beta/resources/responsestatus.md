---
title: responseStatus 资源类型
description: 会议请求的响应状态。
localization_priority: Normal
ms.openlocfilehash: 8ec4b5f74fa8d83369c23f829b34dfa0ed53a1a1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343575"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="ae308-103">responseStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae308-103">responseStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae308-104">会议请求的响应状态。</span><span class="sxs-lookup"><span data-stu-id="ae308-104">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="ae308-105">属性</span><span class="sxs-lookup"><span data-stu-id="ae308-105">Properties</span></span>

| <span data-ttu-id="ae308-106">属性</span><span class="sxs-lookup"><span data-stu-id="ae308-106">Property</span></span> | <span data-ttu-id="ae308-107">类型</span><span class="sxs-lookup"><span data-stu-id="ae308-107">Type</span></span>           | <span data-ttu-id="ae308-108">说明</span><span class="sxs-lookup"><span data-stu-id="ae308-108">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="ae308-109">响应</span><span class="sxs-lookup"><span data-stu-id="ae308-109">response</span></span> | <span data-ttu-id="ae308-110">String</span><span class="sxs-lookup"><span data-stu-id="ae308-110">String</span></span>         | <span data-ttu-id="ae308-111">响应类型。</span><span class="sxs-lookup"><span data-stu-id="ae308-111">The response type.</span></span> <span data-ttu-id="ae308-112">可取值为：`None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。</span><span class="sxs-lookup"><span data-stu-id="ae308-112">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="ae308-113">时间</span><span class="sxs-lookup"><span data-stu-id="ae308-113">time</span></span>     | <span data-ttu-id="ae308-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae308-114">DateTimeOffset</span></span> | <span data-ttu-id="ae308-p102">响应返回的日期和时间。它使用 ISO 8601 格式，并始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ae308-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae308-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae308-118">JSON representation</span></span>

<span data-ttu-id="ae308-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae308-119">Here is a JSON representation of the resource</span></span>

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
