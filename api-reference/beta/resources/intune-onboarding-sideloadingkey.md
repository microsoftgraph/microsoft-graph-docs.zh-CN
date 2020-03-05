---
title: sideLoadingKey 资源类型
description: 对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1be5f4db6876ff18d17305fe657c9852c01fd15f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524081"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="d503f-103">sideLoadingKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="d503f-103">sideLoadingKey resource type</span></span>

<span data-ttu-id="d503f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d503f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d503f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d503f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d503f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d503f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d503f-107">对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。</span><span class="sxs-lookup"><span data-stu-id="d503f-107">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="d503f-108">方法</span><span class="sxs-lookup"><span data-stu-id="d503f-108">Methods</span></span>
|<span data-ttu-id="d503f-109">方法</span><span class="sxs-lookup"><span data-stu-id="d503f-109">Method</span></span>|<span data-ttu-id="d503f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d503f-110">Return Type</span></span>|<span data-ttu-id="d503f-111">说明</span><span class="sxs-lookup"><span data-stu-id="d503f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d503f-112">列出 sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="d503f-112">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="d503f-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)集合</span><span class="sxs-lookup"><span data-stu-id="d503f-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="d503f-114">列出[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d503f-114">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="d503f-115">获取 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d503f-115">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="d503f-116">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d503f-116">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="d503f-117">读取[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d503f-117">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="d503f-118">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d503f-118">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="d503f-119">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d503f-119">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="d503f-120">创建新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d503f-120">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="d503f-121">删除 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d503f-121">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="d503f-122">无</span><span class="sxs-lookup"><span data-stu-id="d503f-122">None</span></span>|<span data-ttu-id="d503f-123">删除[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。</span><span class="sxs-lookup"><span data-stu-id="d503f-123">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="d503f-124">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d503f-124">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="d503f-125">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="d503f-125">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="d503f-126">更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d503f-126">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d503f-127">属性</span><span class="sxs-lookup"><span data-stu-id="d503f-127">Properties</span></span>
|<span data-ttu-id="d503f-128">属性</span><span class="sxs-lookup"><span data-stu-id="d503f-128">Property</span></span>|<span data-ttu-id="d503f-129">类型</span><span class="sxs-lookup"><span data-stu-id="d503f-129">Type</span></span>|<span data-ttu-id="d503f-130">说明</span><span class="sxs-lookup"><span data-stu-id="d503f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d503f-131">id</span><span class="sxs-lookup"><span data-stu-id="d503f-131">id</span></span>|<span data-ttu-id="d503f-132">字符串</span><span class="sxs-lookup"><span data-stu-id="d503f-132">String</span></span>|<span data-ttu-id="d503f-133">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="d503f-133">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="d503f-134">value</span><span class="sxs-lookup"><span data-stu-id="d503f-134">value</span></span>|<span data-ttu-id="d503f-135">String</span><span class="sxs-lookup"><span data-stu-id="d503f-135">String</span></span>|<span data-ttu-id="d503f-136">侧加载密钥值，它是一个5x5 值，由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="d503f-136">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="d503f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d503f-137">displayName</span></span>|<span data-ttu-id="d503f-138">字符串</span><span class="sxs-lookup"><span data-stu-id="d503f-138">String</span></span>|<span data-ttu-id="d503f-139">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="d503f-139">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="d503f-140">说明</span><span class="sxs-lookup"><span data-stu-id="d503f-140">description</span></span>|<span data-ttu-id="d503f-141">String</span><span class="sxs-lookup"><span data-stu-id="d503f-141">String</span></span>|<span data-ttu-id="d503f-142">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="d503f-142">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="d503f-143">totalActivation</span><span class="sxs-lookup"><span data-stu-id="d503f-143">totalActivation</span></span>|<span data-ttu-id="d503f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d503f-144">Int32</span></span>|<span data-ttu-id="d503f-145">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="d503f-145">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="d503f-146">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d503f-146">lastUpdatedDateTime</span></span>|<span data-ttu-id="d503f-147">String</span><span class="sxs-lookup"><span data-stu-id="d503f-147">String</span></span>|<span data-ttu-id="d503f-148">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="d503f-148">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d503f-149">关系</span><span class="sxs-lookup"><span data-stu-id="d503f-149">Relationships</span></span>
<span data-ttu-id="d503f-150">无</span><span class="sxs-lookup"><span data-stu-id="d503f-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d503f-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d503f-151">JSON Representation</span></span>
<span data-ttu-id="d503f-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d503f-152">Here is a JSON representation of the resource.</span></span>
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



