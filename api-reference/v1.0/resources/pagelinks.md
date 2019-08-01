---
title: pageLinks 资源类型
description: 用于打开 OneNote 页面的链接。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5224702d22d111b54d29db15da3c20923ccf7317
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035642"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="af253-103">pageLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="af253-103">pageLinks resource type</span></span>

<span data-ttu-id="af253-104">用于打开 OneNote 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="af253-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af253-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af253-105">JSON representation</span></span>

<span data-ttu-id="af253-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af253-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="af253-107">属性</span><span class="sxs-lookup"><span data-stu-id="af253-107">Properties</span></span>
| <span data-ttu-id="af253-108">属性</span><span class="sxs-lookup"><span data-stu-id="af253-108">Property</span></span>     | <span data-ttu-id="af253-109">类型</span><span class="sxs-lookup"><span data-stu-id="af253-109">Type</span></span>   |<span data-ttu-id="af253-110">说明</span><span class="sxs-lookup"><span data-stu-id="af253-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af253-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="af253-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="af253-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="af253-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="af253-113">如果安装了 OneNote 本机客户端, 则在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="af253-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="af253-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="af253-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="af253-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="af253-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="af253-116">打开 web 上的 OneNote 中的页面。</span><span class="sxs-lookup"><span data-stu-id="af253-116">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
