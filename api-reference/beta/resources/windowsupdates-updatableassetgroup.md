---
title: updatableAssetGroup 资源类型
description: 一组可接收更新的 azureADDevice 资源。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a3aca42b69a906f167393cfd284d6756b3c4bb52
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067299"
---
# <a name="updatableassetgroup-resource-type"></a><span data-ttu-id="3615b-103">updatableAssetGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="3615b-103">updatableAssetGroup resource type</span></span>

<span data-ttu-id="3615b-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3615b-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3615b-105">一组可接收更新的 [azureADDevice](../resources/windowsupdates-azureaddevice.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="3615b-105">A group of [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources that can receive updates.</span></span>

<span data-ttu-id="3615b-106">成员为 [azureADDevice 资源](../resources/windowsupdates-azureADDevice.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="3615b-106">Members are of the [azureADDevice](../resources/windowsupdates-azureADDevice.md) resource type.</span></span> <span data-ttu-id="3615b-107">**updatableAssetGroup** 资源不能是另一 **个 updatableAssetGroup 的成员**。</span><span class="sxs-lookup"><span data-stu-id="3615b-107">An **updatableAssetGroup** resource cannot be a member of another **updatableAssetGroup**.</span></span>

<span data-ttu-id="3615b-108">继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)。</span><span class="sxs-lookup"><span data-stu-id="3615b-108">Inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3615b-109">方法</span><span class="sxs-lookup"><span data-stu-id="3615b-109">Methods</span></span>
|<span data-ttu-id="3615b-110">方法</span><span class="sxs-lookup"><span data-stu-id="3615b-110">Method</span></span>|<span data-ttu-id="3615b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3615b-111">Return type</span></span>|<span data-ttu-id="3615b-112">说明</span><span class="sxs-lookup"><span data-stu-id="3615b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3615b-113">列出 updatableAssetGroup 资源</span><span class="sxs-lookup"><span data-stu-id="3615b-113">List updatableAssetGroup resources</span></span>](../api/windowsupdates-updates-list-updatableassets-updatableassetgroup.md)|<span data-ttu-id="3615b-114">[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3615b-114">[microsoft.graph.windowsUpdates.updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) collection</span></span>|<span data-ttu-id="3615b-115">获取 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="3615b-115">Get a list of the [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) objects and their properties.</span></span>|
|[<span data-ttu-id="3615b-116">创建 updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="3615b-116">Create updatableAssetGroup</span></span>](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[<span data-ttu-id="3615b-117">microsoft.graph.windowsUpdates.updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="3615b-117">microsoft.graph.windowsUpdates.updatableAssetGroup</span></span>](../resources/windowsupdates-updatableassetgroup.md)|<span data-ttu-id="3615b-118">创建新的 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3615b-118">Create a new [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="3615b-119">获取 updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="3615b-119">Get updatableAssetGroup</span></span>](../api/windowsupdates-updatableassetgroup-get.md)|[<span data-ttu-id="3615b-120">microsoft.graph.windowsUpdates.updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="3615b-120">microsoft.graph.windowsUpdates.updatableAssetGroup</span></span>](../resources/windowsupdates-updatableassetgroup.md)|<span data-ttu-id="3615b-121">读取 [updatableAssetGroup 对象的属性和](../resources/windowsupdates-updatableassetgroup.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="3615b-121">Read the properties and relationships of an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="3615b-122">删除 updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="3615b-122">Delete updatableAssetGroup</span></span>](../api/windowsupdates-updatableassetgroup-delete.md)|<span data-ttu-id="3615b-123">无</span><span class="sxs-lookup"><span data-stu-id="3615b-123">None</span></span>|<span data-ttu-id="3615b-124">删除 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3615b-124">Deletes an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="3615b-125">添加成员</span><span class="sxs-lookup"><span data-stu-id="3615b-125">Add members</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)|<span data-ttu-id="3615b-126">无</span><span class="sxs-lookup"><span data-stu-id="3615b-126">None</span></span>|<span data-ttu-id="3615b-127">将成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="3615b-127">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="3615b-128">按 ID (添加) </span><span class="sxs-lookup"><span data-stu-id="3615b-128">Add members (by ID)</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)|<span data-ttu-id="3615b-129">无</span><span class="sxs-lookup"><span data-stu-id="3615b-129">None</span></span>|<span data-ttu-id="3615b-130">将成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="3615b-130">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="3615b-131">删除成员</span><span class="sxs-lookup"><span data-stu-id="3615b-131">Remove members</span></span>](../api/windowsupdates-updatableassetgroup-removemembers.md)|<span data-ttu-id="3615b-132">无</span><span class="sxs-lookup"><span data-stu-id="3615b-132">None</span></span>|<span data-ttu-id="3615b-133">从 [updatableAssetGroup 中删除成员](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="3615b-133">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="3615b-134">按 ID (删除) </span><span class="sxs-lookup"><span data-stu-id="3615b-134">Remove members (by ID)</span></span>](../api/windowsupdates-updatableassetgroup-removemembers.md)|<span data-ttu-id="3615b-135">无</span><span class="sxs-lookup"><span data-stu-id="3615b-135">None</span></span>|<span data-ttu-id="3615b-136">从 [updatableAssetGroup 中删除成员](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="3615b-136">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="3615b-137">List members</span><span class="sxs-lookup"><span data-stu-id="3615b-137">List members</span></span>](../api/windowsupdates-updatableassetgroup-list-members.md)|<span data-ttu-id="3615b-138">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3615b-138">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="3615b-139">从 [members 导航属性获取 updatableAsset](../resources/windowsupdates-updatableasset.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="3615b-139">Get the [updatableAsset](../resources/windowsupdates-updatableasset.md) resources from the members navigation property.</span></span>|

