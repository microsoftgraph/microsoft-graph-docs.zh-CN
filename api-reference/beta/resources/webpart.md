---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453607"
---
# <a name="webpart-resource"></a><span data-ttu-id="0c883-102">webPart 资源</span><span class="sxs-lookup"><span data-stu-id="0c883-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c883-103">**webPart**资源表示[sitePage](sitepage.md)上的 web 部件的类型和呈现信息。</span><span class="sxs-lookup"><span data-stu-id="0c883-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c883-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c883-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0c883-105">属性</span><span class="sxs-lookup"><span data-stu-id="0c883-105">Properties</span></span>

| <span data-ttu-id="0c883-106">属性</span><span class="sxs-lookup"><span data-stu-id="0c883-106">Property</span></span>                | <span data-ttu-id="0c883-107">类型</span><span class="sxs-lookup"><span data-stu-id="0c883-107">Type</span></span>             | <span data-ttu-id="0c883-108">描述</span><span class="sxs-lookup"><span data-stu-id="0c883-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="0c883-109">**类型**</span><span class="sxs-lookup"><span data-stu-id="0c883-109">**type**</span></span>                | <span data-ttu-id="0c883-110">字符串</span><span class="sxs-lookup"><span data-stu-id="0c883-110">String</span></span>           | <span data-ttu-id="0c883-111">指定 web 部件类型的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0c883-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="0c883-112">只读。</span><span class="sxs-lookup"><span data-stu-id="0c883-112">Read-only.</span></span>
| <span data-ttu-id="0c883-113">**data**</span><span class="sxs-lookup"><span data-stu-id="0c883-113">**data**</span></span>                | <span data-ttu-id="0c883-114">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="0c883-114">[sitePageData][]</span></span> | <span data-ttu-id="0c883-115">web 部件的必需属性 (因 web 部件而异)</span><span class="sxs-lookup"><span data-stu-id="0c883-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="0c883-117">备注</span><span class="sxs-lookup"><span data-stu-id="0c883-117">Remarks</span></span>

<span data-ttu-id="0c883-118">Web 部件可以在**data**下定义自己的必需属性。</span><span class="sxs-lookup"><span data-stu-id="0c883-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="0c883-119">有关页面的详细信息, 请参阅[sitePage](sitepage.md)。</span><span class="sxs-lookup"><span data-stu-id="0c883-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
