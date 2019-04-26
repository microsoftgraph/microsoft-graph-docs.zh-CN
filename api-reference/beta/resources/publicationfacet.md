---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 66e12c3240d1cade57d377e43403b33102fe166e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563245"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="0f8c5-102">PublicationFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f8c5-102">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f8c5-103">**publicationFacet** 资源提供有关 [driveItemVersion](driveitemversion.md) 或 [driveItem](driveitem.md) 资源发布状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0f8c5-103">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f8c5-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f8c5-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="0f8c5-105">属性</span><span class="sxs-lookup"><span data-stu-id="0f8c5-105">Properties</span></span>

|   <span data-ttu-id="0f8c5-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f8c5-106">Property</span></span>    |  <span data-ttu-id="0f8c5-107">类型</span><span class="sxs-lookup"><span data-stu-id="0f8c5-107">Type</span></span>  | <span data-ttu-id="0f8c5-108">说明</span><span class="sxs-lookup"><span data-stu-id="0f8c5-108">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="0f8c5-109">**level**</span><span class="sxs-lookup"><span data-stu-id="0f8c5-109">**level**</span></span>     | <span data-ttu-id="0f8c5-110">String</span><span class="sxs-lookup"><span data-stu-id="0f8c5-110">String</span></span> | <span data-ttu-id="0f8c5-111">此文档的发布状态。</span><span class="sxs-lookup"><span data-stu-id="0f8c5-111">The state of publication for this document.</span></span> <span data-ttu-id="0f8c5-112">`published` 或 `checkout`。</span><span class="sxs-lookup"><span data-stu-id="0f8c5-112">Either `published` or `checkout`.</span></span> <span data-ttu-id="0f8c5-113">只读。</span><span class="sxs-lookup"><span data-stu-id="0f8c5-113">Read-only.</span></span>  |
| <span data-ttu-id="0f8c5-114">**versionId**</span><span class="sxs-lookup"><span data-stu-id="0f8c5-114">**versionId**</span></span> | <span data-ttu-id="0f8c5-115">String</span><span class="sxs-lookup"><span data-stu-id="0f8c5-115">String</span></span> | <span data-ttu-id="0f8c5-116">对当前调用方可见的版本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0f8c5-116">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="0f8c5-117">只读。</span><span class="sxs-lookup"><span data-stu-id="0f8c5-117">Read-only.</span></span>  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicationfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
