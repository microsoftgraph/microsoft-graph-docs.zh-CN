---
title: softwareUpdateCatalogEntry 资源类型
description: 可以批准部署的软件更新的元数据。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3e6d0017860acbfc1371c1555279566e808da1eb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067870"
---
# <a name="softwareupdatecatalogentry-resource-type"></a><span data-ttu-id="c0518-103">softwareUpdateCatalogEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="c0518-103">softwareUpdateCatalogEntry resource type</span></span>

<span data-ttu-id="c0518-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c0518-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0518-105">可以批准部署的软件更新的元数据。</span><span class="sxs-lookup"><span data-stu-id="c0518-105">Metadata for a software update that you can approve for deployment.</span></span>

<span data-ttu-id="c0518-106">继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="c0518-106">Inherits from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span> <span data-ttu-id="c0518-107">[featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md)和[qualityUpdateCatalogEntry 的基类型](../resources/windowsupdates-qualityupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="c0518-107">Base type for [featureUpdateCatalogEntry](../resources/windowsupdates-featureupdatecatalogentry.md) and [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md).</span></span>

<span data-ttu-id="c0518-108">这是一个抽象类型。</span><span class="sxs-lookup"><span data-stu-id="c0518-108">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="c0518-109">属性</span><span class="sxs-lookup"><span data-stu-id="c0518-109">Properties</span></span>
|<span data-ttu-id="c0518-110">属性</span><span class="sxs-lookup"><span data-stu-id="c0518-110">Property</span></span>|<span data-ttu-id="c0518-111">类型</span><span class="sxs-lookup"><span data-stu-id="c0518-111">Type</span></span>|<span data-ttu-id="c0518-112">说明</span><span class="sxs-lookup"><span data-stu-id="c0518-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0518-113">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="c0518-113">deployableUntilDateTime</span></span>|<span data-ttu-id="c0518-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0518-114">DateTimeOffset</span></span>|<span data-ttu-id="c0518-115">内容不再可用于使用服务部署的日期。</span><span class="sxs-lookup"><span data-stu-id="c0518-115">The date on which the content is no longer available for deployment using the service.</span></span> <span data-ttu-id="c0518-116">只读。</span><span class="sxs-lookup"><span data-stu-id="c0518-116">Read-only.</span></span> <span data-ttu-id="c0518-117">继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="c0518-117">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|
|<span data-ttu-id="c0518-118">displayName</span><span class="sxs-lookup"><span data-stu-id="c0518-118">displayName</span></span>|<span data-ttu-id="c0518-119">String</span><span class="sxs-lookup"><span data-stu-id="c0518-119">String</span></span>|<span data-ttu-id="c0518-120">内容的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c0518-120">The display name of the content.</span></span> <span data-ttu-id="c0518-121">只读。</span><span class="sxs-lookup"><span data-stu-id="c0518-121">Read-only.</span></span> <span data-ttu-id="c0518-122">继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="c0518-122">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|
|<span data-ttu-id="c0518-123">id</span><span class="sxs-lookup"><span data-stu-id="c0518-123">id</span></span>|<span data-ttu-id="c0518-124">String</span><span class="sxs-lookup"><span data-stu-id="c0518-124">String</span></span>|<span data-ttu-id="c0518-125">目录项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c0518-125">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="c0518-126">只读。</span><span class="sxs-lookup"><span data-stu-id="c0518-126">Read-only.</span></span> <span data-ttu-id="c0518-127">继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="c0518-127">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|
|<span data-ttu-id="c0518-128">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="c0518-128">releaseDateTime</span></span>|<span data-ttu-id="c0518-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0518-129">DateTimeOffset</span></span>|<span data-ttu-id="c0518-130">内容的发布日期。</span><span class="sxs-lookup"><span data-stu-id="c0518-130">The release date for the content.</span></span> <span data-ttu-id="c0518-131">只读。</span><span class="sxs-lookup"><span data-stu-id="c0518-131">Read-only.</span></span> <span data-ttu-id="c0518-132">继承自 [catalogEntry](../resources/windowsupdates-catalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="c0518-132">Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0518-133">关系</span><span class="sxs-lookup"><span data-stu-id="c0518-133">Relationships</span></span>
<span data-ttu-id="c0518-134">无。</span><span class="sxs-lookup"><span data-stu-id="c0518-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0518-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c0518-135">JSON representation</span></span>
<span data-ttu-id="c0518-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0518-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.catalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)"
}
```

