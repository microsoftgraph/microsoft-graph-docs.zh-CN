---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01965c1dfaeb04d05d2dc6293fc449c0bbc878fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157636"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="2a8f7-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a8f7-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="2a8f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a8f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a8f7-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a8f7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a8f7-107">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="2a8f7-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a8f7-108">Properties</span></span>
|<span data-ttu-id="2a8f7-109">属性</span><span class="sxs-lookup"><span data-stu-id="2a8f7-109">Property</span></span>|<span data-ttu-id="2a8f7-110">类型</span><span class="sxs-lookup"><span data-stu-id="2a8f7-110">Type</span></span>|<span data-ttu-id="2a8f7-111">说明</span><span class="sxs-lookup"><span data-stu-id="2a8f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a8f7-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-112">androidCount</span></span>|<span data-ttu-id="2a8f7-113">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-113">Int32</span></span>|<span data-ttu-id="2a8f7-114">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-114">Number of android device count.</span></span>|
|<span data-ttu-id="2a8f7-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-115">iosCount</span></span>|<span data-ttu-id="2a8f7-116">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-116">Int32</span></span>|<span data-ttu-id="2a8f7-117">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="2a8f7-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-118">macOSCount</span></span>|<span data-ttu-id="2a8f7-119">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-119">Int32</span></span>|<span data-ttu-id="2a8f7-120">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="2a8f7-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-121">windowsMobileCount</span></span>|<span data-ttu-id="2a8f7-122">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-122">Int32</span></span>|<span data-ttu-id="2a8f7-123">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="2a8f7-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-124">windowsCount</span></span>|<span data-ttu-id="2a8f7-125">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-125">Int32</span></span>|<span data-ttu-id="2a8f7-126">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="2a8f7-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-127">unknownCount</span></span>|<span data-ttu-id="2a8f7-128">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-128">Int32</span></span>|<span data-ttu-id="2a8f7-129">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="2a8f7-130">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-130">androidDedicatedCount</span></span>|<span data-ttu-id="2a8f7-131">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-131">Int32</span></span>|<span data-ttu-id="2a8f7-132">专用 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="2a8f7-133">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="2a8f7-134">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-134">Int32</span></span>|<span data-ttu-id="2a8f7-135">设备管理员 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="2a8f7-136">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-136">androidFullyManagedCount</span></span>|<span data-ttu-id="2a8f7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-137">Int32</span></span>|<span data-ttu-id="2a8f7-138">完全托管的 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="2a8f7-139">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-139">androidWorkProfileCount</span></span>|<span data-ttu-id="2a8f7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-140">Int32</span></span>|<span data-ttu-id="2a8f7-141">工作配置文件 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="2a8f7-142">androidCorporateWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="2a8f7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-143">Int32</span></span>|<span data-ttu-id="2a8f7-144">企业工作配置文件 Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="2a8f7-145">也称为公司拥有的个人拥有 (的) 。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="2a8f7-146">有效值 -1 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="2a8f7-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="2a8f7-147">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-147">configMgrDeviceCount</span></span>|<span data-ttu-id="2a8f7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-148">Int32</span></span>|<span data-ttu-id="2a8f7-149">ConfigMgr 托管设备的数量。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-149">Number of ConfigMgr managed devices.</span></span>|
|<span data-ttu-id="2a8f7-150">aospUserlessCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-150">aospUserlessCount</span></span>|<span data-ttu-id="2a8f7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-151">Int32</span></span>|<span data-ttu-id="2a8f7-152">无用户 AOSP Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-152">Number of AOSP userless Android devices.</span></span> <span data-ttu-id="2a8f7-153">有效值为 0 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="2a8f7-153">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="2a8f7-154">aospUserAssociatedCount</span><span class="sxs-lookup"><span data-stu-id="2a8f7-154">aospUserAssociatedCount</span></span>|<span data-ttu-id="2a8f7-155">Int32</span><span class="sxs-lookup"><span data-stu-id="2a8f7-155">Int32</span></span>|<span data-ttu-id="2a8f7-156">AOSP 用户关联的 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-156">Number of AOSP user-associated Android devices.</span></span> <span data-ttu-id="2a8f7-157">有效值为 0 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="2a8f7-157">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a8f7-158">关系</span><span class="sxs-lookup"><span data-stu-id="2a8f7-158">Relationships</span></span>
<span data-ttu-id="2a8f7-159">无</span><span class="sxs-lookup"><span data-stu-id="2a8f7-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a8f7-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a8f7-160">JSON Representation</span></span>
<span data-ttu-id="2a8f7-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a8f7-161">Here is a JSON representation of the resource.</span></span>
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
  "aospUserlessCount": 1024,
  "aospUserAssociatedCount": 1024
}
```




