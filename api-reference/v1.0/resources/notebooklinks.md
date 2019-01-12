---
title: notebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d3def81fb9bb3b7f657be3ed04230a65235db5f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984253"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="7f59f-103">notebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f59f-103">notebookLinks resource type</span></span>

<span data-ttu-id="7f59f-104">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="7f59f-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f59f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f59f-105">JSON representation</span></span>

<span data-ttu-id="7f59f-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f59f-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7f59f-107">属性</span><span class="sxs-lookup"><span data-stu-id="7f59f-107">Properties</span></span>
| <span data-ttu-id="7f59f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f59f-108">Property</span></span>     | <span data-ttu-id="7f59f-109">类型</span><span class="sxs-lookup"><span data-stu-id="7f59f-109">Type</span></span>   |<span data-ttu-id="7f59f-110">说明</span><span class="sxs-lookup"><span data-stu-id="7f59f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f59f-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="7f59f-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="7f59f-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="7f59f-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="7f59f-113">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="7f59f-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="7f59f-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="7f59f-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="7f59f-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="7f59f-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="7f59f-116">在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="7f59f-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
