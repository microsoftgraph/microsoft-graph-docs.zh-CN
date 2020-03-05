---
title: PublicationFacet 资源类型
description: '**publicationFacet** 资源提供有关 driveItemVersion 或 driveItem 资源发布状态的详细信息。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: defd2c9b06a0d866ce43bbd4a9e8b36bdad770fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447036"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="947e4-103">PublicationFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="947e4-103">PublicationFacet resource type</span></span>

<span data-ttu-id="947e4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="947e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="947e4-105">**publicationFacet** 资源提供有关 [driveItemVersion](driveitemversion.md) 或 [driveItem](driveitem.md) 资源发布状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="947e4-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="947e4-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="947e4-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="947e4-107">属性</span><span class="sxs-lookup"><span data-stu-id="947e4-107">Properties</span></span>

|   <span data-ttu-id="947e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="947e4-108">Property</span></span>    |  <span data-ttu-id="947e4-109">类型</span><span class="sxs-lookup"><span data-stu-id="947e4-109">Type</span></span>  | <span data-ttu-id="947e4-110">说明</span><span class="sxs-lookup"><span data-stu-id="947e4-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="947e4-111">**level**</span><span class="sxs-lookup"><span data-stu-id="947e4-111">**level**</span></span>     | <span data-ttu-id="947e4-112">String</span><span class="sxs-lookup"><span data-stu-id="947e4-112">String</span></span> | <span data-ttu-id="947e4-113">此文档的发布状态。</span><span class="sxs-lookup"><span data-stu-id="947e4-113">The state of publication for this document.</span></span> <span data-ttu-id="947e4-114">`published` 或 `checkout`。</span><span class="sxs-lookup"><span data-stu-id="947e4-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="947e4-115">只读。</span><span class="sxs-lookup"><span data-stu-id="947e4-115">Read-only.</span></span>  |
| <span data-ttu-id="947e4-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="947e4-116">**versionId**</span></span> | <span data-ttu-id="947e4-117">String</span><span class="sxs-lookup"><span data-stu-id="947e4-117">String</span></span> | <span data-ttu-id="947e4-118">对当前调用方可见的版本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="947e4-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="947e4-119">只读。</span><span class="sxs-lookup"><span data-stu-id="947e4-119">Read-only.</span></span>  |


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
