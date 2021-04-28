---
title: deploymentAudience 资源类型
description: 部署可应用到的 updatableAsset 资源集。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 98d295183f69012da6ea9fc5803bc440465854c8
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067312"
---
# <a name="deploymentaudience-resource-type"></a><span data-ttu-id="c02c5-103">deploymentAudience 资源类型</span><span class="sxs-lookup"><span data-stu-id="c02c5-103">deploymentAudience resource type</span></span>

<span data-ttu-id="c02c5-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="c02c5-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c02c5-105">部署[可应用到的 updatableAsset](../resources/windowsupdates-updatableasset.md)[资源集](../resources/windowsupdates-deployment.md)。</span><span class="sxs-lookup"><span data-stu-id="c02c5-105">The set of [updatableAsset](../resources/windowsupdates-updatableasset.md) resources to which a [deployment](../resources/windowsupdates-deployment.md) can apply.</span></span>

<span data-ttu-id="c02c5-106">如果排除项和成员关系中包含同一 **updatableAsset** **资源，** 则部署不适用于它。 </span><span class="sxs-lookup"><span data-stu-id="c02c5-106">If the same **updatableAsset** resource is included in the **exclusions** and **members** relationships, deployment will not apply to it.</span></span>

## <a name="methods"></a><span data-ttu-id="c02c5-107">方法</span><span class="sxs-lookup"><span data-stu-id="c02c5-107">Methods</span></span>
|<span data-ttu-id="c02c5-108">方法</span><span class="sxs-lookup"><span data-stu-id="c02c5-108">Method</span></span>|<span data-ttu-id="c02c5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c02c5-109">Return type</span></span>|<span data-ttu-id="c02c5-110">说明</span><span class="sxs-lookup"><span data-stu-id="c02c5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c02c5-111">列出成员</span><span class="sxs-lookup"><span data-stu-id="c02c5-111">List members</span></span>](../api/windowsupdates-deploymentaudience-list-members.md)|<span data-ttu-id="c02c5-112">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c02c5-112">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="c02c5-113">列出 [deploymentAudience 的成员](../resources/windowsupdates-deploymentaudience.md)。</span><span class="sxs-lookup"><span data-stu-id="c02c5-113">List members of the [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>|
|[<span data-ttu-id="c02c5-114">列表排除项</span><span class="sxs-lookup"><span data-stu-id="c02c5-114">List exclusions</span></span>](../api/windowsupdates-deploymentaudience-list-exclusions.md)|<span data-ttu-id="c02c5-115">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c02c5-115">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="c02c5-116">列出 [deploymentAudience 的排除项](../resources/windowsupdates-deploymentaudience.md)。</span><span class="sxs-lookup"><span data-stu-id="c02c5-116">List exclusions of the [deploymentAudience](../resources/windowsupdates-deploymentaudience.md).</span></span>|
|[<span data-ttu-id="c02c5-117">更新成员和排除项</span><span class="sxs-lookup"><span data-stu-id="c02c5-117">Update members and exclusions</span></span>](../api/windowsupdates-deploymentaudience-updateaudience.md)|<span data-ttu-id="c02c5-118">无</span><span class="sxs-lookup"><span data-stu-id="c02c5-118">None</span></span>|<span data-ttu-id="c02c5-119">添加或删除成员和排除项。</span><span class="sxs-lookup"><span data-stu-id="c02c5-119">Add or remove members and exclusions.</span></span>|
|[<span data-ttu-id="c02c5-120">按 ID 更新 (排除项) </span><span class="sxs-lookup"><span data-stu-id="c02c5-120">Update members and exclusions (by ID)</span></span>](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)|<span data-ttu-id="c02c5-121">无</span><span class="sxs-lookup"><span data-stu-id="c02c5-121">None</span></span>|<span data-ttu-id="c02c5-122">添加或删除相同类型的成员和排除项。</span><span class="sxs-lookup"><span data-stu-id="c02c5-122">Add or remove members and exclusions of the same type.</span></span>|

## <a name="properties"></a><span data-ttu-id="c02c5-123">属性</span><span class="sxs-lookup"><span data-stu-id="c02c5-123">Properties</span></span>
|<span data-ttu-id="c02c5-124">属性</span><span class="sxs-lookup"><span data-stu-id="c02c5-124">Property</span></span>|<span data-ttu-id="c02c5-125">类型</span><span class="sxs-lookup"><span data-stu-id="c02c5-125">Type</span></span>|<span data-ttu-id="c02c5-126">说明</span><span class="sxs-lookup"><span data-stu-id="c02c5-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c02c5-127">id</span><span class="sxs-lookup"><span data-stu-id="c02c5-127">id</span></span>|<span data-ttu-id="c02c5-128">String</span><span class="sxs-lookup"><span data-stu-id="c02c5-128">String</span></span>|<span data-ttu-id="c02c5-129">部署访问群体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c02c5-129">The unique identifier for the deployment audience.</span></span> <span data-ttu-id="c02c5-130">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="c02c5-130">Returned by default.</span></span> <span data-ttu-id="c02c5-131">键。</span><span class="sxs-lookup"><span data-stu-id="c02c5-131">Key.</span></span> <span data-ttu-id="c02c5-132">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="c02c5-132">Not nullable.</span></span> <span data-ttu-id="c02c5-133">只读。</span><span class="sxs-lookup"><span data-stu-id="c02c5-133">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c02c5-134">关系</span><span class="sxs-lookup"><span data-stu-id="c02c5-134">Relationships</span></span>
|<span data-ttu-id="c02c5-135">关系</span><span class="sxs-lookup"><span data-stu-id="c02c5-135">Relationship</span></span>|<span data-ttu-id="c02c5-136">类型</span><span class="sxs-lookup"><span data-stu-id="c02c5-136">Type</span></span>|<span data-ttu-id="c02c5-137">说明</span><span class="sxs-lookup"><span data-stu-id="c02c5-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c02c5-138">排除项</span><span class="sxs-lookup"><span data-stu-id="c02c5-138">exclusions</span></span>|<span data-ttu-id="c02c5-139">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c02c5-139">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="c02c5-140">指定要从访问群体中排除的资产。</span><span class="sxs-lookup"><span data-stu-id="c02c5-140">Specifies the assets to exclude from the audience.</span></span>|
|<span data-ttu-id="c02c5-141">members</span><span class="sxs-lookup"><span data-stu-id="c02c5-141">members</span></span>|<span data-ttu-id="c02c5-142">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c02c5-142">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="c02c5-143">指定要包括在访问群体中的资源。</span><span class="sxs-lookup"><span data-stu-id="c02c5-143">Specifies the assets to include in the audience.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c02c5-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c02c5-144">JSON representation</span></span>
<span data-ttu-id="c02c5-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c02c5-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentAudience",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentAudience",
  "id": "String (identifier)"
}
```

