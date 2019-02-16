---
title: locationDataModel 资源类型
description: 表示事件的 locationDataModel 信息。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2b1fd0c25cdd41e6a8d9c87f8a1c0c80d70b78e5
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057343"
---
# <a name="locationdatamodel-resource-type"></a><span data-ttu-id="9b02d-103">locationDataModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b02d-103">locationDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b02d-104">表示会议的位置信息。</span><span class="sxs-lookup"><span data-stu-id="9b02d-104">Represents location information for a meeting.</span></span>


## <a name="properties"></a><span data-ttu-id="9b02d-105">属性</span><span class="sxs-lookup"><span data-stu-id="9b02d-105">Properties</span></span>
| <span data-ttu-id="9b02d-106">属性</span><span class="sxs-lookup"><span data-stu-id="9b02d-106">Property</span></span>  | <span data-ttu-id="9b02d-107">类型</span><span class="sxs-lookup"><span data-stu-id="9b02d-107">Type</span></span>   | <span data-ttu-id="9b02d-108">说明</span><span class="sxs-lookup"><span data-stu-id="9b02d-108">Description</span></span>                                                     |
|:----------|:-------|:----------------------------------------------------------------|
| <span data-ttu-id="9b02d-109">address</span><span class="sxs-lookup"><span data-stu-id="9b02d-109">address</span></span> | [<span data-ttu-id="9b02d-110">省略</span><span class="sxs-lookup"><span data-stu-id="9b02d-110">postalAddress</span></span>](postaladdress.md) |<span data-ttu-id="9b02d-111">位置的街道地址。</span><span class="sxs-lookup"><span data-stu-id="9b02d-111">The street address of the location.</span></span> |
| <span data-ttu-id="9b02d-112">coordinates</span><span class="sxs-lookup"><span data-stu-id="9b02d-112">coordinates</span></span> | [<span data-ttu-id="9b02d-113">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="9b02d-113">outlookGeoCoordinates</span></span>](outlookgeocoordinates.md) | <span data-ttu-id="9b02d-114">地理坐标和位置的海拔高度。</span><span class="sxs-lookup"><span data-stu-id="9b02d-114">The geographic coordinates and elevation of the location.</span></span> |
| <span data-ttu-id="9b02d-115">displayName</span><span class="sxs-lookup"><span data-stu-id="9b02d-115">displayName</span></span>  | <span data-ttu-id="9b02d-116">字符串</span><span class="sxs-lookup"><span data-stu-id="9b02d-116">String</span></span> | <span data-ttu-id="9b02d-117">与地点相关联的名称。</span><span class="sxs-lookup"><span data-stu-id="9b02d-117">The name associated with the location.</span></span>                       |
| <span data-ttu-id="9b02d-118">locationEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9b02d-118">locationEmailAddress</span></span> | <span data-ttu-id="9b02d-119">String</span><span class="sxs-lookup"><span data-stu-id="9b02d-119">String</span></span> | <span data-ttu-id="9b02d-120">（可选）与位置相关联的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9b02d-120">Optional email address of the location.</span></span> |
| <span data-ttu-id="9b02d-121">locationUri</span><span class="sxs-lookup"><span data-stu-id="9b02d-121">locationUri</span></span> | <span data-ttu-id="9b02d-122">String</span><span class="sxs-lookup"><span data-stu-id="9b02d-122">String</span></span> | <span data-ttu-id="9b02d-123">（可选）表示位置的 URI。</span><span class="sxs-lookup"><span data-stu-id="9b02d-123">Optional URI representing the location.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="9b02d-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b02d-124">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationDataModel"
}-->
```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "coordinates": {"@odata.type": "microsoft.graph.outlookGeoCoordinates"},
  "displayName": "string",
  "locationEmailAddress": "string",
  "locationUri": "string"
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/locationdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
