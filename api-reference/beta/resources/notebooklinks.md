---
title: notebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: b0050463ec3b88bd32e69efa6cfde5189fdce8d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033669"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="95656-103">notebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="95656-103">notebookLinks resource type</span></span>

<span data-ttu-id="95656-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95656-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95656-105">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="95656-105">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95656-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95656-106">JSON representation</span></span>

<span data-ttu-id="95656-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95656-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="95656-108">属性</span><span class="sxs-lookup"><span data-stu-id="95656-108">Properties</span></span>
| <span data-ttu-id="95656-109">属性</span><span class="sxs-lookup"><span data-stu-id="95656-109">Property</span></span>     | <span data-ttu-id="95656-110">类型</span><span class="sxs-lookup"><span data-stu-id="95656-110">Type</span></span>   |<span data-ttu-id="95656-111">说明</span><span class="sxs-lookup"><span data-stu-id="95656-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95656-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="95656-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="95656-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="95656-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="95656-114">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="95656-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="95656-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="95656-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="95656-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="95656-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="95656-117">在 OneNote 中的 web 上打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="95656-117">Opens the notebook in OneNote on the web.</span></span>|

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


