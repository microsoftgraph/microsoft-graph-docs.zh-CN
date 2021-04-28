---
title: 目录资源类型
description: 表示可以批准部署的内容目录的实体。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3fc0630a36d123e6c3e208838d81ee7c33c62853
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067981"
---
# <a name="catalog-resource-type"></a><span data-ttu-id="ebc4f-103">目录资源类型</span><span class="sxs-lookup"><span data-stu-id="ebc4f-103">catalog resource type</span></span>

<span data-ttu-id="ebc4f-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="ebc4f-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebc4f-105">表示可以批准部署的内容目录的实体。</span><span class="sxs-lookup"><span data-stu-id="ebc4f-105">Entity representing the catalog of content that you can approve for deployment.</span></span>

## <a name="methods"></a><span data-ttu-id="ebc4f-106">方法</span><span class="sxs-lookup"><span data-stu-id="ebc4f-106">Methods</span></span>
|<span data-ttu-id="ebc4f-107">方法</span><span class="sxs-lookup"><span data-stu-id="ebc4f-107">Method</span></span>|<span data-ttu-id="ebc4f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="ebc4f-108">Return type</span></span>|<span data-ttu-id="ebc4f-109">说明</span><span class="sxs-lookup"><span data-stu-id="ebc4f-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ebc4f-110">列表条目</span><span class="sxs-lookup"><span data-stu-id="ebc4f-110">List entries</span></span>](../api/windowsupdates-catalog-list-entries.md)|<span data-ttu-id="ebc4f-111">[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebc4f-111">[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) collection</span></span>|<span data-ttu-id="ebc4f-112">从条目导航属性获取 [catalogEntry](../resources/windowsupdates-catalogentry.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="ebc4f-112">Get the [catalogEntry](../resources/windowsupdates-catalogentry.md) resources from the entries navigation property.</span></span> <span data-ttu-id="ebc4f-113">返回 **以下派生类型的 catalogEntry** 资源 [：featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) [、qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="ebc4f-113">Returns **catalogEntry** resources of the following derived types: [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md), [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="ebc4f-114">属性</span><span class="sxs-lookup"><span data-stu-id="ebc4f-114">Properties</span></span>
|<span data-ttu-id="ebc4f-115">属性</span><span class="sxs-lookup"><span data-stu-id="ebc4f-115">Property</span></span>|<span data-ttu-id="ebc4f-116">类型</span><span class="sxs-lookup"><span data-stu-id="ebc4f-116">Type</span></span>|<span data-ttu-id="ebc4f-117">说明</span><span class="sxs-lookup"><span data-stu-id="ebc4f-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebc4f-118">id</span><span class="sxs-lookup"><span data-stu-id="ebc4f-118">id</span></span>|<span data-ttu-id="ebc4f-119">String</span><span class="sxs-lookup"><span data-stu-id="ebc4f-119">String</span></span>|<span data-ttu-id="ebc4f-120">目录的标识符。</span><span class="sxs-lookup"><span data-stu-id="ebc4f-120">An identifier for the catalog.</span></span> <span data-ttu-id="ebc4f-121">只读。</span><span class="sxs-lookup"><span data-stu-id="ebc4f-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebc4f-122">关系</span><span class="sxs-lookup"><span data-stu-id="ebc4f-122">Relationships</span></span>
|<span data-ttu-id="ebc4f-123">关系</span><span class="sxs-lookup"><span data-stu-id="ebc4f-123">Relationship</span></span>|<span data-ttu-id="ebc4f-124">类型</span><span class="sxs-lookup"><span data-stu-id="ebc4f-124">Type</span></span>|<span data-ttu-id="ebc4f-125">说明</span><span class="sxs-lookup"><span data-stu-id="ebc4f-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebc4f-126">条目</span><span class="sxs-lookup"><span data-stu-id="ebc4f-126">entries</span></span>|<span data-ttu-id="ebc4f-127">[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ebc4f-127">[microsoft.graph.windowsUpdates.catalogEntry](../resources/windowsupdates-catalogentry.md) collection</span></span>|<span data-ttu-id="ebc4f-128">列出可以批准部署的内容。</span><span class="sxs-lookup"><span data-stu-id="ebc4f-128">Lists the content that you can approve for deployment.</span></span> <span data-ttu-id="ebc4f-129">只读。</span><span class="sxs-lookup"><span data-stu-id="ebc4f-129">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebc4f-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebc4f-130">JSON representation</span></span>
<span data-ttu-id="ebc4f-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebc4f-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.catalog",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalog",
  "id": "String (identifier)"
}
```

