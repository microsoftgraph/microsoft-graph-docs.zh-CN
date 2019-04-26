---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b2c43d81d045ee6b563e7ae81f8fe6fab56bdf83
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341846"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="6639d-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="6639d-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="6639d-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6639d-104">JSON representation</span></span>

<span data-ttu-id="6639d-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6639d-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookItem"
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
## <a name="properties"></a><span data-ttu-id="6639d-106">属性</span><span class="sxs-lookup"><span data-stu-id="6639d-106">Properties</span></span>
| <span data-ttu-id="6639d-107">属性</span><span class="sxs-lookup"><span data-stu-id="6639d-107">Property</span></span>     | <span data-ttu-id="6639d-108">类型</span><span class="sxs-lookup"><span data-stu-id="6639d-108">Type</span></span>   |<span data-ttu-id="6639d-109">说明</span><span class="sxs-lookup"><span data-stu-id="6639d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6639d-110">类别</span><span class="sxs-lookup"><span data-stu-id="6639d-110">categories</span></span>|<span data-ttu-id="6639d-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="6639d-111">String collection</span></span>||
|<span data-ttu-id="6639d-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="6639d-112">changeKey</span></span>|<span data-ttu-id="6639d-113">String</span><span class="sxs-lookup"><span data-stu-id="6639d-113">String</span></span>||
|<span data-ttu-id="6639d-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6639d-114">createdDateTime</span></span>|<span data-ttu-id="6639d-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6639d-115">DateTimeOffset</span></span>|<span data-ttu-id="6639d-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6639d-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6639d-118">id</span><span class="sxs-lookup"><span data-stu-id="6639d-118">id</span></span>|<span data-ttu-id="6639d-119">String</span><span class="sxs-lookup"><span data-stu-id="6639d-119">String</span></span>| <span data-ttu-id="6639d-120">只读。</span><span class="sxs-lookup"><span data-stu-id="6639d-120">Read-only.</span></span>|
|<span data-ttu-id="6639d-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6639d-121">lastModifiedDateTime</span></span>|<span data-ttu-id="6639d-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6639d-122">DateTimeOffset</span></span>|<span data-ttu-id="6639d-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6639d-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="6639d-125">关系</span><span class="sxs-lookup"><span data-stu-id="6639d-125">Relationships</span></span>
<span data-ttu-id="6639d-126">无</span><span class="sxs-lookup"><span data-stu-id="6639d-126">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
