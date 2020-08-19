---
title: pageLinks 资源类型
description: 用于打开 OneNote 页面的链接。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 3442862f52c1d8f6dd29ea2a2a0e99b2f65970f0
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812525"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="95808-103">pageLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="95808-103">pageLinks resource type</span></span>

<span data-ttu-id="95808-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95808-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95808-105">用于打开 OneNote 页面的链接。</span><span class="sxs-lookup"><span data-stu-id="95808-105">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95808-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95808-106">JSON representation</span></span>

<span data-ttu-id="95808-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95808-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="95808-108">属性</span><span class="sxs-lookup"><span data-stu-id="95808-108">Properties</span></span>
| <span data-ttu-id="95808-109">属性</span><span class="sxs-lookup"><span data-stu-id="95808-109">Property</span></span>     | <span data-ttu-id="95808-110">类型</span><span class="sxs-lookup"><span data-stu-id="95808-110">Type</span></span>   |<span data-ttu-id="95808-111">说明</span><span class="sxs-lookup"><span data-stu-id="95808-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95808-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="95808-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="95808-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="95808-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="95808-114">如果安装了 OneNote 本机客户端，则在其中打开页面。</span><span class="sxs-lookup"><span data-stu-id="95808-114">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="95808-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="95808-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="95808-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="95808-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="95808-117">打开 web 上的 OneNote 中的页面。</span><span class="sxs-lookup"><span data-stu-id="95808-117">Opens the page in OneNote on the web.</span></span>|

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
