---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 4cb3a56b5bdb4c3e7c9fc9fe69c0b34cae134a0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805605"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="4d9f9-102">PublicationFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d9f9-102">PublicationFacet resource type</span></span>

> <span data-ttu-id="4d9f9-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4d9f9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d9f9-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4d9f9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d9f9-105">**publicationFacet** 资源提供有关 [driveItemVersion](driveitemversion.md) 或 [driveItem](driveitem.md) 资源发布状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="4d9f9-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d9f9-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d9f9-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4d9f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="4d9f9-107">Properties</span></span>

|   <span data-ttu-id="4d9f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d9f9-108">Property</span></span>    |  <span data-ttu-id="4d9f9-109">类型</span><span class="sxs-lookup"><span data-stu-id="4d9f9-109">Type</span></span>  | <span data-ttu-id="4d9f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="4d9f9-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="4d9f9-111">**level**</span><span class="sxs-lookup"><span data-stu-id="4d9f9-111">**level**</span></span>     | <span data-ttu-id="4d9f9-112">String</span><span class="sxs-lookup"><span data-stu-id="4d9f9-112">String</span></span> | <span data-ttu-id="4d9f9-113">此文档的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4d9f9-113">The state of publication for this document.</span></span> <span data-ttu-id="4d9f9-114">`published` 或 `checkout`。</span><span class="sxs-lookup"><span data-stu-id="4d9f9-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="4d9f9-115">只读。</span><span class="sxs-lookup"><span data-stu-id="4d9f9-115">Read-only.</span></span>  |
| <span data-ttu-id="4d9f9-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="4d9f9-116">**versionId**</span></span> | <span data-ttu-id="4d9f9-117">String</span><span class="sxs-lookup"><span data-stu-id="4d9f9-117">String</span></span> | <span data-ttu-id="4d9f9-118">对当前调用方可见的版本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4d9f9-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="4d9f9-119">只读。</span><span class="sxs-lookup"><span data-stu-id="4d9f9-119">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
