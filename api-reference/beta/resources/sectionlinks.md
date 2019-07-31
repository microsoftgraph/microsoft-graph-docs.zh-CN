---
title: sectionLinks 资源类型
description: 用于打开 OneNote 分区的链接。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 270cc08f797546f08dbb89c4137631dd30cc4ae0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008591"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="c4c5c-103">sectionLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4c5c-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4c5c-104">用于打开 OneNote 分区的链接。</span><span class="sxs-lookup"><span data-stu-id="c4c5c-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4c5c-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4c5c-105">JSON representation</span></span>

<span data-ttu-id="c4c5c-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4c5c-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="c4c5c-107">属性</span><span class="sxs-lookup"><span data-stu-id="c4c5c-107">Properties</span></span>
| <span data-ttu-id="c4c5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="c4c5c-108">Property</span></span>     | <span data-ttu-id="c4c5c-109">类型</span><span class="sxs-lookup"><span data-stu-id="c4c5c-109">Type</span></span>   |<span data-ttu-id="c4c5c-110">说明</span><span class="sxs-lookup"><span data-stu-id="c4c5c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4c5c-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="c4c5c-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="c4c5c-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="c4c5c-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="c4c5c-113">如果安装了 OneNote 本机客户端, 则打开该分区。</span><span class="sxs-lookup"><span data-stu-id="c4c5c-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="c4c5c-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="c4c5c-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="c4c5c-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="c4c5c-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="c4c5c-116">打开 web 上的 OneNote 中的部分。</span><span class="sxs-lookup"><span data-stu-id="c4c5c-116">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
