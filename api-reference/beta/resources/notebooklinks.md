---
title: notebookLinks 资源类型
description: 用于打开 OneNote 笔记本的链接。
ms.openlocfilehash: 33f9a877ea6cae64acf3f05234362bfb86530c2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042660"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="a5cd5-103">notebookLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5cd5-103">notebookLinks resource type</span></span>

> <span data-ttu-id="a5cd5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a5cd5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5cd5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5cd5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5cd5-106">用于打开 OneNote 笔记本的链接。</span><span class="sxs-lookup"><span data-stu-id="a5cd5-106">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5cd5-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5cd5-107">JSON representation</span></span>

<span data-ttu-id="a5cd5-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5cd5-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a5cd5-109">属性</span><span class="sxs-lookup"><span data-stu-id="a5cd5-109">Properties</span></span>
| <span data-ttu-id="a5cd5-110">属性</span><span class="sxs-lookup"><span data-stu-id="a5cd5-110">Property</span></span>     | <span data-ttu-id="a5cd5-111">类型</span><span class="sxs-lookup"><span data-stu-id="a5cd5-111">Type</span></span>   |<span data-ttu-id="a5cd5-112">说明</span><span class="sxs-lookup"><span data-stu-id="a5cd5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5cd5-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="a5cd5-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="a5cd5-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="a5cd5-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="a5cd5-115">如果安装了 OneNote 本机客户端，则在其中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="a5cd5-115">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="a5cd5-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="a5cd5-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="a5cd5-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="a5cd5-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="a5cd5-118">在 OneNote Online 中打开笔记本。</span><span class="sxs-lookup"><span data-stu-id="a5cd5-118">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->