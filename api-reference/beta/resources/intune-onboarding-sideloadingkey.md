---
title: sideLoadingKey 资源类型
description: 对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e0d44ceabb8834b71b41a50fe977c952bddeaa01
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029363"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="36a84-103">sideLoadingKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="36a84-103">sideLoadingKey resource type</span></span>

<span data-ttu-id="36a84-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36a84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36a84-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36a84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36a84-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36a84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36a84-107">对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。</span><span class="sxs-lookup"><span data-stu-id="36a84-107">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="36a84-108">方法</span><span class="sxs-lookup"><span data-stu-id="36a84-108">Methods</span></span>
|<span data-ttu-id="36a84-109">方法</span><span class="sxs-lookup"><span data-stu-id="36a84-109">Method</span></span>|<span data-ttu-id="36a84-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="36a84-110">Return Type</span></span>|<span data-ttu-id="36a84-111">说明</span><span class="sxs-lookup"><span data-stu-id="36a84-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="36a84-112">列出 sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="36a84-112">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="36a84-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="36a84-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="36a84-114">列出 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="36a84-114">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="36a84-115">获取 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="36a84-115">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="36a84-116">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="36a84-116">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="36a84-117">读取 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="36a84-117">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="36a84-118">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="36a84-118">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="36a84-119">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="36a84-119">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="36a84-120">创建新的 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="36a84-120">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="36a84-121">删除 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="36a84-121">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="36a84-122">无</span><span class="sxs-lookup"><span data-stu-id="36a84-122">None</span></span>|<span data-ttu-id="36a84-123">删除 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。</span><span class="sxs-lookup"><span data-stu-id="36a84-123">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="36a84-124">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="36a84-124">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="36a84-125">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="36a84-125">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="36a84-126">更新 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="36a84-126">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="36a84-127">属性</span><span class="sxs-lookup"><span data-stu-id="36a84-127">Properties</span></span>
|<span data-ttu-id="36a84-128">属性</span><span class="sxs-lookup"><span data-stu-id="36a84-128">Property</span></span>|<span data-ttu-id="36a84-129">类型</span><span class="sxs-lookup"><span data-stu-id="36a84-129">Type</span></span>|<span data-ttu-id="36a84-130">说明</span><span class="sxs-lookup"><span data-stu-id="36a84-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36a84-131">id</span><span class="sxs-lookup"><span data-stu-id="36a84-131">id</span></span>|<span data-ttu-id="36a84-132">String</span><span class="sxs-lookup"><span data-stu-id="36a84-132">String</span></span>|<span data-ttu-id="36a84-133">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="36a84-133">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="36a84-134">value</span><span class="sxs-lookup"><span data-stu-id="36a84-134">value</span></span>|<span data-ttu-id="36a84-135">String</span><span class="sxs-lookup"><span data-stu-id="36a84-135">String</span></span>|<span data-ttu-id="36a84-136">侧加载密钥值，它是一个5x5 值，由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="36a84-136">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="36a84-137">displayName</span><span class="sxs-lookup"><span data-stu-id="36a84-137">displayName</span></span>|<span data-ttu-id="36a84-138">String</span><span class="sxs-lookup"><span data-stu-id="36a84-138">String</span></span>|<span data-ttu-id="36a84-139">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="36a84-139">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="36a84-140">description</span><span class="sxs-lookup"><span data-stu-id="36a84-140">description</span></span>|<span data-ttu-id="36a84-141">String</span><span class="sxs-lookup"><span data-stu-id="36a84-141">String</span></span>|<span data-ttu-id="36a84-142">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="36a84-142">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="36a84-143">totalActivation</span><span class="sxs-lookup"><span data-stu-id="36a84-143">totalActivation</span></span>|<span data-ttu-id="36a84-144">Int32</span><span class="sxs-lookup"><span data-stu-id="36a84-144">Int32</span></span>|<span data-ttu-id="36a84-145">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="36a84-145">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="36a84-146">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="36a84-146">lastUpdatedDateTime</span></span>|<span data-ttu-id="36a84-147">String</span><span class="sxs-lookup"><span data-stu-id="36a84-147">String</span></span>|<span data-ttu-id="36a84-148">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="36a84-148">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36a84-149">关系</span><span class="sxs-lookup"><span data-stu-id="36a84-149">Relationships</span></span>
<span data-ttu-id="36a84-150">无</span><span class="sxs-lookup"><span data-stu-id="36a84-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36a84-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="36a84-151">JSON Representation</span></span>
<span data-ttu-id="36a84-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36a84-152">Here is a JSON representation of the resource.</span></span>
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






