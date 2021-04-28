---
title: 部署资源类型
description: 表示内容部署到一组设备。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: e34bca8fc1776c749e42e97caa1dd0d91fa51433
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067859"
---
# <a name="deployment-resource-type"></a><span data-ttu-id="91191-103">部署资源类型</span><span class="sxs-lookup"><span data-stu-id="91191-103">deployment resource type</span></span>

<span data-ttu-id="91191-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="91191-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91191-105">表示内容部署到一组设备。</span><span class="sxs-lookup"><span data-stu-id="91191-105">Represents the deployment of content to a set of devices.</span></span>

## <a name="methods"></a><span data-ttu-id="91191-106">方法</span><span class="sxs-lookup"><span data-stu-id="91191-106">Methods</span></span>
|<span data-ttu-id="91191-107">方法</span><span class="sxs-lookup"><span data-stu-id="91191-107">Method</span></span>|<span data-ttu-id="91191-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="91191-108">Return type</span></span>|<span data-ttu-id="91191-109">说明</span><span class="sxs-lookup"><span data-stu-id="91191-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91191-110">列出部署</span><span class="sxs-lookup"><span data-stu-id="91191-110">List deployments</span></span>](../api/windowsupdates-updates-list-deployments.md)|<span data-ttu-id="91191-111">[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91191-111">[microsoft.graph.windowsUpdates.deployment](../resources/windowsupdates-deployment.md) collection</span></span>|<span data-ttu-id="91191-112">获取部署对象 [及其](../resources/windowsupdates-deployment.md) 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="91191-112">Get a list of the [deployment](../resources/windowsupdates-deployment.md) objects and their properties.</span></span>|
|[<span data-ttu-id="91191-113">创建部署</span><span class="sxs-lookup"><span data-stu-id="91191-113">Create deployment</span></span>](../api/windowsupdates-updates-post-deployments.md)|[<span data-ttu-id="91191-114">microsoft.graph.windowsUpdates.deployment</span><span class="sxs-lookup"><span data-stu-id="91191-114">microsoft.graph.windowsUpdates.deployment</span></span>](../resources/windowsupdates-deployment.md)|<span data-ttu-id="91191-115">创建新的 [部署](../resources/windowsupdates-deployment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91191-115">Create a new [deployment](../resources/windowsupdates-deployment.md) object.</span></span>|
|[<span data-ttu-id="91191-116">获取部署</span><span class="sxs-lookup"><span data-stu-id="91191-116">Get deployment</span></span>](../api/windowsupdates-deployment-get.md)|[<span data-ttu-id="91191-117">microsoft.graph.windowsUpdates.deployment</span><span class="sxs-lookup"><span data-stu-id="91191-117">microsoft.graph.windowsUpdates.deployment</span></span>](../resources/windowsupdates-deployment.md)|<span data-ttu-id="91191-118">读取部署 [对象的属性和](../resources/windowsupdates-deployment.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="91191-118">Read the properties and relationships of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>|
|[<span data-ttu-id="91191-119">更新部署</span><span class="sxs-lookup"><span data-stu-id="91191-119">Update deployment</span></span>](../api/windowsupdates-deployment-update.md)|[<span data-ttu-id="91191-120">microsoft.graph.windowsUpdates.deployment</span><span class="sxs-lookup"><span data-stu-id="91191-120">microsoft.graph.windowsUpdates.deployment</span></span>](../resources/windowsupdates-deployment.md)|<span data-ttu-id="91191-121">更新 [部署对象的属性](../resources/windowsupdates-deployment.md) 。</span><span class="sxs-lookup"><span data-stu-id="91191-121">Update the properties of a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>|
|[<span data-ttu-id="91191-122">删除部署</span><span class="sxs-lookup"><span data-stu-id="91191-122">Delete deployment</span></span>](../api/windowsupdates-deployment-delete.md)|<span data-ttu-id="91191-123">无</span><span class="sxs-lookup"><span data-stu-id="91191-123">None</span></span>|<span data-ttu-id="91191-124">删除 [部署对象](../resources/windowsupdates-deployment.md) 。</span><span class="sxs-lookup"><span data-stu-id="91191-124">Deletes a [deployment](../resources/windowsupdates-deployment.md) object.</span></span>|
|[<span data-ttu-id="91191-125">列出访问群体成员</span><span class="sxs-lookup"><span data-stu-id="91191-125">List audience members</span></span>](../api/windowsupdates-deploymentaudience-list-members.md)|<span data-ttu-id="91191-126">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91191-126">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="91191-127">列出部署访问群体的成员。</span><span class="sxs-lookup"><span data-stu-id="91191-127">List members of the deployment audience.</span></span>|
|[<span data-ttu-id="91191-128">列出访问群体排除项</span><span class="sxs-lookup"><span data-stu-id="91191-128">List audience exclusions</span></span>](../api/windowsupdates-deploymentaudience-list-exclusions.md)|<span data-ttu-id="91191-129">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) 集合</span><span class="sxs-lookup"><span data-stu-id="91191-129">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="91191-130">列出部署访问群体中的排除项。</span><span class="sxs-lookup"><span data-stu-id="91191-130">List exclusions from the deployment audience.</span></span>|
|[<span data-ttu-id="91191-131">更新访问群体成员和排除项</span><span class="sxs-lookup"><span data-stu-id="91191-131">Update audience members and exclusions</span></span>](../api/windowsupdates-deploymentaudience-updateaudience.md)|<span data-ttu-id="91191-132">无</span><span class="sxs-lookup"><span data-stu-id="91191-132">None</span></span>|<span data-ttu-id="91191-133">添加或删除部署访问群体的成员和排除项。</span><span class="sxs-lookup"><span data-stu-id="91191-133">Add or remove members and exclusions of the deployment audience.</span></span>|

## <a name="properties"></a><span data-ttu-id="91191-134">属性</span><span class="sxs-lookup"><span data-stu-id="91191-134">Properties</span></span>
|<span data-ttu-id="91191-135">属性</span><span class="sxs-lookup"><span data-stu-id="91191-135">Property</span></span>|<span data-ttu-id="91191-136">类型</span><span class="sxs-lookup"><span data-stu-id="91191-136">Type</span></span>|<span data-ttu-id="91191-137">说明</span><span class="sxs-lookup"><span data-stu-id="91191-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91191-138">内容</span><span class="sxs-lookup"><span data-stu-id="91191-138">content</span></span>|[<span data-ttu-id="91191-139">microsoft.graph.windowsUpdates.deployableContent</span><span class="sxs-lookup"><span data-stu-id="91191-139">microsoft.graph.windowsUpdates.deployableContent</span></span>](../resources/windowsupdates-deployablecontent.md)|<span data-ttu-id="91191-140">指定要部署的内容。</span><span class="sxs-lookup"><span data-stu-id="91191-140">Specifies what content to deploy.</span></span> <span data-ttu-id="91191-141">无法更改。</span><span class="sxs-lookup"><span data-stu-id="91191-141">Cannot be changed.</span></span> <span data-ttu-id="91191-142">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="91191-142">Returned by default.</span></span>|
|<span data-ttu-id="91191-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91191-143">createdDateTime</span></span>|<span data-ttu-id="91191-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91191-144">DateTimeOffset</span></span>|<span data-ttu-id="91191-145">创建部署的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="91191-145">The date and time the deployment was created.</span></span> <span data-ttu-id="91191-146">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="91191-146">Returned by default.</span></span> <span data-ttu-id="91191-147">只读。</span><span class="sxs-lookup"><span data-stu-id="91191-147">Read-only.</span></span>|
|<span data-ttu-id="91191-148">id</span><span class="sxs-lookup"><span data-stu-id="91191-148">id</span></span>|<span data-ttu-id="91191-149">String</span><span class="sxs-lookup"><span data-stu-id="91191-149">String</span></span>|<span data-ttu-id="91191-150">部署的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="91191-150">The unique identifier for the deployment.</span></span> <span data-ttu-id="91191-151">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="91191-151">Returned by default.</span></span> <span data-ttu-id="91191-152">键。</span><span class="sxs-lookup"><span data-stu-id="91191-152">Key.</span></span> <span data-ttu-id="91191-153">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="91191-153">Not nullable.</span></span> <span data-ttu-id="91191-154">只读。</span><span class="sxs-lookup"><span data-stu-id="91191-154">Read-only.</span></span>|
|<span data-ttu-id="91191-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91191-155">lastModifiedDateTime</span></span>|<span data-ttu-id="91191-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91191-156">DateTimeOffset</span></span>|<span data-ttu-id="91191-157">上次修改部署的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="91191-157">The date and time the deployment was last modified.</span></span> <span data-ttu-id="91191-158">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="91191-158">Returned by default.</span></span> <span data-ttu-id="91191-159">只读。</span><span class="sxs-lookup"><span data-stu-id="91191-159">Read-only.</span></span>|
|<span data-ttu-id="91191-160">settings</span><span class="sxs-lookup"><span data-stu-id="91191-160">settings</span></span>|[<span data-ttu-id="91191-161">microsoft.graph.windowsUpdates.deploymentSettings</span><span class="sxs-lookup"><span data-stu-id="91191-161">microsoft.graph.windowsUpdates.deploymentSettings</span></span>](../resources/windowsupdates-deploymentsettings.md)|<span data-ttu-id="91191-162">设置管理如何部署内容的特定部署上指定 **的内容**。</span><span class="sxs-lookup"><span data-stu-id="91191-162">Settings specified on the specific deployment governing how to deploy **content**.</span></span> <span data-ttu-id="91191-163">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="91191-163">Returned by default.</span></span>|
|<span data-ttu-id="91191-164">state</span><span class="sxs-lookup"><span data-stu-id="91191-164">state</span></span>|[<span data-ttu-id="91191-165">microsoft.graph.windowsUpdates.deploymentState</span><span class="sxs-lookup"><span data-stu-id="91191-165">microsoft.graph.windowsUpdates.deploymentState</span></span>](../resources/windowsupdates-deploymentstate.md)|<span data-ttu-id="91191-166">部署的执行状态。</span><span class="sxs-lookup"><span data-stu-id="91191-166">Execution status of the deployment.</span></span> <span data-ttu-id="91191-167">默认情况下返回。</span><span class="sxs-lookup"><span data-stu-id="91191-167">Returned by default.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91191-168">关系</span><span class="sxs-lookup"><span data-stu-id="91191-168">Relationships</span></span>
|<span data-ttu-id="91191-169">关系</span><span class="sxs-lookup"><span data-stu-id="91191-169">Relationship</span></span>|<span data-ttu-id="91191-170">类型</span><span class="sxs-lookup"><span data-stu-id="91191-170">Type</span></span>|<span data-ttu-id="91191-171">说明</span><span class="sxs-lookup"><span data-stu-id="91191-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91191-172">audience</span><span class="sxs-lookup"><span data-stu-id="91191-172">audience</span></span>|[<span data-ttu-id="91191-173">microsoft.graph.windowsUpdates.deploymentAudience</span><span class="sxs-lookup"><span data-stu-id="91191-173">microsoft.graph.windowsUpdates.deploymentAudience</span></span>](../resources/windowsupdates-deploymentaudience.md)|<span data-ttu-id="91191-174">指定内容部署到的目标访问群体。</span><span class="sxs-lookup"><span data-stu-id="91191-174">Specifies the audience to which content is deployed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="91191-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91191-175">JSON representation</span></span>
<span data-ttu-id="91191-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91191-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.deployment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deployment",
  "id": "String (identifier)",
  "state": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
  },
  "content": {
    "@odata.type": "microsoft.graph.windowsUpdates.deployableContent"
  },
  "settings": {
    "@odata.type": "microsoft.graph.windowsUpdates.deploymentSettings"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```

