---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 77741fa05f356418e688cdc4a45c5a4750604c3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009277"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="a4f7e-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4f7e-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="a4f7e-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4f7e-104">JSON representation</span></span>

<span data-ttu-id="a4f7e-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4f7e-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a4f7e-106">属性</span><span class="sxs-lookup"><span data-stu-id="a4f7e-106">Properties</span></span>
| <span data-ttu-id="a4f7e-107">属性</span><span class="sxs-lookup"><span data-stu-id="a4f7e-107">Property</span></span>     | <span data-ttu-id="a4f7e-108">类型</span><span class="sxs-lookup"><span data-stu-id="a4f7e-108">Type</span></span>   |<span data-ttu-id="a4f7e-109">说明</span><span class="sxs-lookup"><span data-stu-id="a4f7e-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4f7e-110">categories</span><span class="sxs-lookup"><span data-stu-id="a4f7e-110">categories</span></span>|<span data-ttu-id="a4f7e-111">String collection</span><span class="sxs-lookup"><span data-stu-id="a4f7e-111">String collection</span></span>||
|<span data-ttu-id="a4f7e-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="a4f7e-112">changeKey</span></span>|<span data-ttu-id="a4f7e-113">String</span><span class="sxs-lookup"><span data-stu-id="a4f7e-113">String</span></span>||
|<span data-ttu-id="a4f7e-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4f7e-114">createdDateTime</span></span>|<span data-ttu-id="a4f7e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4f7e-115">DateTimeOffset</span></span>|<span data-ttu-id="a4f7e-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a4f7e-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a4f7e-118">id</span><span class="sxs-lookup"><span data-stu-id="a4f7e-118">id</span></span>|<span data-ttu-id="a4f7e-119">String</span><span class="sxs-lookup"><span data-stu-id="a4f7e-119">String</span></span>| <span data-ttu-id="a4f7e-120">只读。</span><span class="sxs-lookup"><span data-stu-id="a4f7e-120">Read-only.</span></span>|
|<span data-ttu-id="a4f7e-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4f7e-121">lastModifiedDateTime</span></span>|<span data-ttu-id="a4f7e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4f7e-122">DateTimeOffset</span></span>|<span data-ttu-id="a4f7e-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a4f7e-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4f7e-125">关系</span><span class="sxs-lookup"><span data-stu-id="a4f7e-125">Relationships</span></span>
<span data-ttu-id="a4f7e-126">无</span><span class="sxs-lookup"><span data-stu-id="a4f7e-126">None</span></span>


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
