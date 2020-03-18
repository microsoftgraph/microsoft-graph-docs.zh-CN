---
title: sideLoadingKey 资源类型
description: 对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f1a5f0dbc305e7a9cd71cfb8a90046edf1e2cfb5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777936"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="2d9ce-103">sideLoadingKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d9ce-103">sideLoadingKey resource type</span></span>

> <span data-ttu-id="2d9ce-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d9ce-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d9ce-106">对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-106">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="2d9ce-107">方法</span><span class="sxs-lookup"><span data-stu-id="2d9ce-107">Methods</span></span>
|<span data-ttu-id="2d9ce-108">方法</span><span class="sxs-lookup"><span data-stu-id="2d9ce-108">Method</span></span>|<span data-ttu-id="2d9ce-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2d9ce-109">Return Type</span></span>|<span data-ttu-id="2d9ce-110">说明</span><span class="sxs-lookup"><span data-stu-id="2d9ce-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2d9ce-111">列出 sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="2d9ce-111">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="2d9ce-112">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)集合</span><span class="sxs-lookup"><span data-stu-id="2d9ce-112">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="2d9ce-113">列出[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-113">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="2d9ce-114">获取 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="2d9ce-114">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="2d9ce-115">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="2d9ce-115">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="2d9ce-116">读取[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-116">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="2d9ce-117">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="2d9ce-117">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="2d9ce-118">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="2d9ce-118">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="2d9ce-119">创建新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-119">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="2d9ce-120">删除 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="2d9ce-120">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="2d9ce-121">None</span><span class="sxs-lookup"><span data-stu-id="2d9ce-121">None</span></span>|<span data-ttu-id="2d9ce-122">删除[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-122">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="2d9ce-123">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="2d9ce-123">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="2d9ce-124">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="2d9ce-124">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="2d9ce-125">更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-125">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d9ce-126">属性</span><span class="sxs-lookup"><span data-stu-id="2d9ce-126">Properties</span></span>
|<span data-ttu-id="2d9ce-127">属性</span><span class="sxs-lookup"><span data-stu-id="2d9ce-127">Property</span></span>|<span data-ttu-id="2d9ce-128">类型</span><span class="sxs-lookup"><span data-stu-id="2d9ce-128">Type</span></span>|<span data-ttu-id="2d9ce-129">说明</span><span class="sxs-lookup"><span data-stu-id="2d9ce-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d9ce-130">id</span><span class="sxs-lookup"><span data-stu-id="2d9ce-130">id</span></span>|<span data-ttu-id="2d9ce-131">字符串</span><span class="sxs-lookup"><span data-stu-id="2d9ce-131">String</span></span>|<span data-ttu-id="2d9ce-132">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-132">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="2d9ce-133">value</span><span class="sxs-lookup"><span data-stu-id="2d9ce-133">value</span></span>|<span data-ttu-id="2d9ce-134">String</span><span class="sxs-lookup"><span data-stu-id="2d9ce-134">String</span></span>|<span data-ttu-id="2d9ce-135">侧加载密钥值，它是一个5x5 值，由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-135">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="2d9ce-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2d9ce-136">displayName</span></span>|<span data-ttu-id="2d9ce-137">字符串</span><span class="sxs-lookup"><span data-stu-id="2d9ce-137">String</span></span>|<span data-ttu-id="2d9ce-138">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-138">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="2d9ce-139">说明</span><span class="sxs-lookup"><span data-stu-id="2d9ce-139">description</span></span>|<span data-ttu-id="2d9ce-140">String</span><span class="sxs-lookup"><span data-stu-id="2d9ce-140">String</span></span>|<span data-ttu-id="2d9ce-141">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-141">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="2d9ce-142">totalActivation</span><span class="sxs-lookup"><span data-stu-id="2d9ce-142">totalActivation</span></span>|<span data-ttu-id="2d9ce-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2d9ce-143">Int32</span></span>|<span data-ttu-id="2d9ce-144">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-144">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="2d9ce-145">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d9ce-145">lastUpdatedDateTime</span></span>|<span data-ttu-id="2d9ce-146">String</span><span class="sxs-lookup"><span data-stu-id="2d9ce-146">String</span></span>|<span data-ttu-id="2d9ce-147">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-147">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d9ce-148">关系</span><span class="sxs-lookup"><span data-stu-id="2d9ce-148">Relationships</span></span>
<span data-ttu-id="2d9ce-149">无</span><span class="sxs-lookup"><span data-stu-id="2d9ce-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d9ce-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d9ce-150">JSON Representation</span></span>
<span data-ttu-id="2d9ce-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d9ce-151">Here is a JSON representation of the resource.</span></span>
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



