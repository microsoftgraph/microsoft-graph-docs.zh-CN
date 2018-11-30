---
title: recentNotebookLinks 资源类型
description: 若要打开的 OneNote 笔记本的链接。 此资源类型以 recentNotebook 资源属性的形式存在。
ms.openlocfilehash: de13f25148425a1816a60f6cf5b9f4a09f61c7dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045060"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="ed890-104">recentNotebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed890-104">recentNotebookLinks resource type</span></span>

> <span data-ttu-id="ed890-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ed890-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed890-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ed890-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed890-107">若要打开的 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="ed890-107">Links to open a OneNote notebook.</span></span> <span data-ttu-id="ed890-108">此资源类型以 [recentNotebook](recentnotebook.md) 资源属性的形式存在。</span><span class="sxs-lookup"><span data-stu-id="ed890-108">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="ed890-109">属性</span><span class="sxs-lookup"><span data-stu-id="ed890-109">Properties</span></span>
| <span data-ttu-id="ed890-110">属性</span><span class="sxs-lookup"><span data-stu-id="ed890-110">Property</span></span>     | <span data-ttu-id="ed890-111">类型</span><span class="sxs-lookup"><span data-stu-id="ed890-111">Type</span></span>   |<span data-ttu-id="ed890-112">说明</span><span class="sxs-lookup"><span data-stu-id="ed890-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed890-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ed890-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="ed890-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="ed890-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="ed890-115">如果安装在 OneNote 客户端中，打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="ed890-115">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="ed890-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ed890-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="ed890-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="ed890-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="ed890-118">在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="ed890-118">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed890-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed890-119">JSON representation</span></span>

<span data-ttu-id="ed890-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed890-120">The following is a JSON representation of the resource.</span></span>

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
