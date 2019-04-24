---
title: pageLinks 资源类型
description: 用于打开 OneNote 页面的链接。
localization_priority: Normal
ms.openlocfilehash: a5950366f6c6079443338b68db258c5762c15a7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462506"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="4ee3a-103">pageLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ee3a-103">pageLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ee3a-104">用于打开 OneNote 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="4ee3a-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ee3a-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ee3a-105">JSON representation</span></span>

<span data-ttu-id="4ee3a-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ee3a-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pageLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="4ee3a-107">属性</span><span class="sxs-lookup"><span data-stu-id="4ee3a-107">Properties</span></span>
| <span data-ttu-id="4ee3a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ee3a-108">Property</span></span>     | <span data-ttu-id="4ee3a-109">类型</span><span class="sxs-lookup"><span data-stu-id="4ee3a-109">Type</span></span>   |<span data-ttu-id="4ee3a-110">说明</span><span class="sxs-lookup"><span data-stu-id="4ee3a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ee3a-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="4ee3a-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="4ee3a-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="4ee3a-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="4ee3a-113">如果安装了 OneNote 本机客户端, 则在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="4ee3a-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="4ee3a-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="4ee3a-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="4ee3a-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="4ee3a-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="4ee3a-116">在 OneNote Online 中打开页面。</span><span class="sxs-lookup"><span data-stu-id="4ee3a-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/pagelinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
