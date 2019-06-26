---
title: notebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 376000d84ccec8cdc0c1ae601e65f3217275b1e4
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236620"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="a01aa-103">notebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="a01aa-103">notebookLinks resource type</span></span>

<span data-ttu-id="a01aa-104">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="a01aa-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a01aa-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a01aa-105">JSON representation</span></span>

<span data-ttu-id="a01aa-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a01aa-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a01aa-107">属性</span><span class="sxs-lookup"><span data-stu-id="a01aa-107">Properties</span></span>
| <span data-ttu-id="a01aa-108">属性</span><span class="sxs-lookup"><span data-stu-id="a01aa-108">Property</span></span>     | <span data-ttu-id="a01aa-109">类型</span><span class="sxs-lookup"><span data-stu-id="a01aa-109">Type</span></span>   |<span data-ttu-id="a01aa-110">说明</span><span class="sxs-lookup"><span data-stu-id="a01aa-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a01aa-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="a01aa-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="a01aa-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="a01aa-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="a01aa-113">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="a01aa-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="a01aa-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="a01aa-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="a01aa-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="a01aa-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="a01aa-116">在 OneNote 中的 web 上打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="a01aa-116">Opens the notebook in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
