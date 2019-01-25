---
title: outlookItem 资源类型
description: 下面是资源的 JSON 表示形式。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8a44f9a2e568991c6803ebf72baf5f712f39ba64
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528289"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="d50ad-103">outlookItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d50ad-103">outlookItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="d50ad-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d50ad-104">JSON representation</span></span>

<span data-ttu-id="d50ad-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d50ad-105">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d50ad-106">属性</span><span class="sxs-lookup"><span data-stu-id="d50ad-106">Properties</span></span>
| <span data-ttu-id="d50ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="d50ad-107">Property</span></span>     | <span data-ttu-id="d50ad-108">类型</span><span class="sxs-lookup"><span data-stu-id="d50ad-108">Type</span></span>   |<span data-ttu-id="d50ad-109">说明</span><span class="sxs-lookup"><span data-stu-id="d50ad-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d50ad-110">categories</span><span class="sxs-lookup"><span data-stu-id="d50ad-110">categories</span></span>|<span data-ttu-id="d50ad-111">String collection</span><span class="sxs-lookup"><span data-stu-id="d50ad-111">String collection</span></span>||
|<span data-ttu-id="d50ad-112">changeKey</span><span class="sxs-lookup"><span data-stu-id="d50ad-112">changeKey</span></span>|<span data-ttu-id="d50ad-113">String</span><span class="sxs-lookup"><span data-stu-id="d50ad-113">String</span></span>||
|<span data-ttu-id="d50ad-114">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d50ad-114">createdDateTime</span></span>|<span data-ttu-id="d50ad-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d50ad-115">DateTimeOffset</span></span>|<span data-ttu-id="d50ad-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d50ad-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d50ad-118">id</span><span class="sxs-lookup"><span data-stu-id="d50ad-118">id</span></span>|<span data-ttu-id="d50ad-119">String</span><span class="sxs-lookup"><span data-stu-id="d50ad-119">String</span></span>| <span data-ttu-id="d50ad-120">只读。</span><span class="sxs-lookup"><span data-stu-id="d50ad-120">Read-only.</span></span>|
|<span data-ttu-id="d50ad-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d50ad-121">lastModifiedDateTime</span></span>|<span data-ttu-id="d50ad-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d50ad-122">DateTimeOffset</span></span>|<span data-ttu-id="d50ad-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d50ad-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="d50ad-125">关系</span><span class="sxs-lookup"><span data-stu-id="d50ad-125">Relationships</span></span>
<span data-ttu-id="d50ad-126">无</span><span class="sxs-lookup"><span data-stu-id="d50ad-126">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/outlookitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
