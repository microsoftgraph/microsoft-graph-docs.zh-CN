---
title: notebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。
author: Jewan-microsoft
ms.openlocfilehash: f263a255199dea844f62d322b4be010111c9c823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357174"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="5da4b-103">notebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="5da4b-103">notebookLinks resource type</span></span>

<span data-ttu-id="5da4b-104">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="5da4b-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5da4b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5da4b-105">JSON representation</span></span>

<span data-ttu-id="5da4b-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5da4b-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="5da4b-107">属性</span><span class="sxs-lookup"><span data-stu-id="5da4b-107">Properties</span></span>
| <span data-ttu-id="5da4b-108">属性</span><span class="sxs-lookup"><span data-stu-id="5da4b-108">Property</span></span>     | <span data-ttu-id="5da4b-109">类型</span><span class="sxs-lookup"><span data-stu-id="5da4b-109">Type</span></span>   |<span data-ttu-id="5da4b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5da4b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5da4b-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="5da4b-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="5da4b-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="5da4b-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="5da4b-113">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="5da4b-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="5da4b-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="5da4b-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="5da4b-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="5da4b-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="5da4b-116">在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="5da4b-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->