---
author: rahmit
description: WebPart 资源表示 sitePage 上的 web 部件的类型和呈现信息。
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71626440abe9eb63af3419b3e65c4351ae442dea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007352"
---
# <a name="webpart-resource"></a><span data-ttu-id="3d0f2-103">webPart 资源</span><span class="sxs-lookup"><span data-stu-id="3d0f2-103">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d0f2-104">**WebPart**资源表示[sitePage](sitepage.md)上的 web 部件的类型和呈现信息。</span><span class="sxs-lookup"><span data-stu-id="3d0f2-104">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d0f2-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d0f2-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3d0f2-106">属性</span><span class="sxs-lookup"><span data-stu-id="3d0f2-106">Properties</span></span>

| <span data-ttu-id="3d0f2-107">属性</span><span class="sxs-lookup"><span data-stu-id="3d0f2-107">Property</span></span>                | <span data-ttu-id="3d0f2-108">类型</span><span class="sxs-lookup"><span data-stu-id="3d0f2-108">Type</span></span>             | <span data-ttu-id="3d0f2-109">说明</span><span class="sxs-lookup"><span data-stu-id="3d0f2-109">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="3d0f2-110">**类型**</span><span class="sxs-lookup"><span data-stu-id="3d0f2-110">**type**</span></span>                | <span data-ttu-id="3d0f2-111">String</span><span class="sxs-lookup"><span data-stu-id="3d0f2-111">String</span></span>           | <span data-ttu-id="3d0f2-112">指定 Web 部件类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3d0f2-112">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="3d0f2-113">只读。</span><span class="sxs-lookup"><span data-stu-id="3d0f2-113">Read-only.</span></span>
| <span data-ttu-id="3d0f2-114">**data**</span><span class="sxs-lookup"><span data-stu-id="3d0f2-114">**data**</span></span>                | <span data-ttu-id="3d0f2-115">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="3d0f2-115">[sitePageData][]</span></span> | <span data-ttu-id="3d0f2-116">Web 部件的必需属性 (因 Web 部件而异)</span><span class="sxs-lookup"><span data-stu-id="3d0f2-116">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="3d0f2-118">说明</span><span class="sxs-lookup"><span data-stu-id="3d0f2-118">Remarks</span></span>

<span data-ttu-id="3d0f2-119">Web 部件可以在**data**下定义自己的必需属性。</span><span class="sxs-lookup"><span data-stu-id="3d0f2-119">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="3d0f2-120">有关页面的详细信息, 请参阅[sitePage](sitepage.md)。</span><span class="sxs-lookup"><span data-stu-id="3d0f2-120">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
