---
title: onenoteEntitySchemaObjectModel 资源
description: 这是 OneNote 实体的基本类型。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 9dd44c3360a58195f04632b849f5cafd73490676
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722333"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="ce5d3-103">onenoteEntitySchemaObjectModel 资源</span><span class="sxs-lookup"><span data-stu-id="ce5d3-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="ce5d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce5d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce5d3-105">这是 OneNote 实体的基本类型。</span><span class="sxs-lookup"><span data-stu-id="ce5d3-105">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce5d3-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce5d3-106">JSON representation</span></span>

<span data-ttu-id="ce5d3-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce5d3-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntitySchemaObjectModel"
}-->

```json
{
  "createdDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="ce5d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce5d3-108">Properties</span></span>
| <span data-ttu-id="ce5d3-109">属性</span><span class="sxs-lookup"><span data-stu-id="ce5d3-109">Property</span></span>     | <span data-ttu-id="ce5d3-110">类型</span><span class="sxs-lookup"><span data-stu-id="ce5d3-110">Type</span></span>   |<span data-ttu-id="ce5d3-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce5d3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce5d3-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce5d3-112">createdDateTime</span></span>|<span data-ttu-id="ce5d3-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce5d3-113">DateTimeOffset</span></span>|<span data-ttu-id="ce5d3-114">页面的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ce5d3-114">The date and time when the page was created.</span></span> <span data-ttu-id="ce5d3-115">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ce5d3-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce5d3-116">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="ce5d3-116">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="ce5d3-117">只读。</span><span class="sxs-lookup"><span data-stu-id="ce5d3-117">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

