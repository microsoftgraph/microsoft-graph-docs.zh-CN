---
title: sectionLinks 资源类型
description: 用于打开 OneNote 分区的链接。
localization_priority: Normal
ms.openlocfilehash: a5e2f4800472e8cedc495e6de1c17a6586710e87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562872"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="e2d94-103">sectionLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2d94-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2d94-104">用于打开 OneNote 分区的链接。</span><span class="sxs-lookup"><span data-stu-id="e2d94-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2d94-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2d94-105">JSON representation</span></span>

<span data-ttu-id="e2d94-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2d94-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="e2d94-107">属性</span><span class="sxs-lookup"><span data-stu-id="e2d94-107">Properties</span></span>
| <span data-ttu-id="e2d94-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2d94-108">Property</span></span>     | <span data-ttu-id="e2d94-109">类型</span><span class="sxs-lookup"><span data-stu-id="e2d94-109">Type</span></span>   |<span data-ttu-id="e2d94-110">说明</span><span class="sxs-lookup"><span data-stu-id="e2d94-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2d94-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="e2d94-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="e2d94-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="e2d94-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="e2d94-113">如果安装了 OneNote 本机客户端, 则打开该分区。</span><span class="sxs-lookup"><span data-stu-id="e2d94-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="e2d94-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="e2d94-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="e2d94-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="e2d94-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="e2d94-116">在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="e2d94-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sectionlinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
