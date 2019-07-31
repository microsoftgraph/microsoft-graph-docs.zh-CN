---
author: JeremyKelley
description: publicationFacet 资源提供有关 driveItemVersion 或 driveItem 资源发布状态的详细信息。
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9c09f0863376e1569fb4af0acc0044fa1c7c8cfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008857"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="2cc7c-103">PublicationFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cc7c-103">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cc7c-104">**publicationFacet** 资源提供有关 [driveItemVersion](driveitemversion.md) 或 [driveItem](driveitem.md) 资源发布状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2cc7c-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cc7c-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cc7c-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2cc7c-106">属性</span><span class="sxs-lookup"><span data-stu-id="2cc7c-106">Properties</span></span>

|   <span data-ttu-id="2cc7c-107">属性</span><span class="sxs-lookup"><span data-stu-id="2cc7c-107">Property</span></span>    |  <span data-ttu-id="2cc7c-108">类型</span><span class="sxs-lookup"><span data-stu-id="2cc7c-108">Type</span></span>  | <span data-ttu-id="2cc7c-109">说明</span><span class="sxs-lookup"><span data-stu-id="2cc7c-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="2cc7c-110">**level**</span><span class="sxs-lookup"><span data-stu-id="2cc7c-110">**level**</span></span>     | <span data-ttu-id="2cc7c-111">String</span><span class="sxs-lookup"><span data-stu-id="2cc7c-111">String</span></span> | <span data-ttu-id="2cc7c-112">此文档的发布状态。</span><span class="sxs-lookup"><span data-stu-id="2cc7c-112">The state of publication for this document.</span></span> <span data-ttu-id="2cc7c-113">`published` 或 `checkout`。</span><span class="sxs-lookup"><span data-stu-id="2cc7c-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="2cc7c-114">只读。</span><span class="sxs-lookup"><span data-stu-id="2cc7c-114">Read-only.</span></span>  |
| <span data-ttu-id="2cc7c-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="2cc7c-115">**versionId**</span></span> | <span data-ttu-id="2cc7c-116">String</span><span class="sxs-lookup"><span data-stu-id="2cc7c-116">String</span></span> | <span data-ttu-id="2cc7c-117">对当前调用方可见的版本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2cc7c-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="2cc7c-118">只读。</span><span class="sxs-lookup"><span data-stu-id="2cc7c-118">Read-only.</span></span>  |


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
