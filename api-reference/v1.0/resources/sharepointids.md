---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
description: SharePointIds 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。
doc_type: resourcePageType
ms.openlocfilehash: a7dfd936770ac85b458cb8b086ff05e328d2ea9c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034277"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="47a4a-103">SharePointIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="47a4a-103">SharePointIds resource type</span></span>

<span data-ttu-id="47a4a-104">**SharePointIds** 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="47a4a-104">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="47a4a-105">**注意：** OneDrive 个人版返回的项将不包括 **SharePointIds** 方面。</span><span class="sxs-lookup"><span data-stu-id="47a4a-105">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47a4a-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47a4a-106">JSON representation</span></span>

<span data-ttu-id="47a4a-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47a4a-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="47a4a-108">属性</span><span class="sxs-lookup"><span data-stu-id="47a4a-108">Properties</span></span>

| <span data-ttu-id="47a4a-109">属性</span><span class="sxs-lookup"><span data-stu-id="47a4a-109">Property</span></span>         | <span data-ttu-id="47a4a-110">类型</span><span class="sxs-lookup"><span data-stu-id="47a4a-110">Type</span></span>         | <span data-ttu-id="47a4a-111">说明</span><span class="sxs-lookup"><span data-stu-id="47a4a-111">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="47a4a-112">listId</span><span class="sxs-lookup"><span data-stu-id="47a4a-112">listId</span></span>           | <span data-ttu-id="47a4a-113">string</span><span class="sxs-lookup"><span data-stu-id="47a4a-113">string</span></span>       | <span data-ttu-id="47a4a-114">SharePoint 中的项列表的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="47a4a-114">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="47a4a-115">listItemId</span><span class="sxs-lookup"><span data-stu-id="47a4a-115">listItemId</span></span>       | <span data-ttu-id="47a4a-116">string</span><span class="sxs-lookup"><span data-stu-id="47a4a-116">string</span></span>       | <span data-ttu-id="47a4a-117">包含列表中的项的整数标识符。</span><span class="sxs-lookup"><span data-stu-id="47a4a-117">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="47a4a-118">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="47a4a-118">listItemUniqueId</span></span> | <span data-ttu-id="47a4a-119">string</span><span class="sxs-lookup"><span data-stu-id="47a4a-119">string</span></span>       | <span data-ttu-id="47a4a-120">OneDrive for Business 或 SharePoint 网站中的项的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="47a4a-120">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="47a4a-121">siteId</span><span class="sxs-lookup"><span data-stu-id="47a4a-121">siteId</span></span>           | <span data-ttu-id="47a4a-122">string</span><span class="sxs-lookup"><span data-stu-id="47a4a-122">string</span></span>       | <span data-ttu-id="47a4a-123">项的网站集 (SPSite) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="47a4a-123">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="47a4a-124">siteUrl</span><span class="sxs-lookup"><span data-stu-id="47a4a-124">siteUrl</span></span>          | <span data-ttu-id="47a4a-125">string (url)</span><span class="sxs-lookup"><span data-stu-id="47a4a-125">string (url)</span></span> | <span data-ttu-id="47a4a-126">包含项的网站的 SharePoint URL。</span><span class="sxs-lookup"><span data-stu-id="47a4a-126">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="47a4a-127">webId</span><span class="sxs-lookup"><span data-stu-id="47a4a-127">webId</span></span>            | <span data-ttu-id="47a4a-128">string</span><span class="sxs-lookup"><span data-stu-id="47a4a-128">string</span></span>       | <span data-ttu-id="47a4a-129">项的网站集 (SPWeb) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="47a4a-129">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="47a4a-130">注解</span><span class="sxs-lookup"><span data-stu-id="47a4a-130">Remarks</span></span>

<span data-ttu-id="47a4a-131">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="47a4a-131">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
