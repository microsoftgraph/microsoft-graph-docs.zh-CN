---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: a95ec524b8e33ce65d9ecb7030a90a49305cdf6c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344058"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="83677-102">PublicationFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="83677-102">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83677-103">**publicationFacet** 资源提供有关 [driveItemVersion](driveitemversion.md) 或 [driveItem](driveitem.md) 资源发布状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="83677-103">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="83677-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83677-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="83677-105">属性</span><span class="sxs-lookup"><span data-stu-id="83677-105">Properties</span></span>

|   <span data-ttu-id="83677-106">属性</span><span class="sxs-lookup"><span data-stu-id="83677-106">Property</span></span>    |  <span data-ttu-id="83677-107">类型</span><span class="sxs-lookup"><span data-stu-id="83677-107">Type</span></span>  | <span data-ttu-id="83677-108">说明</span><span class="sxs-lookup"><span data-stu-id="83677-108">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="83677-109">**level**</span><span class="sxs-lookup"><span data-stu-id="83677-109">**level**</span></span>     | <span data-ttu-id="83677-110">String</span><span class="sxs-lookup"><span data-stu-id="83677-110">String</span></span> | <span data-ttu-id="83677-111">此文档的发布状态。</span><span class="sxs-lookup"><span data-stu-id="83677-111">The state of publication for this document.</span></span> <span data-ttu-id="83677-112">`published` 或 `checkout`。</span><span class="sxs-lookup"><span data-stu-id="83677-112">Either `published` or `checkout`.</span></span> <span data-ttu-id="83677-113">只读。</span><span class="sxs-lookup"><span data-stu-id="83677-113">Read-only.</span></span>  |
| <span data-ttu-id="83677-114">**versionId**</span><span class="sxs-lookup"><span data-stu-id="83677-114">**versionId**</span></span> | <span data-ttu-id="83677-115">String</span><span class="sxs-lookup"><span data-stu-id="83677-115">String</span></span> | <span data-ttu-id="83677-116">对当前调用方可见的版本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="83677-116">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="83677-117">只读。</span><span class="sxs-lookup"><span data-stu-id="83677-117">Read-only.</span></span>  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
