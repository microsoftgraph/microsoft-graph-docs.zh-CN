---
title: sectionLinks 资源类型
description: 用于打开 OneNote 分区的链接。
localization_priority: Normal
ms.openlocfilehash: 2c3744e08c492a8857600dc9e51dc205ae387bad
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236508"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="66e2b-103">sectionLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="66e2b-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66e2b-104">用于打开 OneNote 分区的链接。</span><span class="sxs-lookup"><span data-stu-id="66e2b-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66e2b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66e2b-105">JSON representation</span></span>

<span data-ttu-id="66e2b-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66e2b-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="66e2b-107">属性</span><span class="sxs-lookup"><span data-stu-id="66e2b-107">Properties</span></span>
| <span data-ttu-id="66e2b-108">属性</span><span class="sxs-lookup"><span data-stu-id="66e2b-108">Property</span></span>     | <span data-ttu-id="66e2b-109">类型</span><span class="sxs-lookup"><span data-stu-id="66e2b-109">Type</span></span>   |<span data-ttu-id="66e2b-110">说明</span><span class="sxs-lookup"><span data-stu-id="66e2b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66e2b-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="66e2b-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="66e2b-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="66e2b-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="66e2b-113">如果安装了 OneNote 本机客户端, 则打开该分区。</span><span class="sxs-lookup"><span data-stu-id="66e2b-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="66e2b-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="66e2b-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="66e2b-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="66e2b-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="66e2b-116">打开 web 上的 OneNote 中的部分。</span><span class="sxs-lookup"><span data-stu-id="66e2b-116">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
