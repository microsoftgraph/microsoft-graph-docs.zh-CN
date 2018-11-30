---
title: sectionLinks 资源类型
description: 用于打开 OneNote 分区的链接。
ms.openlocfilehash: 26dbffd6f3bde9c05efabc737852c3619cc1e275
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046796"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="2f3ae-103">sectionLinks 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f3ae-103">sectionLinks resource type</span></span>

> <span data-ttu-id="2f3ae-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2f3ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f3ae-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2f3ae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f3ae-106">用于打开 OneNote 分区的链接。</span><span class="sxs-lookup"><span data-stu-id="2f3ae-106">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f3ae-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f3ae-107">JSON representation</span></span>

<span data-ttu-id="2f3ae-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f3ae-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2f3ae-109">属性</span><span class="sxs-lookup"><span data-stu-id="2f3ae-109">Properties</span></span>
| <span data-ttu-id="2f3ae-110">属性</span><span class="sxs-lookup"><span data-stu-id="2f3ae-110">Property</span></span>     | <span data-ttu-id="2f3ae-111">类型</span><span class="sxs-lookup"><span data-stu-id="2f3ae-111">Type</span></span>   |<span data-ttu-id="2f3ae-112">说明</span><span class="sxs-lookup"><span data-stu-id="2f3ae-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f3ae-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="2f3ae-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="2f3ae-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="2f3ae-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="2f3ae-115">如果安装了 OneNote 本机客户端，则在其中打开分区。</span><span class="sxs-lookup"><span data-stu-id="2f3ae-115">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="2f3ae-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="2f3ae-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="2f3ae-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="2f3ae-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="2f3ae-118">在 OneNote Online 中打开分区。</span><span class="sxs-lookup"><span data-stu-id="2f3ae-118">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->