---
title: externalLink 资源类型
description: 打开 OneNote 页面或笔记本的 URL。
localization_priority: Normal
ms.openlocfilehash: 36acee037a9012290f489f7df675f92265feda1e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515613"
---
# <a name="externallink-resource-type"></a><span data-ttu-id="e4f1b-103">externalLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4f1b-103">externalLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f1b-104">打开 OneNote 页面或笔记本的 URL。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-104">A url that opens a OneNote page or notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4f1b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4f1b-105">JSON representation</span></span>

<span data-ttu-id="e4f1b-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalLink"
}-->

```json
{
  "href": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e4f1b-107">属性</span><span class="sxs-lookup"><span data-stu-id="e4f1b-107">Properties</span></span>
| <span data-ttu-id="e4f1b-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4f1b-108">Property</span></span>     | <span data-ttu-id="e4f1b-109">类型</span><span class="sxs-lookup"><span data-stu-id="e4f1b-109">Type</span></span>   |<span data-ttu-id="e4f1b-110">说明</span><span class="sxs-lookup"><span data-stu-id="e4f1b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4f1b-111">href</span><span class="sxs-lookup"><span data-stu-id="e4f1b-111">href</span></span>|<span data-ttu-id="e4f1b-112">String</span><span class="sxs-lookup"><span data-stu-id="e4f1b-112">String</span></span>|<span data-ttu-id="e4f1b-113">链接的 URL。</span><span class="sxs-lookup"><span data-stu-id="e4f1b-113">The url of the link.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "externalLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/externallink.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
