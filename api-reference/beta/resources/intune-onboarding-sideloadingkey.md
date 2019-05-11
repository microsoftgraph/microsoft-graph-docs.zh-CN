---
title: sideLoadingKey 资源类型
description: 对于租户, Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c09cdc1bc620c6f6882abeeae29c7e00613254b1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940139"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="013e6-103">sideLoadingKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="013e6-103">sideLoadingKey resource type</span></span>

> <span data-ttu-id="013e6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="013e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="013e6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="013e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="013e6-106">对于租户, Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。</span><span class="sxs-lookup"><span data-stu-id="013e6-106">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="013e6-107">方法</span><span class="sxs-lookup"><span data-stu-id="013e6-107">Methods</span></span>
|<span data-ttu-id="013e6-108">方法</span><span class="sxs-lookup"><span data-stu-id="013e6-108">Method</span></span>|<span data-ttu-id="013e6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="013e6-109">Return Type</span></span>|<span data-ttu-id="013e6-110">说明</span><span class="sxs-lookup"><span data-stu-id="013e6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="013e6-111">列出 sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="013e6-111">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="013e6-112">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)集合</span><span class="sxs-lookup"><span data-stu-id="013e6-112">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="013e6-113">列出[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="013e6-113">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="013e6-114">获取 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="013e6-114">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="013e6-115">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="013e6-115">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="013e6-116">读取[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="013e6-116">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="013e6-117">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="013e6-117">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="013e6-118">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="013e6-118">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="013e6-119">创建新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="013e6-119">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="013e6-120">删除 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="013e6-120">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="013e6-121">无</span><span class="sxs-lookup"><span data-stu-id="013e6-121">None</span></span>|<span data-ttu-id="013e6-122">删除[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。</span><span class="sxs-lookup"><span data-stu-id="013e6-122">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="013e6-123">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="013e6-123">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="013e6-124">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="013e6-124">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="013e6-125">更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="013e6-125">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="013e6-126">属性</span><span class="sxs-lookup"><span data-stu-id="013e6-126">Properties</span></span>
|<span data-ttu-id="013e6-127">属性</span><span class="sxs-lookup"><span data-stu-id="013e6-127">Property</span></span>|<span data-ttu-id="013e6-128">类型</span><span class="sxs-lookup"><span data-stu-id="013e6-128">Type</span></span>|<span data-ttu-id="013e6-129">说明</span><span class="sxs-lookup"><span data-stu-id="013e6-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="013e6-130">id</span><span class="sxs-lookup"><span data-stu-id="013e6-130">id</span></span>|<span data-ttu-id="013e6-131">字符串</span><span class="sxs-lookup"><span data-stu-id="013e6-131">String</span></span>|<span data-ttu-id="013e6-132">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="013e6-132">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="013e6-133">value</span><span class="sxs-lookup"><span data-stu-id="013e6-133">value</span></span>|<span data-ttu-id="013e6-134">String</span><span class="sxs-lookup"><span data-stu-id="013e6-134">String</span></span>|<span data-ttu-id="013e6-135">侧加载密钥值, 它是一个5x5 值, 由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="013e6-135">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="013e6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="013e6-136">displayName</span></span>|<span data-ttu-id="013e6-137">字符串</span><span class="sxs-lookup"><span data-stu-id="013e6-137">String</span></span>|<span data-ttu-id="013e6-138">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="013e6-138">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="013e6-139">说明</span><span class="sxs-lookup"><span data-stu-id="013e6-139">description</span></span>|<span data-ttu-id="013e6-140">String</span><span class="sxs-lookup"><span data-stu-id="013e6-140">String</span></span>|<span data-ttu-id="013e6-141">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="013e6-141">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="013e6-142">totalActivation</span><span class="sxs-lookup"><span data-stu-id="013e6-142">totalActivation</span></span>|<span data-ttu-id="013e6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="013e6-143">Int32</span></span>|<span data-ttu-id="013e6-144">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="013e6-144">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="013e6-145">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="013e6-145">lastUpdatedDateTime</span></span>|<span data-ttu-id="013e6-146">String</span><span class="sxs-lookup"><span data-stu-id="013e6-146">String</span></span>|<span data-ttu-id="013e6-147">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="013e6-147">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="013e6-148">关系</span><span class="sxs-lookup"><span data-stu-id="013e6-148">Relationships</span></span>
<span data-ttu-id="013e6-149">无</span><span class="sxs-lookup"><span data-stu-id="013e6-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="013e6-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="013e6-150">JSON Representation</span></span>
<span data-ttu-id="013e6-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="013e6-151">Here is a JSON representation of the resource.</span></span>
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




