---
title: sectionLinks 资源类型
description: 用于打开 OneNote 分区的链接。
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2c0bf1090f3d60388819b871b88ef8d34aa77d82
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812181"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="44664-103">sectionLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="44664-103">sectionLinks resource type</span></span>

<span data-ttu-id="44664-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44664-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44664-105">用于打开 OneNote 分区的链接。</span><span class="sxs-lookup"><span data-stu-id="44664-105">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="44664-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44664-106">JSON representation</span></span>

<span data-ttu-id="44664-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44664-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="44664-108">属性</span><span class="sxs-lookup"><span data-stu-id="44664-108">Properties</span></span>
| <span data-ttu-id="44664-109">属性</span><span class="sxs-lookup"><span data-stu-id="44664-109">Property</span></span>     | <span data-ttu-id="44664-110">类型</span><span class="sxs-lookup"><span data-stu-id="44664-110">Type</span></span>   |<span data-ttu-id="44664-111">说明</span><span class="sxs-lookup"><span data-stu-id="44664-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44664-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="44664-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="44664-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="44664-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="44664-114">如果安装了 OneNote 本机客户端，则打开该分区。</span><span class="sxs-lookup"><span data-stu-id="44664-114">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="44664-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="44664-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="44664-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="44664-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="44664-117">打开 web 上的 OneNote 中的部分。</span><span class="sxs-lookup"><span data-stu-id="44664-117">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
