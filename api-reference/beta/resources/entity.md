---
title: 实体资源类型
description: 无
localization_priority: Normal
ms.openlocfilehash: e1dd9a8d66dd326076c8a7dd534c2210f53d06e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509117"
---
# <a name="entity-resource-type"></a><span data-ttu-id="2fa53-103">实体资源类型</span><span class="sxs-lookup"><span data-stu-id="2fa53-103">entity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="2fa53-104">属性</span><span class="sxs-lookup"><span data-stu-id="2fa53-104">Properties</span></span>
| <span data-ttu-id="2fa53-105">属性</span><span class="sxs-lookup"><span data-stu-id="2fa53-105">Property</span></span> | <span data-ttu-id="2fa53-106">类型</span><span class="sxs-lookup"><span data-stu-id="2fa53-106">Type</span></span>  | <span data-ttu-id="2fa53-107">说明</span><span class="sxs-lookup"><span data-stu-id="2fa53-107">Description</span></span> |
|:---------|:------|:------------|
|<span data-ttu-id="2fa53-108">id</span><span class="sxs-lookup"><span data-stu-id="2fa53-108">id</span></span>        |<span data-ttu-id="2fa53-109">String</span><span class="sxs-lookup"><span data-stu-id="2fa53-109">String</span></span> | <span data-ttu-id="2fa53-110">只读。</span><span class="sxs-lookup"><span data-stu-id="2fa53-110">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="2fa53-111">关系</span><span class="sxs-lookup"><span data-stu-id="2fa53-111">Relationships</span></span>
<span data-ttu-id="2fa53-112">无</span><span class="sxs-lookup"><span data-stu-id="2fa53-112">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fa53-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fa53-113">JSON representation</span></span>

<span data-ttu-id="2fa53-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fa53-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "abstract": "true",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entity"
}-->
```json
{
  "id": "string (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "entity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/entity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
