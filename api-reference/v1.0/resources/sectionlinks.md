---
title: sectionLinks 资源类型
description: 用于打开 OneNote 分区的链接。
localization_priority: Normal
ms.openlocfilehash: afc740aebc494aa6f204febbce1be4433005a4b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839933"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="dc63f-103">sectionLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc63f-103">sectionLinks resource type</span></span>

<span data-ttu-id="dc63f-104">用于打开 OneNote 分区的链接。</span><span class="sxs-lookup"><span data-stu-id="dc63f-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc63f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc63f-105">JSON representation</span></span>

<span data-ttu-id="dc63f-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc63f-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="dc63f-107">属性</span><span class="sxs-lookup"><span data-stu-id="dc63f-107">Properties</span></span>
| <span data-ttu-id="dc63f-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc63f-108">Property</span></span>     | <span data-ttu-id="dc63f-109">类型</span><span class="sxs-lookup"><span data-stu-id="dc63f-109">Type</span></span>   |<span data-ttu-id="dc63f-110">说明</span><span class="sxs-lookup"><span data-stu-id="dc63f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc63f-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="dc63f-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="dc63f-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="dc63f-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="dc63f-113">如果安装了 OneNote 本机客户端，则在其中打开分区。</span><span class="sxs-lookup"><span data-stu-id="dc63f-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="dc63f-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="dc63f-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="dc63f-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="dc63f-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="dc63f-116">在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="dc63f-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
