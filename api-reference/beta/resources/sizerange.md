---
title: sizeRange 资源类型
description: 指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。
localization_priority: Normal
ms.openlocfilehash: ecf4a4349e7ee54b9f21fa27879834b45dc87491
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522397"
---
# <a name="sizerange-resource-type"></a><span data-ttu-id="81a71-103">sizeRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="81a71-103">sizeRange resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81a71-104">指定传入邮件必须具有的最大大小和最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="81a71-104">Specifies the maximum and minimum sizes (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span>

## <a name="properties"></a><span data-ttu-id="81a71-105">属性</span><span class="sxs-lookup"><span data-stu-id="81a71-105">Properties</span></span>
| <span data-ttu-id="81a71-106">属性</span><span class="sxs-lookup"><span data-stu-id="81a71-106">Property</span></span>     | <span data-ttu-id="81a71-107">类型</span><span class="sxs-lookup"><span data-stu-id="81a71-107">Type</span></span>   |<span data-ttu-id="81a71-108">说明</span><span class="sxs-lookup"><span data-stu-id="81a71-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="81a71-109">maximumSize</span><span class="sxs-lookup"><span data-stu-id="81a71-109">maximumSize</span></span> | <span data-ttu-id="81a71-110">Int32</span><span class="sxs-lookup"><span data-stu-id="81a71-110">Int32</span></span> | <span data-ttu-id="81a71-111">传入邮件必须具有的最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="81a71-111">The maximum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |
| <span data-ttu-id="81a71-112">minimumSize</span><span class="sxs-lookup"><span data-stu-id="81a71-112">minimumSize</span></span> | <span data-ttu-id="81a71-113">Int32</span><span class="sxs-lookup"><span data-stu-id="81a71-113">Int32</span></span> | <span data-ttu-id="81a71-114">传入邮件必须具有的最小大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="81a71-114">The minimum size (in kilobytes) that an incoming message must have in order for a condition or exception to apply.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="81a71-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81a71-115">JSON representation</span></span>
<span data-ttu-id="81a71-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81a71-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sizerange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
