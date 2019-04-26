---
title: sectionLinks 资源类型
description: 用于打开 OneNote 分区的链接。
localization_priority: Normal
ms.openlocfilehash: afc740aebc494aa6f204febbce1be4433005a4b1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549669"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="09e01-103">sectionLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="09e01-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09e01-104">用于打开 OneNote 分区的链接。</span><span class="sxs-lookup"><span data-stu-id="09e01-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09e01-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09e01-105">JSON representation</span></span>

<span data-ttu-id="09e01-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09e01-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="09e01-107">属性</span><span class="sxs-lookup"><span data-stu-id="09e01-107">Properties</span></span>
| <span data-ttu-id="09e01-108">属性</span><span class="sxs-lookup"><span data-stu-id="09e01-108">Property</span></span>     | <span data-ttu-id="09e01-109">类型</span><span class="sxs-lookup"><span data-stu-id="09e01-109">Type</span></span>   |<span data-ttu-id="09e01-110">说明</span><span class="sxs-lookup"><span data-stu-id="09e01-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09e01-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="09e01-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="09e01-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="09e01-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="09e01-113">如果安装了 OneNote 本机客户端, 则打开该分区。</span><span class="sxs-lookup"><span data-stu-id="09e01-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="09e01-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="09e01-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="09e01-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="09e01-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="09e01-116">在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="09e01-116">Opens the section in OneNote Online.</span></span>|

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
