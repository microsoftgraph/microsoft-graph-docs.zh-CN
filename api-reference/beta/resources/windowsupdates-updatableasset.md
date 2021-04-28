---
title: updatableAsset 资源类型
description: 表示可以接收更新的资产。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 4bfdd3663c0868d22b262d398e505e0e8cb82835
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067296"
---
# <a name="updatableasset-resource-type"></a><span data-ttu-id="42958-103">updatableAsset 资源类型</span><span class="sxs-lookup"><span data-stu-id="42958-103">updatableAsset resource type</span></span>

<span data-ttu-id="42958-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="42958-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42958-105">表示可以接收更新的资产。</span><span class="sxs-lookup"><span data-stu-id="42958-105">Represents an asset that can receive updates.</span></span>

<span data-ttu-id="42958-106">所有可更新资源作为以下派生类型之一存在 [：azureADDevice](../resources/windowsupdates-azureaddevice.md) 和 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="42958-106">All updatable assets exist as one of the following derived types: [azureADDevice](../resources/windowsupdates-azureaddevice.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="42958-107">[azureADDevice 和](../resources/windowsupdates-azureaddevice.md) [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)的基本类型。</span><span class="sxs-lookup"><span data-stu-id="42958-107">Base type of [azureADDevice](../resources/windowsupdates-azureaddevice.md) and [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="42958-108">这是一个抽象类型。</span><span class="sxs-lookup"><span data-stu-id="42958-108">This is an abstract type.</span></span>

## <a name="methods"></a><span data-ttu-id="42958-109">方法</span><span class="sxs-lookup"><span data-stu-id="42958-109">Methods</span></span>
|<span data-ttu-id="42958-110">方法</span><span class="sxs-lookup"><span data-stu-id="42958-110">Method</span></span>|<span data-ttu-id="42958-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="42958-111">Return type</span></span>|<span data-ttu-id="42958-112">说明</span><span class="sxs-lookup"><span data-stu-id="42958-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42958-113">列出 updatableAsset 资源</span><span class="sxs-lookup"><span data-stu-id="42958-113">List updatableAsset resources</span></span>](../api/windowsupdates-updates-list-updatableassets.md)|<span data-ttu-id="42958-114">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42958-114">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="42958-115">获取 [updatableAsset 对象](../resources/windowsupdates-updatableasset.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="42958-115">Get a list of the [updatableAsset](../resources/windowsupdates-updatableasset.md) objects and their properties.</span></span>|
|[<span data-ttu-id="42958-116">创建 updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="42958-116">Create updatableAssetGroup</span></span>](../api/windowsupdates-updates-post-updatableassets-updatableassetgroup.md)|[<span data-ttu-id="42958-117">microsoft.graph.windowsUpdates.updatableAssetGroup</span><span class="sxs-lookup"><span data-stu-id="42958-117">microsoft.graph.windowsUpdates.updatableAssetGroup</span></span>](../resources/windowsupdates-updatableassetgroup.md)|<span data-ttu-id="42958-118">创建新的 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="42958-118">Create a new [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) object.</span></span>|
|[<span data-ttu-id="42958-119">获取 updatableAsset</span><span class="sxs-lookup"><span data-stu-id="42958-119">Get updatableAsset</span></span>](../api/windowsupdates-updatableasset-get.md)|[<span data-ttu-id="42958-120">microsoft.graph.windowsUpdates.updatableAsset</span><span class="sxs-lookup"><span data-stu-id="42958-120">microsoft.graph.windowsUpdates.updatableAsset</span></span>](../resources/windowsupdates-updatableasset.md)|<span data-ttu-id="42958-121">读取 [updatableAsset 对象的属性和](../resources/windowsupdates-updatableasset.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="42958-121">Read the properties and relationships of an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>|
|[<span data-ttu-id="42958-122">删除 updatableAsset</span><span class="sxs-lookup"><span data-stu-id="42958-122">Delete updatableAsset</span></span>](../api/windowsupdates-updatableasset-delete.md)|<span data-ttu-id="42958-123">无</span><span class="sxs-lookup"><span data-stu-id="42958-123">None</span></span>|<span data-ttu-id="42958-124">删除 [updatableAsset](../resources/windowsupdates-updatableasset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="42958-124">Delete an [updatableAsset](../resources/windowsupdates-updatableasset.md) object.</span></span>|
|[<span data-ttu-id="42958-125">在管理中注册资产</span><span class="sxs-lookup"><span data-stu-id="42958-125">Enroll asset in management</span></span>](../api/windowsupdates-updatableasset-enrollassets.md)|<span data-ttu-id="42958-126">无</span><span class="sxs-lookup"><span data-stu-id="42958-126">None</span></span>|<span data-ttu-id="42958-127">在[部署服务的更新管理中注册 updatableAssets。](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="42958-127">Enroll [updatableAssets](../resources/windowsupdates-updatableasset.md) in update management by the deployment service.</span></span>|
|[<span data-ttu-id="42958-128">按 ID 管理 (资产) </span><span class="sxs-lookup"><span data-stu-id="42958-128">Enroll asset in management (by ID)</span></span>](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|<span data-ttu-id="42958-129">无</span><span class="sxs-lookup"><span data-stu-id="42958-129">None</span></span>|<span data-ttu-id="42958-130">在部署服务更新管理中注册相同类型的[updatableAssets。](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="42958-130">Enroll [updatableAssets](../resources/windowsupdates-updatableasset.md) of the same type in update management by the deployment service.</span></span>|
|[<span data-ttu-id="42958-131">从管理中注销资产</span><span class="sxs-lookup"><span data-stu-id="42958-131">Unenroll asset from management</span></span>](../api/windowsupdates-updatableasset-unenrollassets.md)|<span data-ttu-id="42958-132">无</span><span class="sxs-lookup"><span data-stu-id="42958-132">None</span></span>|<span data-ttu-id="42958-133">从部署服务的更新管理中注销[updatableAssets。](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="42958-133">Unenroll [updatableAssets](../resources/windowsupdates-updatableasset.md) from update management by the deployment service.</span></span>|
|[<span data-ttu-id="42958-134">注销按 ID 管理 (资产) </span><span class="sxs-lookup"><span data-stu-id="42958-134">Unenroll asset from management (by ID)</span></span>](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|<span data-ttu-id="42958-135">无</span><span class="sxs-lookup"><span data-stu-id="42958-135">None</span></span>|<span data-ttu-id="42958-136">从部署服务更新管理中注销相同类型的[updatableAssets。](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="42958-136">Unenroll [updatableAssets](../resources/windowsupdates-updatableasset.md) of the same type from update management by the deployment service.</span></span>|
|[<span data-ttu-id="42958-137">向组添加成员</span><span class="sxs-lookup"><span data-stu-id="42958-137">Add members to group</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)|<span data-ttu-id="42958-138">无</span><span class="sxs-lookup"><span data-stu-id="42958-138">None</span></span>|<span data-ttu-id="42958-139">将成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="42958-139">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="42958-140">按 ID (将成员添加到) </span><span class="sxs-lookup"><span data-stu-id="42958-140">Add members to group (by ID)</span></span>](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)|<span data-ttu-id="42958-141">无</span><span class="sxs-lookup"><span data-stu-id="42958-141">None</span></span>|<span data-ttu-id="42958-142">将相同类型的成员添加到 [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="42958-142">Add members of the same type to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="42958-143">从组中删除成员</span><span class="sxs-lookup"><span data-stu-id="42958-143">Remove members from group</span></span>](../api/windowsupdates-updatableassetgroup-removemembers.md)|<span data-ttu-id="42958-144">无</span><span class="sxs-lookup"><span data-stu-id="42958-144">None</span></span>|<span data-ttu-id="42958-145">从 [updatableAssetGroup 中删除成员](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="42958-145">Remove members from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|
|[<span data-ttu-id="42958-146">按 ID (从组中删除) </span><span class="sxs-lookup"><span data-stu-id="42958-146">Remove members from group (by ID)</span></span>](../api/windowsupdates-updatableassetgroup-removemembersbyid.md)|<span data-ttu-id="42958-147">无</span><span class="sxs-lookup"><span data-stu-id="42958-147">None</span></span>|<span data-ttu-id="42958-148">从 [updatableAssetGroup 中删除相同类型的成员](../resources/windowsupdates-updatableassetgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="42958-148">Remove members of the same type from an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="42958-149">属性</span><span class="sxs-lookup"><span data-stu-id="42958-149">Properties</span></span>
|<span data-ttu-id="42958-150">属性</span><span class="sxs-lookup"><span data-stu-id="42958-150">Property</span></span>|<span data-ttu-id="42958-151">类型</span><span class="sxs-lookup"><span data-stu-id="42958-151">Type</span></span>|<span data-ttu-id="42958-152">说明</span><span class="sxs-lookup"><span data-stu-id="42958-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42958-153">id</span><span class="sxs-lookup"><span data-stu-id="42958-153">id</span></span>|<span data-ttu-id="42958-154">String</span><span class="sxs-lookup"><span data-stu-id="42958-154">String</span></span>|<span data-ttu-id="42958-155">资产的标识符。</span><span class="sxs-lookup"><span data-stu-id="42958-155">An identifier for the asset.</span></span> <span data-ttu-id="42958-156">键。</span><span class="sxs-lookup"><span data-stu-id="42958-156">Key.</span></span> <span data-ttu-id="42958-157">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="42958-157">Not nullable.</span></span> <span data-ttu-id="42958-158">只读。</span><span class="sxs-lookup"><span data-stu-id="42958-158">Read-only.</span></span> <span data-ttu-id="42958-159">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="42958-159">Returned by default.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42958-160">关系</span><span class="sxs-lookup"><span data-stu-id="42958-160">Relationships</span></span>
<span data-ttu-id="42958-161">无。</span><span class="sxs-lookup"><span data-stu-id="42958-161">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="42958-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42958-162">JSON representation</span></span>
<span data-ttu-id="42958-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42958-163">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
  "id": "String (identifier)"
}
```

