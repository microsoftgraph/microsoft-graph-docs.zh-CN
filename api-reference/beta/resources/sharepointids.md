---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.openlocfilehash: 6c67c45b333ead1d427c5b15ddd4ed5925b84eac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807810"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="099b8-102">SharePointIds 资源类型</span><span class="sxs-lookup"><span data-stu-id="099b8-102">SharePointIds resource type</span></span>

> <span data-ttu-id="099b8-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="099b8-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="099b8-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="099b8-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="099b8-105">**SharePointIds** 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="099b8-105">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="099b8-106">**注意：** OneDrive 个人版返回的项将不包括 **SharePointIds** 方面。</span><span class="sxs-lookup"><span data-stu-id="099b8-106">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="099b8-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="099b8-107">JSON representation</span></span>

<span data-ttu-id="099b8-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="099b8-108">Here is a JSON representation of the resource</span></span>

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
    "tenantId": "string",
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="099b8-109">属性</span><span class="sxs-lookup"><span data-stu-id="099b8-109">Properties</span></span>

| <span data-ttu-id="099b8-110">属性</span><span class="sxs-lookup"><span data-stu-id="099b8-110">Property</span></span>         | <span data-ttu-id="099b8-111">类型</span><span class="sxs-lookup"><span data-stu-id="099b8-111">Type</span></span>         | <span data-ttu-id="099b8-112">说明</span><span class="sxs-lookup"><span data-stu-id="099b8-112">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="099b8-113">listId</span><span class="sxs-lookup"><span data-stu-id="099b8-113">listId</span></span>           | <span data-ttu-id="099b8-114">string</span><span class="sxs-lookup"><span data-stu-id="099b8-114">string</span></span>       | <span data-ttu-id="099b8-115">SharePoint 中的项列表的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="099b8-115">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="099b8-116">listItemId</span><span class="sxs-lookup"><span data-stu-id="099b8-116">listItemId</span></span>       | <span data-ttu-id="099b8-117">string</span><span class="sxs-lookup"><span data-stu-id="099b8-117">string</span></span>       | <span data-ttu-id="099b8-118">包含列表中的项的整数标识符。</span><span class="sxs-lookup"><span data-stu-id="099b8-118">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="099b8-119">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="099b8-119">listItemUniqueId</span></span> | <span data-ttu-id="099b8-120">string</span><span class="sxs-lookup"><span data-stu-id="099b8-120">string</span></span>       | <span data-ttu-id="099b8-121">OneDrive for Business 或 SharePoint 网站中的项的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="099b8-121">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="099b8-122">siteId</span><span class="sxs-lookup"><span data-stu-id="099b8-122">siteId</span></span>           | <span data-ttu-id="099b8-123">string</span><span class="sxs-lookup"><span data-stu-id="099b8-123">string</span></span>       | <span data-ttu-id="099b8-124">项的网站集 (SPSite) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="099b8-124">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="099b8-125">siteUrl</span><span class="sxs-lookup"><span data-stu-id="099b8-125">siteUrl</span></span>          | <span data-ttu-id="099b8-126">string (url)</span><span class="sxs-lookup"><span data-stu-id="099b8-126">string (url)</span></span> | <span data-ttu-id="099b8-127">包含项的网站的 SharePoint URL。</span><span class="sxs-lookup"><span data-stu-id="099b8-127">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="099b8-128">tenantId</span><span class="sxs-lookup"><span data-stu-id="099b8-128">tenantId</span></span>         | <span data-ttu-id="099b8-129">string</span><span class="sxs-lookup"><span data-stu-id="099b8-129">string</span></span>       | <span data-ttu-id="099b8-130">租户的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="099b8-130">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="099b8-131">webId</span><span class="sxs-lookup"><span data-stu-id="099b8-131">webId</span></span>            | <span data-ttu-id="099b8-132">string</span><span class="sxs-lookup"><span data-stu-id="099b8-132">string</span></span>       | <span data-ttu-id="099b8-133">项的网站集 (SPWeb) 的唯一标识符 (guid)。</span><span class="sxs-lookup"><span data-stu-id="099b8-133">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="099b8-134">注解</span><span class="sxs-lookup"><span data-stu-id="099b8-134">Remarks</span></span>

<span data-ttu-id="099b8-135">有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="099b8-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
