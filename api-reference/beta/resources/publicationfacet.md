---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
ms.openlocfilehash: 60dff1e0dd97073ccb7eccd7be0f51b6b77fc273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045569"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="14f61-102">PublicationFacet 资源类型</span><span class="sxs-lookup"><span data-stu-id="14f61-102">PublicationFacet resource type</span></span>

> <span data-ttu-id="14f61-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="14f61-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14f61-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="14f61-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="14f61-105">**publicationFacet** 资源提供有关 [driveItemVersion](driveitemversion.md) 或 [driveItem](driveitem.md) 资源发布状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="14f61-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="14f61-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14f61-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="14f61-107">属性</span><span class="sxs-lookup"><span data-stu-id="14f61-107">Properties</span></span>

|   <span data-ttu-id="14f61-108">属性</span><span class="sxs-lookup"><span data-stu-id="14f61-108">Property</span></span>    |  <span data-ttu-id="14f61-109">类型</span><span class="sxs-lookup"><span data-stu-id="14f61-109">Type</span></span>  | <span data-ttu-id="14f61-110">说明</span><span class="sxs-lookup"><span data-stu-id="14f61-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="14f61-111">**level**</span><span class="sxs-lookup"><span data-stu-id="14f61-111">**level**</span></span>     | <span data-ttu-id="14f61-112">String</span><span class="sxs-lookup"><span data-stu-id="14f61-112">String</span></span> | <span data-ttu-id="14f61-113">此文档的发布状态。</span><span class="sxs-lookup"><span data-stu-id="14f61-113">The state of publication for this document.</span></span> <span data-ttu-id="14f61-114">`published` 或 `checkout`。</span><span class="sxs-lookup"><span data-stu-id="14f61-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="14f61-115">只读。</span><span class="sxs-lookup"><span data-stu-id="14f61-115">Read-only.</span></span>  |
| <span data-ttu-id="14f61-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="14f61-116">**versionId**</span></span> | <span data-ttu-id="14f61-117">String</span><span class="sxs-lookup"><span data-stu-id="14f61-117">String</span></span> | <span data-ttu-id="14f61-118">对当前调用方可见的版本的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="14f61-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="14f61-119">只读。</span><span class="sxs-lookup"><span data-stu-id="14f61-119">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
