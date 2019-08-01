---
title: onenoteEntitySchemaObjectModel 资源
description: 这是 OneNote 实体的基本类型。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 4072a6d02ffb003731613c081effac50215f605a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035810"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="32e6e-103">onenoteEntitySchemaObjectModel 资源</span><span class="sxs-lookup"><span data-stu-id="32e6e-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="32e6e-104">这是 OneNote 实体的基本类型。</span><span class="sxs-lookup"><span data-stu-id="32e6e-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="32e6e-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32e6e-105">JSON representation</span></span>

<span data-ttu-id="32e6e-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32e6e-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="32e6e-107">属性</span><span class="sxs-lookup"><span data-stu-id="32e6e-107">Properties</span></span>
| <span data-ttu-id="32e6e-108">属性</span><span class="sxs-lookup"><span data-stu-id="32e6e-108">Property</span></span>     | <span data-ttu-id="32e6e-109">类型</span><span class="sxs-lookup"><span data-stu-id="32e6e-109">Type</span></span>   |<span data-ttu-id="32e6e-110">说明</span><span class="sxs-lookup"><span data-stu-id="32e6e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32e6e-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32e6e-111">createdDateTime</span></span>|<span data-ttu-id="32e6e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32e6e-112">DateTimeOffset</span></span>|<span data-ttu-id="32e6e-113">页面的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="32e6e-113">The date and time when the page was created.</span></span> <span data-ttu-id="32e6e-114">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="32e6e-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="32e6e-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="32e6e-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="32e6e-116">只读。</span><span class="sxs-lookup"><span data-stu-id="32e6e-116">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
