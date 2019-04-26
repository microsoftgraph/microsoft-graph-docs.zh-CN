---
title: externalLink 资源类型
description: 打开 OneNote 页面或笔记本的 url。
localization_priority: Normal
ms.openlocfilehash: d5658382585f5c7f7c5a9fe457e17976979091c6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333920"
---
# <a name="externallink-resource-type"></a><span data-ttu-id="04ee3-103">externalLink 资源类型</span><span class="sxs-lookup"><span data-stu-id="04ee3-103">externalLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04ee3-104">打开 OneNote 页面或笔记本的 url。</span><span class="sxs-lookup"><span data-stu-id="04ee3-104">A url that opens a OneNote page or notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04ee3-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04ee3-105">JSON representation</span></span>

<span data-ttu-id="04ee3-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04ee3-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalLink"
}-->

```json
{
  "href": "string"
}

```
## <a name="properties"></a><span data-ttu-id="04ee3-107">属性</span><span class="sxs-lookup"><span data-stu-id="04ee3-107">Properties</span></span>
| <span data-ttu-id="04ee3-108">属性</span><span class="sxs-lookup"><span data-stu-id="04ee3-108">Property</span></span>     | <span data-ttu-id="04ee3-109">类型</span><span class="sxs-lookup"><span data-stu-id="04ee3-109">Type</span></span>   |<span data-ttu-id="04ee3-110">说明</span><span class="sxs-lookup"><span data-stu-id="04ee3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04ee3-111">href</span><span class="sxs-lookup"><span data-stu-id="04ee3-111">href</span></span>|<span data-ttu-id="04ee3-112">String</span><span class="sxs-lookup"><span data-stu-id="04ee3-112">String</span></span>|<span data-ttu-id="04ee3-113">链接的 url。</span><span class="sxs-lookup"><span data-stu-id="04ee3-113">The url of the link.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "externalLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
