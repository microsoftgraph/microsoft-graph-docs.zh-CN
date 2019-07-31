---
title: pageLinks 资源类型
description: 用于打开 OneNote 页面的链接。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ea78528cca15da42dfab3260c00d8399f0784bd1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009193"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="ee5c8-103">pageLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee5c8-103">pageLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee5c8-104">用于打开 OneNote 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="ee5c8-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee5c8-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee5c8-105">JSON representation</span></span>

<span data-ttu-id="ee5c8-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee5c8-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ee5c8-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee5c8-107">Properties</span></span>
| <span data-ttu-id="ee5c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee5c8-108">Property</span></span>     | <span data-ttu-id="ee5c8-109">类型</span><span class="sxs-lookup"><span data-stu-id="ee5c8-109">Type</span></span>   |<span data-ttu-id="ee5c8-110">说明</span><span class="sxs-lookup"><span data-stu-id="ee5c8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee5c8-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ee5c8-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="ee5c8-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="ee5c8-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="ee5c8-113">如果安装了 OneNote 本机客户端, 则在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="ee5c8-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="ee5c8-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ee5c8-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="ee5c8-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="ee5c8-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="ee5c8-116">打开 web 上的 OneNote 中的页面。</span><span class="sxs-lookup"><span data-stu-id="ee5c8-116">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
