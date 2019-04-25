---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: SitePageData
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 78661f5ce6336f4430297d8969ff8cd82b761c9a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583394"
---
# <a name="sitepagedata-resource"></a><span data-ttu-id="60a11-102">sitePageData 资源</span><span class="sxs-lookup"><span data-stu-id="60a11-102">sitePageData resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60a11-103">**sitePageData**资源表示[web 部件][]的属性。</span><span class="sxs-lookup"><span data-stu-id="60a11-103">The **sitePageData** resource represents the properties of a [webPart][].</span></span> <span data-ttu-id="60a11-104">由于这些属性因 web 部件而异, 这是没有固定属性的 OpenType。</span><span class="sxs-lookup"><span data-stu-id="60a11-104">As these properties vary by web part, this is an OpenType with no fixed properties.</span></span>

[.webpart]: webpart.md
[webPart]: webpart.md

## <a name="json-representation"></a><span data-ttu-id="60a11-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60a11-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sitePageData"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="60a11-107">属性</span><span class="sxs-lookup"><span data-stu-id="60a11-107">Properties</span></span>
<span data-ttu-id="60a11-108">此资源没有固定属性, 但它是包含定义 web 部件所需的所有属性的 OpenType。</span><span class="sxs-lookup"><span data-stu-id="60a11-108">This resource has no fixed properties, but is an OpenType containing all properties necessary to define a web part.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Defines the data in a web part",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/SitePageData",
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepagedata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
