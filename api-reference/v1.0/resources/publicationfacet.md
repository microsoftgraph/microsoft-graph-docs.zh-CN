---
title: PublicationFacet 资源类型
description: '**publicationFacet** 资源提供有关 driveItemVersion 或 driveItem 资源发布状态的详细信息。'
ms.openlocfilehash: 429ec649dc9f511a4012e6790842fdd774bead8b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008193"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="4cedf-103">PublicationFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cedf-103">PublicationFacet resource type</span></span>

<span data-ttu-id="4cedf-104">**publicationFacet** 资源提供有关 [driveItemVersion](driveitemversion.md) 或 [driveItem](driveitem.md) 资源发布状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4cedf-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cedf-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cedf-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4cedf-106">属性</span><span class="sxs-lookup"><span data-stu-id="4cedf-106">Properties</span></span>

|   <span data-ttu-id="4cedf-107">属性</span><span class="sxs-lookup"><span data-stu-id="4cedf-107">Property</span></span>    |  <span data-ttu-id="4cedf-108">类型</span><span class="sxs-lookup"><span data-stu-id="4cedf-108">Type</span></span>  | <span data-ttu-id="4cedf-109">说明</span><span class="sxs-lookup"><span data-stu-id="4cedf-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="4cedf-110">**level**</span><span class="sxs-lookup"><span data-stu-id="4cedf-110">**level**</span></span>     | <span data-ttu-id="4cedf-111">String</span><span class="sxs-lookup"><span data-stu-id="4cedf-111">String</span></span> | <span data-ttu-id="4cedf-112">此文档的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4cedf-112">The state of publication for this document.</span></span> <span data-ttu-id="4cedf-113">`published` 或 `checkout`。</span><span class="sxs-lookup"><span data-stu-id="4cedf-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="4cedf-114">只读。</span><span class="sxs-lookup"><span data-stu-id="4cedf-114">Read-only.</span></span>  |
| <span data-ttu-id="4cedf-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="4cedf-115">**versionId**</span></span> | <span data-ttu-id="4cedf-116">String</span><span class="sxs-lookup"><span data-stu-id="4cedf-116">String</span></span> | <span data-ttu-id="4cedf-117">对当前调用方可见的版本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4cedf-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="4cedf-118">只读。</span><span class="sxs-lookup"><span data-stu-id="4cedf-118">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
