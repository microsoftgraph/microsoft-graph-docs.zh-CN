---
title: qualityUpdateCatalogEntry 资源类型
description: 可以批准Windows 10质量更新的元数据。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: f455919bfc3d5f0e6c4e2aa5ef6a6b630b66bc52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067853"
---
# <a name="qualityupdatecatalogentry-resource-type"></a><span data-ttu-id="80b51-103">qualityUpdateCatalogEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="80b51-103">qualityUpdateCatalogEntry resource type</span></span>

<span data-ttu-id="80b51-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="80b51-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80b51-105">可以批准Windows 10质量更新的元数据。</span><span class="sxs-lookup"><span data-stu-id="80b51-105">Metadata for a Windows 10 quality update that you can be approve for deployment.</span></span>

<span data-ttu-id="80b51-106">Windows 10质量更新每月发布一次或多次。</span><span class="sxs-lookup"><span data-stu-id="80b51-106">Windows 10 quality updates are released one or more times per month.</span></span> <span data-ttu-id="80b51-107">这些更新包含安全和质量修补程序，并且通常在每个月的第二个星期二发布，尽管它们可能会随时发布。</span><span class="sxs-lookup"><span data-stu-id="80b51-107">These updates contain both security and quality fixes and are typically released on the second Tuesday of every month, though they may be released at any time.</span></span> <span data-ttu-id="80b51-108">这些更新是累积更新，因此更高版本始终包含所有以前的修补程序。</span><span class="sxs-lookup"><span data-stu-id="80b51-108">These updates are cumulative, so later versions always contain all previous fixes.</span></span> <span data-ttu-id="80b51-109">Microsoft 强烈建议在设备可用时立即安装最新质量更新，使设备保持最新状态。</span><span class="sxs-lookup"><span data-stu-id="80b51-109">Microsoft strongly recommends keeping devices current by installing the most recent quality updates as soon as they are available.</span></span> 

<span data-ttu-id="80b51-110">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="80b51-110">Inherits from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>

## <a name="properties"></a><span data-ttu-id="80b51-111">属性</span><span class="sxs-lookup"><span data-stu-id="80b51-111">Properties</span></span>
|<span data-ttu-id="80b51-112">属性</span><span class="sxs-lookup"><span data-stu-id="80b51-112">Property</span></span>|<span data-ttu-id="80b51-113">类型</span><span class="sxs-lookup"><span data-stu-id="80b51-113">Type</span></span>|<span data-ttu-id="80b51-114">说明</span><span class="sxs-lookup"><span data-stu-id="80b51-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80b51-115">deployableUntilDateTime</span><span class="sxs-lookup"><span data-stu-id="80b51-115">deployableUntilDateTime</span></span>|<span data-ttu-id="80b51-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80b51-116">DateTimeOffset</span></span>|<span data-ttu-id="80b51-117">内容不再可用于使用服务部署的日期。</span><span class="sxs-lookup"><span data-stu-id="80b51-117">The date on which the content is no longer available for deployment using the service.</span></span> <span data-ttu-id="80b51-118">只读。</span><span class="sxs-lookup"><span data-stu-id="80b51-118">Read-only.</span></span> <span data-ttu-id="80b51-119">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="80b51-119">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="80b51-120">displayName</span><span class="sxs-lookup"><span data-stu-id="80b51-120">displayName</span></span>|<span data-ttu-id="80b51-121">String</span><span class="sxs-lookup"><span data-stu-id="80b51-121">String</span></span>|<span data-ttu-id="80b51-122">内容的显示名称。</span><span class="sxs-lookup"><span data-stu-id="80b51-122">The display name of the content.</span></span> <span data-ttu-id="80b51-123">只读。</span><span class="sxs-lookup"><span data-stu-id="80b51-123">Read-only.</span></span> <span data-ttu-id="80b51-124">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="80b51-124">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="80b51-125">id</span><span class="sxs-lookup"><span data-stu-id="80b51-125">id</span></span>|<span data-ttu-id="80b51-126">String</span><span class="sxs-lookup"><span data-stu-id="80b51-126">String</span></span>|<span data-ttu-id="80b51-127">目录项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="80b51-127">The unique identifier for the catalog entry.</span></span> <span data-ttu-id="80b51-128">只读。</span><span class="sxs-lookup"><span data-stu-id="80b51-128">Read-only.</span></span> <span data-ttu-id="80b51-129">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="80b51-129">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|
|<span data-ttu-id="80b51-130">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="80b51-130">isExpeditable</span></span>|<span data-ttu-id="80b51-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="80b51-131">Boolean</span></span>|<span data-ttu-id="80b51-132">指示内容是否可以部署为快速质量更新。</span><span class="sxs-lookup"><span data-stu-id="80b51-132">Indicates whether the content can be deployed as an expedited quality update.</span></span> <span data-ttu-id="80b51-133">只读。</span><span class="sxs-lookup"><span data-stu-id="80b51-133">Read-only.</span></span>|
|<span data-ttu-id="80b51-134">qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="80b51-134">qualityUpdateClassification</span></span>|<span data-ttu-id="80b51-135">microsoft.graph.windowsUpdates.qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="80b51-135">microsoft.graph.windowsUpdates.qualityUpdateClassification</span></span>|<span data-ttu-id="80b51-136">质量更新的分类。</span><span class="sxs-lookup"><span data-stu-id="80b51-136">The classification on the quality update.</span></span> <span data-ttu-id="80b51-137">支持 **qualityUpdateClassification 值的子集**。</span><span class="sxs-lookup"><span data-stu-id="80b51-137">Supports a subset of the values for **qualityUpdateClassification**.</span></span> <span data-ttu-id="80b51-138">可取值为：`all`、`security`、`nonSecurity`。</span><span class="sxs-lookup"><span data-stu-id="80b51-138">Possible values are: `all`, `security`, `nonSecurity`.</span></span> <span data-ttu-id="80b51-139">只读。</span><span class="sxs-lookup"><span data-stu-id="80b51-139">Read-only.</span></span>|
|<span data-ttu-id="80b51-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="80b51-140">releaseDateTime</span></span>|<span data-ttu-id="80b51-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80b51-141">DateTimeOffset</span></span>|<span data-ttu-id="80b51-142">内容的发布日期。</span><span class="sxs-lookup"><span data-stu-id="80b51-142">The release date of the content.</span></span> <span data-ttu-id="80b51-143">只读。</span><span class="sxs-lookup"><span data-stu-id="80b51-143">Read-only.</span></span> <span data-ttu-id="80b51-144">继承自 [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md)。</span><span class="sxs-lookup"><span data-stu-id="80b51-144">Inherited from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="80b51-145">关系</span><span class="sxs-lookup"><span data-stu-id="80b51-145">Relationships</span></span>
<span data-ttu-id="80b51-146">无。</span><span class="sxs-lookup"><span data-stu-id="80b51-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80b51-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80b51-147">JSON representation</span></span>
<span data-ttu-id="80b51-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80b51-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "deployableUntilDateTime": "String (timestamp)",
  "isExpeditable": "Boolean",
  "qualityUpdateClassification": "String"
}
```

