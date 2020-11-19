---
title: sideLoadingKey 资源类型
description: 对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a37eae80f3628f5fa8952cf8c2cde225e4f5fc0c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266457"
---
# <a name="sideloadingkey-resource-type"></a><span data-ttu-id="cc0fd-103">sideLoadingKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc0fd-103">sideLoadingKey resource type</span></span>

<span data-ttu-id="cc0fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc0fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc0fd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc0fd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc0fd-107">对于租户，Windows 8 和8.1 设备需要 SideLoadingKey 实体为 intall 的业务线应用程序。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-107">SideLoadingKey entity is required for Windows 8 and 8.1 devices to intall Line Of Business Apps for a tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="cc0fd-108">方法</span><span class="sxs-lookup"><span data-stu-id="cc0fd-108">Methods</span></span>
|<span data-ttu-id="cc0fd-109">方法</span><span class="sxs-lookup"><span data-stu-id="cc0fd-109">Method</span></span>|<span data-ttu-id="cc0fd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc0fd-110">Return Type</span></span>|<span data-ttu-id="cc0fd-111">说明</span><span class="sxs-lookup"><span data-stu-id="cc0fd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc0fd-112">列出 sideLoadingKeies</span><span class="sxs-lookup"><span data-stu-id="cc0fd-112">List sideLoadingKeies</span></span>](../api/intune-onboarding-sideloadingkey-list.md)|<span data-ttu-id="cc0fd-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc0fd-113">[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) collection</span></span>|<span data-ttu-id="cc0fd-114">列出 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-114">List properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) objects.</span></span>|
|[<span data-ttu-id="cc0fd-115">获取 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="cc0fd-115">Get sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-get.md)|[<span data-ttu-id="cc0fd-116">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="cc0fd-116">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="cc0fd-117">读取 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-117">Read properties and relationships of the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="cc0fd-118">创建 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="cc0fd-118">Create sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-create.md)|[<span data-ttu-id="cc0fd-119">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="cc0fd-119">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="cc0fd-120">创建新的 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-120">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|
|[<span data-ttu-id="cc0fd-121">删除 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="cc0fd-121">Delete sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-delete.md)|<span data-ttu-id="cc0fd-122">无</span><span class="sxs-lookup"><span data-stu-id="cc0fd-122">None</span></span>|<span data-ttu-id="cc0fd-123">删除 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-123">Deletes a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>|
|[<span data-ttu-id="cc0fd-124">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="cc0fd-124">Update sideLoadingKey</span></span>](../api/intune-onboarding-sideloadingkey-update.md)|[<span data-ttu-id="cc0fd-125">sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="cc0fd-125">sideLoadingKey</span></span>](../resources/intune-onboarding-sideloadingkey.md)|<span data-ttu-id="cc0fd-126">更新 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-126">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc0fd-127">属性</span><span class="sxs-lookup"><span data-stu-id="cc0fd-127">Properties</span></span>
|<span data-ttu-id="cc0fd-128">属性</span><span class="sxs-lookup"><span data-stu-id="cc0fd-128">Property</span></span>|<span data-ttu-id="cc0fd-129">类型</span><span class="sxs-lookup"><span data-stu-id="cc0fd-129">Type</span></span>|<span data-ttu-id="cc0fd-130">说明</span><span class="sxs-lookup"><span data-stu-id="cc0fd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc0fd-131">id</span><span class="sxs-lookup"><span data-stu-id="cc0fd-131">id</span></span>|<span data-ttu-id="cc0fd-132">字符串</span><span class="sxs-lookup"><span data-stu-id="cc0fd-132">String</span></span>|<span data-ttu-id="cc0fd-133">侧加载密钥唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-133">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="cc0fd-134">value</span><span class="sxs-lookup"><span data-stu-id="cc0fd-134">value</span></span>|<span data-ttu-id="cc0fd-135">String</span><span class="sxs-lookup"><span data-stu-id="cc0fd-135">String</span></span>|<span data-ttu-id="cc0fd-136">侧加载密钥值，它是一个5x5 值，由 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-136">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="cc0fd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cc0fd-137">displayName</span></span>|<span data-ttu-id="cc0fd-138">字符串</span><span class="sxs-lookup"><span data-stu-id="cc0fd-138">String</span></span>|<span data-ttu-id="cc0fd-139">向 It 专业管理员显示的侧加载密钥名称。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-139">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="cc0fd-140">description</span><span class="sxs-lookup"><span data-stu-id="cc0fd-140">description</span></span>|<span data-ttu-id="cc0fd-141">字符串</span><span class="sxs-lookup"><span data-stu-id="cc0fd-141">String</span></span>|<span data-ttu-id="cc0fd-142">向 It 专业管理员显示的侧加载密钥说明。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-142">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="cc0fd-143">totalActivation</span><span class="sxs-lookup"><span data-stu-id="cc0fd-143">totalActivation</span></span>|<span data-ttu-id="cc0fd-144">Int32</span><span class="sxs-lookup"><span data-stu-id="cc0fd-144">Int32</span></span>|<span data-ttu-id="cc0fd-145">向 It 专业管理员显示的端加载密钥总激活数。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-145">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="cc0fd-146">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0fd-146">lastUpdatedDateTime</span></span>|<span data-ttu-id="cc0fd-147">字符串</span><span class="sxs-lookup"><span data-stu-id="cc0fd-147">String</span></span>|<span data-ttu-id="cc0fd-148">向 It 专业管理员显示的侧加载密钥上次更新日期。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-148">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc0fd-149">关系</span><span class="sxs-lookup"><span data-stu-id="cc0fd-149">Relationships</span></span>
<span data-ttu-id="cc0fd-150">无</span><span class="sxs-lookup"><span data-stu-id="cc0fd-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc0fd-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc0fd-151">JSON Representation</span></span>
<span data-ttu-id="cc0fd-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc0fd-152">Here is a JSON representation of the resource.</span></span>
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




