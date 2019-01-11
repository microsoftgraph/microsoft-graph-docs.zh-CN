---
title: responseStatus 资源类型
description: 会议请求的响应状态。
localization_priority: Normal
ms.openlocfilehash: b337422615e2c34791cd5181a446c25201c183e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843027"
---
# <a name="responsestatus-resource-type"></a><span data-ttu-id="35a5c-103">responseStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="35a5c-103">responseStatus resource type</span></span>

> <span data-ttu-id="35a5c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="35a5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35a5c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="35a5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35a5c-106">会议请求的响应状态。</span><span class="sxs-lookup"><span data-stu-id="35a5c-106">The response status of a meeting request.</span></span>

## <a name="properties"></a><span data-ttu-id="35a5c-107">属性</span><span class="sxs-lookup"><span data-stu-id="35a5c-107">Properties</span></span>

| <span data-ttu-id="35a5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="35a5c-108">Property</span></span> | <span data-ttu-id="35a5c-109">类型</span><span class="sxs-lookup"><span data-stu-id="35a5c-109">Type</span></span>           | <span data-ttu-id="35a5c-110">说明</span><span class="sxs-lookup"><span data-stu-id="35a5c-110">Description</span></span> |
|:---------|:---------------|:------------|
| <span data-ttu-id="35a5c-111">响应</span><span class="sxs-lookup"><span data-stu-id="35a5c-111">response</span></span> | <span data-ttu-id="35a5c-112">String</span><span class="sxs-lookup"><span data-stu-id="35a5c-112">String</span></span>         | <span data-ttu-id="35a5c-113">响应类型。</span><span class="sxs-lookup"><span data-stu-id="35a5c-113">The response type.</span></span> <span data-ttu-id="35a5c-114">可取值为：`None`、`Organizer`、`TentativelyAccepted`、`Accepted`、`Declined`、`NotResponded`。</span><span class="sxs-lookup"><span data-stu-id="35a5c-114">Possible values are: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.</span></span>
| <span data-ttu-id="35a5c-115">时间</span><span class="sxs-lookup"><span data-stu-id="35a5c-115">time</span></span>     | <span data-ttu-id="35a5c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35a5c-116">DateTimeOffset</span></span> | <span data-ttu-id="35a5c-p103">响应返回的日期和时间。它使用 ISO 8601 格式，并始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="35a5c-p103">The date and time that the response was returned. It uses ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>

## <a name="json-representation"></a><span data-ttu-id="35a5c-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35a5c-120">JSON representation</span></span>

<span data-ttu-id="35a5c-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35a5c-121">Here is a JSON representation of the resource</span></span>

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
