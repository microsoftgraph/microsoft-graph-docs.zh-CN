---
title: recentNotebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。 此资源类型以 recentNotebook 资源属性的形式存在。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8435c1c1af8e3c1bc13e4dc07548d303a9ad1a66
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965500"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="ab1d7-104">recentNotebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab1d7-104">recentNotebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab1d7-105">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="ab1d7-105">Links to open a OneNote notebook.</span></span> <span data-ttu-id="ab1d7-106">此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。</span><span class="sxs-lookup"><span data-stu-id="ab1d7-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="ab1d7-107">属性</span><span class="sxs-lookup"><span data-stu-id="ab1d7-107">Properties</span></span>
| <span data-ttu-id="ab1d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab1d7-108">Property</span></span>     | <span data-ttu-id="ab1d7-109">类型</span><span class="sxs-lookup"><span data-stu-id="ab1d7-109">Type</span></span>   |<span data-ttu-id="ab1d7-110">说明</span><span class="sxs-lookup"><span data-stu-id="ab1d7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab1d7-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ab1d7-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="ab1d7-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="ab1d7-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="ab1d7-113">在 OneNote 客户端中打开笔记本 (如果已安装)。</span><span class="sxs-lookup"><span data-stu-id="ab1d7-113">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="ab1d7-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ab1d7-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="ab1d7-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="ab1d7-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="ab1d7-116">在 OneNote 中的 web 上打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="ab1d7-116">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab1d7-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab1d7-117">JSON representation</span></span>

<span data-ttu-id="ab1d7-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab1d7-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
