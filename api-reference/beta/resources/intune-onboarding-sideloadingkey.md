---
title: sideLoadingKey 资源类型
description: 对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 93a0e91332403d3bc333db90a74923e57a55d107
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704726"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="69916-103">sideLoadingKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="69916-103">sideLoadingKey resource type</span></span>

<span data-ttu-id="69916-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69916-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69916-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69916-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69916-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69916-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69916-107">对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。</span><span class="sxs-lookup"><span data-stu-id="69916-107">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="69916-108">Methods</span><span class="sxs-lookup"><span data-stu-id="69916-108">Methods</span></span>
|<span data-ttu-id="69916-109">方法</span><span class="sxs-lookup"><span data-stu-id="69916-109">Method</span></span>|<span data-ttu-id="69916-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="69916-110">Return Type</span></span>|<span data-ttu-id="69916-111">说明</span><span class="sxs-lookup"><span data-stu-id="69916-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69916-112">列出 sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="69916-112">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="69916-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="69916-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="69916-114">列出 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69916-114">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="69916-115">获取 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="69916-115">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="69916-116">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="69916-116">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="69916-117">读取 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69916-117">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="69916-118">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="69916-118">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="69916-119">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="69916-119">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="69916-120">创建新的 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69916-120">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="69916-121">删除 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="69916-121">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="69916-122">无</span><span class="sxs-lookup"><span data-stu-id="69916-122">None</span></span>|<span data-ttu-id="69916-123">删除 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。</span><span class="sxs-lookup"><span data-stu-id="69916-123">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="69916-124">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="69916-124">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="69916-125">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="69916-125">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="69916-126">更新 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69916-126">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="69916-127">属性</span><span class="sxs-lookup"><span data-stu-id="69916-127">Properties</span></span>
|<span data-ttu-id="69916-128">属性</span><span class="sxs-lookup"><span data-stu-id="69916-128">Property</span></span>|<span data-ttu-id="69916-129">类型</span><span class="sxs-lookup"><span data-stu-id="69916-129">Type</span></span>|<span data-ttu-id="69916-130">说明</span><span class="sxs-lookup"><span data-stu-id="69916-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69916-131">id</span><span class="sxs-lookup"><span data-stu-id="69916-131">id</span></span>|<span data-ttu-id="69916-132">String</span><span class="sxs-lookup"><span data-stu-id="69916-132">String</span></span>|<span data-ttu-id="69916-133">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="69916-133">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="69916-134">value</span><span class="sxs-lookup"><span data-stu-id="69916-134">value</span></span>|<span data-ttu-id="69916-135">String</span><span class="sxs-lookup"><span data-stu-id="69916-135">String</span></span>|<span data-ttu-id="69916-136">侧加载密钥值，它是一个5x5 值，由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="69916-136">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="69916-137">displayName</span><span class="sxs-lookup"><span data-stu-id="69916-137">displayName</span></span>|<span data-ttu-id="69916-138">String</span><span class="sxs-lookup"><span data-stu-id="69916-138">String</span></span>|<span data-ttu-id="69916-139">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="69916-139">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="69916-140">说明</span><span class="sxs-lookup"><span data-stu-id="69916-140">description</span></span>|<span data-ttu-id="69916-141">String</span><span class="sxs-lookup"><span data-stu-id="69916-141">String</span></span>|<span data-ttu-id="69916-142">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="69916-142">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="69916-143">totalActivation</span><span class="sxs-lookup"><span data-stu-id="69916-143">totalActivation</span></span>|<span data-ttu-id="69916-144">Int32</span><span class="sxs-lookup"><span data-stu-id="69916-144">Int32</span></span>|<span data-ttu-id="69916-145">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="69916-145">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="69916-146">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="69916-146">lastUpdatedDateTime</span></span>|<span data-ttu-id="69916-147">String</span><span class="sxs-lookup"><span data-stu-id="69916-147">String</span></span>|<span data-ttu-id="69916-148">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="69916-148">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69916-149">关系</span><span class="sxs-lookup"><span data-stu-id="69916-149">Relationships</span></span>
<span data-ttu-id="69916-150">无</span><span class="sxs-lookup"><span data-stu-id="69916-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69916-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69916-151">JSON Representation</span></span>
<span data-ttu-id="69916-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69916-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```





