---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03b5f1007d8dbe6587da736cdf0ac0fdc1ed8a55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345784"
---
# <a name="webpart-resource"></a><span data-ttu-id="c9fc7-102">webPart 资源</span><span class="sxs-lookup"><span data-stu-id="c9fc7-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9fc7-103">**webPart**资源表示[sitePage](sitepage.md)上的 web 部件的类型和呈现信息。</span><span class="sxs-lookup"><span data-stu-id="c9fc7-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9fc7-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9fc7-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (identifier)",
  "data": {"@odata.type":"microsoft.graph.sitePageData"}
}
```

## <a name="properties"></a><span data-ttu-id="c9fc7-105">属性</span><span class="sxs-lookup"><span data-stu-id="c9fc7-105">Properties</span></span>

| <span data-ttu-id="c9fc7-106">属性</span><span class="sxs-lookup"><span data-stu-id="c9fc7-106">Property</span></span>                | <span data-ttu-id="c9fc7-107">类型</span><span class="sxs-lookup"><span data-stu-id="c9fc7-107">Type</span></span>             | <span data-ttu-id="c9fc7-108">说明</span><span class="sxs-lookup"><span data-stu-id="c9fc7-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="c9fc7-109">**类型**</span><span class="sxs-lookup"><span data-stu-id="c9fc7-109">**type**</span></span>                | <span data-ttu-id="c9fc7-110">String</span><span class="sxs-lookup"><span data-stu-id="c9fc7-110">String</span></span>           | <span data-ttu-id="c9fc7-111">指定 web 部件类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c9fc7-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="c9fc7-112">只读。</span><span class="sxs-lookup"><span data-stu-id="c9fc7-112">Read-only.</span></span>
| <span data-ttu-id="c9fc7-113">**data**</span><span class="sxs-lookup"><span data-stu-id="c9fc7-113">**data**</span></span>                | <span data-ttu-id="c9fc7-114">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="c9fc7-114">[sitePageData][]</span></span> | <span data-ttu-id="c9fc7-115">web 部件的必需属性 (因 web 部件而异)</span><span class="sxs-lookup"><span data-stu-id="c9fc7-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="c9fc7-117">注解</span><span class="sxs-lookup"><span data-stu-id="c9fc7-117">Remarks</span></span>

<span data-ttu-id="c9fc7-118">Web 部件可以在**data**下定义自己的必需属性。</span><span class="sxs-lookup"><span data-stu-id="c9fc7-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="c9fc7-119">有关页面的详细信息, 请参阅[sitePage](sitepage.md)。</span><span class="sxs-lookup"><span data-stu-id="c9fc7-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": []
}
-->
