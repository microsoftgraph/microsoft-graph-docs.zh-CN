---
title: pageLinks 资源类型
description: 用于打开 OneNote 页面的链接。
localization_priority: Normal
ms.openlocfilehash: 9bee1b4d3d327118dbf1deec83a37787bd4b18e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832625"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="6c4ae-103">pageLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c4ae-103">pageLinks resource type</span></span>

> <span data-ttu-id="6c4ae-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6c4ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c4ae-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6c4ae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c4ae-106">用于打开 OneNote 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="6c4ae-106">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c4ae-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c4ae-107">JSON representation</span></span>

<span data-ttu-id="6c4ae-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c4ae-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6c4ae-109">属性</span><span class="sxs-lookup"><span data-stu-id="6c4ae-109">Properties</span></span>
| <span data-ttu-id="6c4ae-110">属性</span><span class="sxs-lookup"><span data-stu-id="6c4ae-110">Property</span></span>     | <span data-ttu-id="6c4ae-111">类型</span><span class="sxs-lookup"><span data-stu-id="6c4ae-111">Type</span></span>   |<span data-ttu-id="6c4ae-112">说明</span><span class="sxs-lookup"><span data-stu-id="6c4ae-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c4ae-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="6c4ae-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="6c4ae-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="6c4ae-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="6c4ae-115">如果安装了 OneNote 本机客户端，则在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="6c4ae-115">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="6c4ae-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="6c4ae-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="6c4ae-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="6c4ae-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="6c4ae-118">在 OneNote Online 中打开页面。</span><span class="sxs-lookup"><span data-stu-id="6c4ae-118">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
