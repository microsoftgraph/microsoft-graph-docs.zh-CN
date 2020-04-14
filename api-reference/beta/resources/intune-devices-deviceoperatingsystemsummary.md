---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c15adc462742adb734a503f55dc69af48bf0f82
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470738"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="f564d-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="f564d-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="f564d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f564d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f564d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f564d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f564d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f564d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f564d-107">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="f564d-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="f564d-108">属性</span><span class="sxs-lookup"><span data-stu-id="f564d-108">Properties</span></span>
|<span data-ttu-id="f564d-109">属性</span><span class="sxs-lookup"><span data-stu-id="f564d-109">Property</span></span>|<span data-ttu-id="f564d-110">类型</span><span class="sxs-lookup"><span data-stu-id="f564d-110">Type</span></span>|<span data-ttu-id="f564d-111">说明</span><span class="sxs-lookup"><span data-stu-id="f564d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f564d-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="f564d-112">androidCount</span></span>|<span data-ttu-id="f564d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-113">Int32</span></span>|<span data-ttu-id="f564d-114">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="f564d-114">Number of android device count.</span></span>|
|<span data-ttu-id="f564d-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="f564d-115">iosCount</span></span>|<span data-ttu-id="f564d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-116">Int32</span></span>|<span data-ttu-id="f564d-117">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="f564d-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="f564d-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="f564d-118">macOSCount</span></span>|<span data-ttu-id="f564d-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-119">Int32</span></span>|<span data-ttu-id="f564d-120">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="f564d-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="f564d-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="f564d-121">windowsMobileCount</span></span>|<span data-ttu-id="f564d-122">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-122">Int32</span></span>|<span data-ttu-id="f564d-123">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="f564d-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="f564d-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="f564d-124">windowsCount</span></span>|<span data-ttu-id="f564d-125">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-125">Int32</span></span>|<span data-ttu-id="f564d-126">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="f564d-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="f564d-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="f564d-127">unknownCount</span></span>|<span data-ttu-id="f564d-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-128">Int32</span></span>|<span data-ttu-id="f564d-129">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="f564d-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="f564d-130">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="f564d-130">androidDedicatedCount</span></span>|<span data-ttu-id="f564d-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-131">Int32</span></span>|<span data-ttu-id="f564d-132">专用 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="f564d-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="f564d-133">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="f564d-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="f564d-134">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-134">Int32</span></span>|<span data-ttu-id="f564d-135">设备管理 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="f564d-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="f564d-136">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="f564d-136">androidFullyManagedCount</span></span>|<span data-ttu-id="f564d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-137">Int32</span></span>|<span data-ttu-id="f564d-138">完全管理的 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="f564d-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="f564d-139">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="f564d-139">androidWorkProfileCount</span></span>|<span data-ttu-id="f564d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-140">Int32</span></span>|<span data-ttu-id="f564d-141">工作配置文件 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="f564d-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="f564d-142">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f564d-142">configMgrDeviceCount</span></span>|<span data-ttu-id="f564d-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f564d-143">Int32</span></span>|<span data-ttu-id="f564d-144">ConfigMgr 托管设备的数量。</span><span class="sxs-lookup"><span data-stu-id="f564d-144">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f564d-145">关系</span><span class="sxs-lookup"><span data-stu-id="f564d-145">Relationships</span></span>
<span data-ttu-id="f564d-146">无</span><span class="sxs-lookup"><span data-stu-id="f564d-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f564d-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f564d-147">JSON Representation</span></span>
<span data-ttu-id="f564d-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f564d-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024,
  "androidDedicatedCount": 1024,
  "androidDeviceAdminCount": 1024,
  "androidFullyManagedCount": 1024,
  "androidWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024
}
```



