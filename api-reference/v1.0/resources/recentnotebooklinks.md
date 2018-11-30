---
title: recentNotebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。 此资源类型以 recentNotebook 资源属性的形式存在。
ms.openlocfilehash: 594616a790becd77086177157f71321ffdd36e24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008636"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="29575-104">recentNotebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="29575-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="29575-105">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="29575-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="29575-106">此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。</span><span class="sxs-lookup"><span data-stu-id="29575-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="29575-107">属性</span><span class="sxs-lookup"><span data-stu-id="29575-107">Properties</span></span>
| <span data-ttu-id="29575-108">属性</span><span class="sxs-lookup"><span data-stu-id="29575-108">Property</span></span>     | <span data-ttu-id="29575-109">类型</span><span class="sxs-lookup"><span data-stu-id="29575-109">Type</span></span>   |<span data-ttu-id="29575-110">说明</span><span class="sxs-lookup"><span data-stu-id="29575-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29575-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="29575-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="29575-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="29575-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="29575-113">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="29575-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="29575-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="29575-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="29575-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="29575-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="29575-116">在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="29575-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29575-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29575-117">JSON representation</span></span>

<span data-ttu-id="29575-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29575-118">The following is a JSON representation of the resource.</span></span>

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
