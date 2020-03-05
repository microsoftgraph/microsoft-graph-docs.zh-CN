---
title: notebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: e33e7d3457a72089e7f01972838fb07d9c9747cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522552"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="46287-103">notebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="46287-103">notebookLinks resource type</span></span>

<span data-ttu-id="46287-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="46287-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46287-105">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="46287-105">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46287-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="46287-106">JSON representation</span></span>

<span data-ttu-id="46287-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="46287-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="46287-108">属性</span><span class="sxs-lookup"><span data-stu-id="46287-108">Properties</span></span>
| <span data-ttu-id="46287-109">属性</span><span class="sxs-lookup"><span data-stu-id="46287-109">Property</span></span>     | <span data-ttu-id="46287-110">类型</span><span class="sxs-lookup"><span data-stu-id="46287-110">Type</span></span>   |<span data-ttu-id="46287-111">说明</span><span class="sxs-lookup"><span data-stu-id="46287-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46287-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="46287-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="46287-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="46287-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="46287-114">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="46287-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="46287-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="46287-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="46287-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="46287-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="46287-117">在 OneNote 中的 web 上打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="46287-117">Opens the notebook in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
