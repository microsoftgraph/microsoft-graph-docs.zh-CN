---
author: rahmit
description: WebPart 资源表示 sitePage 上的 web 部件的类型和呈现信息。
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: efcf6aa1db31246af607cda85aa799fcc6804a34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519433"
---
# <a name="webpart-resource"></a><span data-ttu-id="e5c57-103">webPart 资源</span><span class="sxs-lookup"><span data-stu-id="e5c57-103">webPart resource</span></span>

<span data-ttu-id="e5c57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5c57-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5c57-105">**WebPart**资源表示[sitePage](sitepage.md)上的 web 部件的类型和呈现信息。</span><span class="sxs-lookup"><span data-stu-id="e5c57-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5c57-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5c57-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e5c57-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5c57-107">Properties</span></span>

| <span data-ttu-id="e5c57-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5c57-108">Property</span></span>                | <span data-ttu-id="e5c57-109">类型</span><span class="sxs-lookup"><span data-stu-id="e5c57-109">Type</span></span>             | <span data-ttu-id="e5c57-110">说明</span><span class="sxs-lookup"><span data-stu-id="e5c57-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="e5c57-111">**类型**</span><span class="sxs-lookup"><span data-stu-id="e5c57-111">**type**</span></span>                | <span data-ttu-id="e5c57-112">String</span><span class="sxs-lookup"><span data-stu-id="e5c57-112">String</span></span>           | <span data-ttu-id="e5c57-113">指定 Web 部件类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e5c57-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="e5c57-114">只读。</span><span class="sxs-lookup"><span data-stu-id="e5c57-114">Read-only.</span></span>
| <span data-ttu-id="e5c57-115">**data**</span><span class="sxs-lookup"><span data-stu-id="e5c57-115">**data**</span></span>                | <span data-ttu-id="e5c57-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="e5c57-116">[sitePageData][]</span></span> | <span data-ttu-id="e5c57-117">Web 部件 (的必需属性因 Web 部件而异) </span><span class="sxs-lookup"><span data-stu-id="e5c57-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="e5c57-119">说明</span><span class="sxs-lookup"><span data-stu-id="e5c57-119">Remarks</span></span>

<span data-ttu-id="e5c57-120">Web 部件可以在**data**下定义自己的必需属性。</span><span class="sxs-lookup"><span data-stu-id="e5c57-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="e5c57-121">有关页面的详细信息，请参阅[sitePage](sitepage.md)。</span><span class="sxs-lookup"><span data-stu-id="e5c57-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
