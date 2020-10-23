---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 74800d0e4b87dbb30d8cc726b0849b12c2061647
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691370"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="01040-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="01040-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="01040-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01040-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01040-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="01040-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01040-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01040-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01040-107">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="01040-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="01040-108">属性</span><span class="sxs-lookup"><span data-stu-id="01040-108">Properties</span></span>
|<span data-ttu-id="01040-109">属性</span><span class="sxs-lookup"><span data-stu-id="01040-109">Property</span></span>|<span data-ttu-id="01040-110">类型</span><span class="sxs-lookup"><span data-stu-id="01040-110">Type</span></span>|<span data-ttu-id="01040-111">说明</span><span class="sxs-lookup"><span data-stu-id="01040-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01040-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="01040-112">androidCount</span></span>|<span data-ttu-id="01040-113">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-113">Int32</span></span>|<span data-ttu-id="01040-114">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="01040-114">Number of android device count.</span></span>|
|<span data-ttu-id="01040-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="01040-115">iosCount</span></span>|<span data-ttu-id="01040-116">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-116">Int32</span></span>|<span data-ttu-id="01040-117">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="01040-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="01040-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="01040-118">macOSCount</span></span>|<span data-ttu-id="01040-119">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-119">Int32</span></span>|<span data-ttu-id="01040-120">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="01040-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="01040-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="01040-121">windowsMobileCount</span></span>|<span data-ttu-id="01040-122">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-122">Int32</span></span>|<span data-ttu-id="01040-123">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="01040-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="01040-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="01040-124">windowsCount</span></span>|<span data-ttu-id="01040-125">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-125">Int32</span></span>|<span data-ttu-id="01040-126">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="01040-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="01040-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="01040-127">unknownCount</span></span>|<span data-ttu-id="01040-128">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-128">Int32</span></span>|<span data-ttu-id="01040-129">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="01040-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="01040-130">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="01040-130">androidDedicatedCount</span></span>|<span data-ttu-id="01040-131">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-131">Int32</span></span>|<span data-ttu-id="01040-132">专用 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="01040-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="01040-133">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="01040-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="01040-134">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-134">Int32</span></span>|<span data-ttu-id="01040-135">设备管理 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="01040-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="01040-136">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="01040-136">androidFullyManagedCount</span></span>|<span data-ttu-id="01040-137">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-137">Int32</span></span>|<span data-ttu-id="01040-138">完全管理的 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="01040-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="01040-139">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="01040-139">androidWorkProfileCount</span></span>|<span data-ttu-id="01040-140">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-140">Int32</span></span>|<span data-ttu-id="01040-141">工作配置文件 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="01040-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="01040-142">androidCorporateWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="01040-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="01040-143">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-143">Int32</span></span>|<span data-ttu-id="01040-144">企业工作配置文件 Android 设备的计数。</span><span class="sxs-lookup"><span data-stu-id="01040-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="01040-145">也称为企业拥有的个人启用 ("解决) 。</span><span class="sxs-lookup"><span data-stu-id="01040-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="01040-146">有效值-1 到2147483647</span><span class="sxs-lookup"><span data-stu-id="01040-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="01040-147">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="01040-147">configMgrDeviceCount</span></span>|<span data-ttu-id="01040-148">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-148">Int32</span></span>|<span data-ttu-id="01040-149">ConfigMgr 托管设备的数量。</span><span class="sxs-lookup"><span data-stu-id="01040-149">Number of ConfigMgr managed devices.</span></span>|
|<span data-ttu-id="01040-150">aospUserlessCount</span><span class="sxs-lookup"><span data-stu-id="01040-150">aospUserlessCount</span></span>|<span data-ttu-id="01040-151">Int32</span><span class="sxs-lookup"><span data-stu-id="01040-151">Int32</span></span>|<span data-ttu-id="01040-152">AOSP 专用 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="01040-152">Number of AOSP dedicated Android devices.</span></span> <span data-ttu-id="01040-153">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="01040-153">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="01040-154">关系</span><span class="sxs-lookup"><span data-stu-id="01040-154">Relationships</span></span>
<span data-ttu-id="01040-155">无</span><span class="sxs-lookup"><span data-stu-id="01040-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01040-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01040-156">JSON Representation</span></span>
<span data-ttu-id="01040-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01040-157">Here is a JSON representation of the resource.</span></span>
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
  "androidCorporateWorkProfileCount": 1024,
  "configMgrDeviceCount": 1024,
  "aospUserlessCount": 1024
}
```





