---
title: responseStatus 资源类型
description: 会议请求的响应状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 4ab1c5e54112b5d51e3d88452e2ee0ddcb59f6dd
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811383"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="2519c-103">responseStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="2519c-103">responseStatus resource type</span></span>

<span data-ttu-id="2519c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2519c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2519c-105">会议请求的响应状态。</span><span class="sxs-lookup"><span data-stu-id="2519c-105">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="2519c-106">属性</span><span class="sxs-lookup"><span data-stu-id="2519c-106">Properties</span></span>

| <span data-ttu-id="2519c-107">属性</span><span class="sxs-lookup"><span data-stu-id="2519c-107">Property</span></span> | <span data-ttu-id="2519c-108">类型</span><span class="sxs-lookup"><span data-stu-id="2519c-108">Type</span></span>           | <span data-ttu-id="2519c-109">说明</span><span class="sxs-lookup"><span data-stu-id="2519c-109">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="2519c-110">响应</span><span class="sxs-lookup"><span data-stu-id="2519c-110">response</span></span> | <span data-ttu-id="2519c-111">String</span><span class="sxs-lookup"><span data-stu-id="2519c-111">String</span></span>         | <span data-ttu-id="2519c-112">响应类型。</span><span class="sxs-lookup"><span data-stu-id="2519c-112">The response type.</span></span> <span data-ttu-id="2519c-113">可取值为：`None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。</span><span class="sxs-lookup"><span data-stu-id="2519c-113">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="2519c-114">时间</span><span class="sxs-lookup"><span data-stu-id="2519c-114">time</span></span>     | <span data-ttu-id="2519c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2519c-115">DateTimeOffset</span></span> | <span data-ttu-id="2519c-p102">响应返回的日期和时间。它使用 ISO 8601 格式，并始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2519c-p102">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="2519c-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2519c-119">JSON representation</span></span>

<span data-ttu-id="2519c-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2519c-120">Here is a JSON representation of the resource</span></span>

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
