---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e7bbd0f6aa8d4ea04304d6aecae97b98ab0a46b7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574276"
---
# <a name="webpart-resource"></a><span data-ttu-id="82f5d-102">web 部件资源</span><span class="sxs-lookup"><span data-stu-id="82f5d-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82f5d-103">**Web 部件**资源表示类型和呈现[sitePage](sitepage.md)web 部件的信息。</span><span class="sxs-lookup"><span data-stu-id="82f5d-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="82f5d-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82f5d-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  
    ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "String (identifier)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="82f5d-105">属性</span><span class="sxs-lookup"><span data-stu-id="82f5d-105">Properties</span></span>

| <span data-ttu-id="82f5d-106">属性</span><span class="sxs-lookup"><span data-stu-id="82f5d-106">Property</span></span>                | <span data-ttu-id="82f5d-107">类型</span><span class="sxs-lookup"><span data-stu-id="82f5d-107">Type</span></span>             | <span data-ttu-id="82f5d-108">说明</span><span class="sxs-lookup"><span data-stu-id="82f5d-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="82f5d-109">**类型**</span><span class="sxs-lookup"><span data-stu-id="82f5d-109">**type**</span></span>                | <span data-ttu-id="82f5d-110">字符串 （标识符）</span><span class="sxs-lookup"><span data-stu-id="82f5d-110">String (identifier)</span></span>         | <span data-ttu-id="82f5d-111">指定 web 部件类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="82f5d-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="82f5d-112">只读。</span><span class="sxs-lookup"><span data-stu-id="82f5d-112">Read-only.</span></span>
| <span data-ttu-id="82f5d-113">**data**</span><span class="sxs-lookup"><span data-stu-id="82f5d-113">**data**</span></span>                | [<span data-ttu-id="82f5d-114">sitePageData</span><span class="sxs-lookup"><span data-stu-id="82f5d-114">sitePageData</span></span>](sitepagedata.md) | <span data-ttu-id="82f5d-115">所需的 web 部件 （随 web 部件） 属性</span><span class="sxs-lookup"><span data-stu-id="82f5d-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="82f5d-116">说明</span><span class="sxs-lookup"><span data-stu-id="82f5d-116">Remarks</span></span>

<span data-ttu-id="82f5d-117">Web 部件可以定义在**数据**下自己所需的属性。</span><span class="sxs-lookup"><span data-stu-id="82f5d-117">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="82f5d-118">有关页面的详细信息，请参阅[sitePage](sitepage.md)。</span><span class="sxs-lookup"><span data-stu-id="82f5d-118">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
