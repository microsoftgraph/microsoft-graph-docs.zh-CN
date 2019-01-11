---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: b88a450465798386ad57e82ff76896417301a606
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817631"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="3e425-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e425-103">outlookItem resource type</span></span>

> <span data-ttu-id="3e425-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3e425-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e425-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3e425-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e425-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e425-106">JSON representation</span></span>

<span data-ttu-id="3e425-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e425-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookitem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="3e425-108">属性</span><span class="sxs-lookup"><span data-stu-id="3e425-108">Properties</span></span>
| <span data-ttu-id="3e425-109">属性</span><span class="sxs-lookup"><span data-stu-id="3e425-109">Property</span></span>     | <span data-ttu-id="3e425-110">类型</span><span class="sxs-lookup"><span data-stu-id="3e425-110">Type</span></span>   |<span data-ttu-id="3e425-111">说明</span><span class="sxs-lookup"><span data-stu-id="3e425-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e425-112">categories</span><span class="sxs-lookup"><span data-stu-id="3e425-112">categories</span></span>|<span data-ttu-id="3e425-113">String collection</span><span class="sxs-lookup"><span data-stu-id="3e425-113">String collection</span></span>||
|<span data-ttu-id="3e425-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="3e425-114">changeKey</span></span>|<span data-ttu-id="3e425-115">String</span><span class="sxs-lookup"><span data-stu-id="3e425-115">String</span></span>||
|<span data-ttu-id="3e425-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e425-116">createdDateTime</span></span>|<span data-ttu-id="3e425-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e425-117">DateTimeOffset</span></span>|<span data-ttu-id="3e425-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3e425-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3e425-120">id</span><span class="sxs-lookup"><span data-stu-id="3e425-120">id</span></span>|<span data-ttu-id="3e425-121">String</span><span class="sxs-lookup"><span data-stu-id="3e425-121">String</span></span>| <span data-ttu-id="3e425-122">只读。</span><span class="sxs-lookup"><span data-stu-id="3e425-122">Read-only.</span></span>|
|<span data-ttu-id="3e425-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e425-123">lastModifiedDateTime</span></span>|<span data-ttu-id="3e425-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e425-124">DateTimeOffset</span></span>|<span data-ttu-id="3e425-p103">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3e425-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e425-127">Relationships</span><span class="sxs-lookup"><span data-stu-id="3e425-127">Relationships</span></span>
<span data-ttu-id="3e425-128">无</span><span class="sxs-lookup"><span data-stu-id="3e425-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
