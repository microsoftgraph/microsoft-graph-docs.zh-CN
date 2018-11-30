---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
ms.openlocfilehash: e9bb612e20bc3d2416503f571f5abf364215efb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044474"
---
# <a name="webpart-resource"></a><span data-ttu-id="9b51c-102">web 部件资源</span><span class="sxs-lookup"><span data-stu-id="9b51c-102">webPart resource</span></span>

> <span data-ttu-id="9b51c-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9b51c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b51c-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9b51c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b51c-105">**Web 部件**资源表示类型和呈现[sitePage](sitepage.md)web 部件的信息。</span><span class="sxs-lookup"><span data-stu-id="9b51c-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b51c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b51c-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="9b51c-107">属性</span><span class="sxs-lookup"><span data-stu-id="9b51c-107">Properties</span></span>

| <span data-ttu-id="9b51c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9b51c-108">Property</span></span>                | <span data-ttu-id="9b51c-109">类型</span><span class="sxs-lookup"><span data-stu-id="9b51c-109">Type</span></span>             | <span data-ttu-id="9b51c-110">说明</span><span class="sxs-lookup"><span data-stu-id="9b51c-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="9b51c-111">**类型**</span><span class="sxs-lookup"><span data-stu-id="9b51c-111">**type**</span></span>                | <span data-ttu-id="9b51c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="9b51c-112">String</span></span>           | <span data-ttu-id="9b51c-113">指定 web 部件类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9b51c-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="9b51c-114">只读。</span><span class="sxs-lookup"><span data-stu-id="9b51c-114">Read-only.</span></span>
| <span data-ttu-id="9b51c-115">**data**</span><span class="sxs-lookup"><span data-stu-id="9b51c-115">**data**</span></span>                | <span data-ttu-id="9b51c-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="9b51c-116">[sitePageData][]</span></span> | <span data-ttu-id="9b51c-117">所需的 web 部件 （随 web 部件） 属性</span><span class="sxs-lookup"><span data-stu-id="9b51c-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="9b51c-119">备注</span><span class="sxs-lookup"><span data-stu-id="9b51c-119">Remarks</span></span>

<span data-ttu-id="9b51c-120">Web 部件可以定义在**数据**下自己所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9b51c-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="9b51c-121">有关页面的详细信息，请参阅[sitePage](sitepage.md)。</span><span class="sxs-lookup"><span data-stu-id="9b51c-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
