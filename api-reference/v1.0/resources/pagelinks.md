---
title: pageLinks 资源类型
description: 用于打开 OneNote 页面的链接。
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 33f5aa2c5953bc9e143d08d91047919cf73599b6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094209"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="35eb8-103">pageLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="35eb8-103">pageLinks resource type</span></span>

<span data-ttu-id="35eb8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35eb8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35eb8-105">用于打开 OneNote 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="35eb8-105">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35eb8-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35eb8-106">JSON representation</span></span>

<span data-ttu-id="35eb8-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35eb8-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="35eb8-108">属性</span><span class="sxs-lookup"><span data-stu-id="35eb8-108">Properties</span></span>
| <span data-ttu-id="35eb8-109">属性</span><span class="sxs-lookup"><span data-stu-id="35eb8-109">Property</span></span>     | <span data-ttu-id="35eb8-110">类型</span><span class="sxs-lookup"><span data-stu-id="35eb8-110">Type</span></span>   |<span data-ttu-id="35eb8-111">说明</span><span class="sxs-lookup"><span data-stu-id="35eb8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35eb8-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="35eb8-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="35eb8-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="35eb8-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="35eb8-114">如果安装了 OneNote 本机客户端，则在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="35eb8-114">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="35eb8-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="35eb8-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="35eb8-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="35eb8-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="35eb8-117">打开 web 上的 OneNote 中的页面。</span><span class="sxs-lookup"><span data-stu-id="35eb8-117">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

