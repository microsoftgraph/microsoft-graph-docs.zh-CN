---
title: recentNotebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。 此资源类型以 recentNotebook 资源属性的形式存在。
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6961a267948c62ac1d24623c6d8bbeaf94f7569
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078995"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="86f86-104">recentNotebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="86f86-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="86f86-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86f86-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86f86-106">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="86f86-106">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="86f86-107">此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。</span><span class="sxs-lookup"><span data-stu-id="86f86-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="86f86-108">属性</span><span class="sxs-lookup"><span data-stu-id="86f86-108">Properties</span></span>
| <span data-ttu-id="86f86-109">属性</span><span class="sxs-lookup"><span data-stu-id="86f86-109">Property</span></span>     | <span data-ttu-id="86f86-110">类型</span><span class="sxs-lookup"><span data-stu-id="86f86-110">Type</span></span>   |<span data-ttu-id="86f86-111">说明</span><span class="sxs-lookup"><span data-stu-id="86f86-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86f86-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="86f86-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="86f86-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="86f86-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="86f86-114">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="86f86-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="86f86-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="86f86-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="86f86-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="86f86-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="86f86-117">在 OneNote 中的 web 上打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="86f86-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86f86-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86f86-118">JSON representation</span></span>

<span data-ttu-id="86f86-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86f86-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

