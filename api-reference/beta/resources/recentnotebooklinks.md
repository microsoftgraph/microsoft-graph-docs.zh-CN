---
title: recentNotebookLinks 资源类型
description: 若要打开的 OneNote 笔记本的链接。 此资源类型以 recentNotebook 资源属性的形式存在。
localization_priority: Normal
ms.openlocfilehash: 328f337d63645cdd52722a4216006920c493f9e7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525883"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="09d96-104">recentNotebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="09d96-104">recentNotebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09d96-105">若要打开的 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="09d96-105">Links to open a OneNote notebook.</span></span> <span data-ttu-id="09d96-106">此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。</span><span class="sxs-lookup"><span data-stu-id="09d96-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="09d96-107">属性</span><span class="sxs-lookup"><span data-stu-id="09d96-107">Properties</span></span>
| <span data-ttu-id="09d96-108">属性</span><span class="sxs-lookup"><span data-stu-id="09d96-108">Property</span></span>     | <span data-ttu-id="09d96-109">类型</span><span class="sxs-lookup"><span data-stu-id="09d96-109">Type</span></span>   |<span data-ttu-id="09d96-110">说明</span><span class="sxs-lookup"><span data-stu-id="09d96-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09d96-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="09d96-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="09d96-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="09d96-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="09d96-113">如果安装在 OneNote 客户端中，打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="09d96-113">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="09d96-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="09d96-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="09d96-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="09d96-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="09d96-116">在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="09d96-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09d96-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09d96-117">JSON representation</span></span>

<span data-ttu-id="09d96-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09d96-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/recentnotebooklinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
