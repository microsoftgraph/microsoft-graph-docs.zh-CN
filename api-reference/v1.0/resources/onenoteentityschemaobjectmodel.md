---
title: onenoteEntitySchemaObjectModel 资源
description: 这是 OneNote 实体的基类型。
author: Jewan-microsoft
ms.openlocfilehash: a44d05a512b8e4ed2615296faae3f35bd7bd554f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319444"
---
# <a name="onenoteentityschemaobjectmodel-resource"></a><span data-ttu-id="01b67-103">onenoteEntitySchemaObjectModel 资源</span><span class="sxs-lookup"><span data-stu-id="01b67-103">onenoteEntitySchemaObjectModel resource</span></span>

<span data-ttu-id="01b67-104">这是 OneNote 实体的基类型。</span><span class="sxs-lookup"><span data-stu-id="01b67-104">This is a base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01b67-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01b67-105">JSON representation</span></span>

<span data-ttu-id="01b67-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01b67-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="01b67-107">属性</span><span class="sxs-lookup"><span data-stu-id="01b67-107">Properties</span></span>
| <span data-ttu-id="01b67-108">属性</span><span class="sxs-lookup"><span data-stu-id="01b67-108">Property</span></span>     | <span data-ttu-id="01b67-109">类型</span><span class="sxs-lookup"><span data-stu-id="01b67-109">Type</span></span>   |<span data-ttu-id="01b67-110">说明</span><span class="sxs-lookup"><span data-stu-id="01b67-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01b67-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01b67-111">createdDateTime</span></span>|<span data-ttu-id="01b67-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01b67-112">DateTimeOffset</span></span>|<span data-ttu-id="01b67-p101">页面的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。</span><span class="sxs-lookup"><span data-stu-id="01b67-p101">The date and time when the page was created. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->