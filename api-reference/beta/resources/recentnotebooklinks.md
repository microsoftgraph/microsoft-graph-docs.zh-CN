---
title: recentNotebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。 此资源类型以 recentNotebook 资源属性的形式存在。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f98feb5e9fbe5cede591f4edf0349b3bf4267de9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521255"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="baaf2-104">recentNotebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="baaf2-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="baaf2-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="baaf2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baaf2-106">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="baaf2-106">Links to open a OneNote notebook.</span></span> <span data-ttu-id="baaf2-107">此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。</span><span class="sxs-lookup"><span data-stu-id="baaf2-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="baaf2-108">属性</span><span class="sxs-lookup"><span data-stu-id="baaf2-108">Properties</span></span>
| <span data-ttu-id="baaf2-109">属性</span><span class="sxs-lookup"><span data-stu-id="baaf2-109">Property</span></span>     | <span data-ttu-id="baaf2-110">类型</span><span class="sxs-lookup"><span data-stu-id="baaf2-110">Type</span></span>   |<span data-ttu-id="baaf2-111">说明</span><span class="sxs-lookup"><span data-stu-id="baaf2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baaf2-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="baaf2-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="baaf2-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="baaf2-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="baaf2-114">在 OneNote 客户端中打开笔记本（如果已安装）。</span><span class="sxs-lookup"><span data-stu-id="baaf2-114">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="baaf2-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="baaf2-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="baaf2-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="baaf2-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="baaf2-117">在 OneNote 中的 web 上打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="baaf2-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="baaf2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baaf2-118">JSON representation</span></span>

<span data-ttu-id="baaf2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baaf2-119">The following is a JSON representation of the resource.</span></span>

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
