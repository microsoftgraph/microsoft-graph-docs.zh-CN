---
title: recentNotebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。 此资源类型以 recentNotebook 资源属性的形式存在。
localization_priority: Normal
ms.openlocfilehash: 846047bd602d19cb4745e0a63f0326aaf7bfb512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810582"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="e0551-104">recentNotebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0551-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="e0551-105">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="e0551-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="e0551-106">此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。</span><span class="sxs-lookup"><span data-stu-id="e0551-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="e0551-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0551-107">Properties</span></span>
| <span data-ttu-id="e0551-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0551-108">Property</span></span>     | <span data-ttu-id="e0551-109">类型</span><span class="sxs-lookup"><span data-stu-id="e0551-109">Type</span></span>   |<span data-ttu-id="e0551-110">说明</span><span class="sxs-lookup"><span data-stu-id="e0551-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0551-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="e0551-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="e0551-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="e0551-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="e0551-113">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="e0551-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="e0551-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="e0551-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="e0551-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="e0551-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="e0551-116">在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="e0551-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e0551-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0551-117">JSON representation</span></span>

<span data-ttu-id="e0551-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0551-118">The following is a JSON representation of the resource.</span></span>

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
