---
title: pageLinks 资源类型
description: 用于打开 OneNote 页面的链接。
ms.openlocfilehash: f1e4fe36d4356986bc88b744a9a62e28b8d368c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008187"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="72b25-103">pageLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="72b25-103">pageLinks resource type</span></span>

<span data-ttu-id="72b25-104">用于打开 OneNote 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="72b25-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72b25-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72b25-105">JSON representation</span></span>

<span data-ttu-id="72b25-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72b25-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="72b25-107">属性</span><span class="sxs-lookup"><span data-stu-id="72b25-107">Properties</span></span>
| <span data-ttu-id="72b25-108">属性</span><span class="sxs-lookup"><span data-stu-id="72b25-108">Property</span></span>     | <span data-ttu-id="72b25-109">类型</span><span class="sxs-lookup"><span data-stu-id="72b25-109">Type</span></span>   |<span data-ttu-id="72b25-110">说明</span><span class="sxs-lookup"><span data-stu-id="72b25-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72b25-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="72b25-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="72b25-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="72b25-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="72b25-113">如果安装了 OneNote 本机客户端，则在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="72b25-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="72b25-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="72b25-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="72b25-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="72b25-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="72b25-116">在 OneNote Online 中打开页面。</span><span class="sxs-lookup"><span data-stu-id="72b25-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->