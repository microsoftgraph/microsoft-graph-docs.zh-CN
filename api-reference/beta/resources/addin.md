---
title: 外接程序资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: d2a63d4428cbb3bcc7cc169711eb6cc6b9e00a6f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643718"
---
# <a name="addin-resource-type"></a><span data-ttu-id="17d38-103">外接程序资源类型</span><span class="sxs-lookup"><span data-stu-id="17d38-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="17d38-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17d38-104">JSON representation</span></span>

<span data-ttu-id="17d38-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17d38-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyvalue"}],
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="17d38-106">属性</span><span class="sxs-lookup"><span data-stu-id="17d38-106">Properties</span></span>
| <span data-ttu-id="17d38-107">属性</span><span class="sxs-lookup"><span data-stu-id="17d38-107">Property</span></span>     | <span data-ttu-id="17d38-108">类型</span><span class="sxs-lookup"><span data-stu-id="17d38-108">Type</span></span>   |<span data-ttu-id="17d38-109">说明</span><span class="sxs-lookup"><span data-stu-id="17d38-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17d38-110">id</span><span class="sxs-lookup"><span data-stu-id="17d38-110">id</span></span>|<span data-ttu-id="17d38-111">guid</span><span class="sxs-lookup"><span data-stu-id="17d38-111">guid</span></span>||
|<span data-ttu-id="17d38-112">properties</span><span class="sxs-lookup"><span data-stu-id="17d38-112">properties</span></span>|<span data-ttu-id="17d38-113">[keyValue](keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="17d38-113">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="17d38-114">type</span><span class="sxs-lookup"><span data-stu-id="17d38-114">type</span></span>|<span data-ttu-id="17d38-115">字符串</span><span class="sxs-lookup"><span data-stu-id="17d38-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/addin.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
