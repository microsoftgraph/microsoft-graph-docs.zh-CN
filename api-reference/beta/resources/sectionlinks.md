---
title: sectionLinks 资源类型
description: 用于打开 OneNote 分区的链接。
localization_priority: Normal
ms.openlocfilehash: 190842708979d62430a4716a8785fd40309cb189
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858938"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="843f4-103">sectionLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="843f4-103">sectionLinks resource type</span></span>

> <span data-ttu-id="843f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="843f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="843f4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="843f4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="843f4-106">用于打开 OneNote 分区的链接。</span><span class="sxs-lookup"><span data-stu-id="843f4-106">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="843f4-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="843f4-107">JSON representation</span></span>

<span data-ttu-id="843f4-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="843f4-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="843f4-109">属性</span><span class="sxs-lookup"><span data-stu-id="843f4-109">Properties</span></span>
| <span data-ttu-id="843f4-110">属性</span><span class="sxs-lookup"><span data-stu-id="843f4-110">Property</span></span>     | <span data-ttu-id="843f4-111">类型</span><span class="sxs-lookup"><span data-stu-id="843f4-111">Type</span></span>   |<span data-ttu-id="843f4-112">说明</span><span class="sxs-lookup"><span data-stu-id="843f4-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="843f4-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="843f4-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="843f4-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="843f4-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="843f4-115">如果安装了 OneNote 本机客户端，则在其中打开分区。</span><span class="sxs-lookup"><span data-stu-id="843f4-115">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="843f4-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="843f4-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="843f4-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="843f4-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="843f4-118">在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="843f4-118">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