## <a name="properties"></a><span data-ttu-id="3615b-140">属性</span><span class="sxs-lookup"><span data-stu-id="3615b-140">Properties</span></span>
|<span data-ttu-id="3615b-141">属性</span><span class="sxs-lookup"><span data-stu-id="3615b-141">Property</span></span>|<span data-ttu-id="3615b-142">类型</span><span class="sxs-lookup"><span data-stu-id="3615b-142">Type</span></span>|<span data-ttu-id="3615b-143">说明</span><span class="sxs-lookup"><span data-stu-id="3615b-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3615b-144">id</span><span class="sxs-lookup"><span data-stu-id="3615b-144">id</span></span>|<span data-ttu-id="3615b-145">String</span><span class="sxs-lookup"><span data-stu-id="3615b-145">String</span></span>|<span data-ttu-id="3615b-146">组的标识符。</span><span class="sxs-lookup"><span data-stu-id="3615b-146">An identifier for the group.</span></span> <span data-ttu-id="3615b-147">键。</span><span class="sxs-lookup"><span data-stu-id="3615b-147">Key.</span></span> <span data-ttu-id="3615b-148">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="3615b-148">Not nullable.</span></span> <span data-ttu-id="3615b-149">只读。</span><span class="sxs-lookup"><span data-stu-id="3615b-149">Read-only.</span></span> <span data-ttu-id="3615b-150">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="3615b-150">Returned by default.</span></span> <span data-ttu-id="3615b-151">继承自 [updatableAsset](../resources/windowsupdates-updatableasset.md)。</span><span class="sxs-lookup"><span data-stu-id="3615b-151">Inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3615b-152">关系</span><span class="sxs-lookup"><span data-stu-id="3615b-152">Relationships</span></span>
|<span data-ttu-id="3615b-153">关系</span><span class="sxs-lookup"><span data-stu-id="3615b-153">Relationship</span></span>|<span data-ttu-id="3615b-154">类型</span><span class="sxs-lookup"><span data-stu-id="3615b-154">Type</span></span>|<span data-ttu-id="3615b-155">说明</span><span class="sxs-lookup"><span data-stu-id="3615b-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3615b-156">成员</span><span class="sxs-lookup"><span data-stu-id="3615b-156">members</span></span>|<span data-ttu-id="3615b-157">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3615b-157">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="3615b-158">组的成员。</span><span class="sxs-lookup"><span data-stu-id="3615b-158">Members of the group.</span></span> <span data-ttu-id="3615b-159">只读。</span><span class="sxs-lookup"><span data-stu-id="3615b-159">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3615b-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3615b-160">JSON representation</span></span>
<span data-ttu-id="3615b-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3615b-161">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetGroup",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetGroup",
  "id": "String (identifier)"
}
```

