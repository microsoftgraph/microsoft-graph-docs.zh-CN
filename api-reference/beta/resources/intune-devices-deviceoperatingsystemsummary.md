---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b1a49496357a3688bd9f484d8759fdd0c2140eb
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122628"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="63f3c-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="63f3c-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="63f3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63f3c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63f3c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="63f3c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63f3c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="63f3c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63f3c-107">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="63f3c-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="63f3c-108">属性</span><span class="sxs-lookup"><span data-stu-id="63f3c-108">Properties</span></span>
|<span data-ttu-id="63f3c-109">属性</span><span class="sxs-lookup"><span data-stu-id="63f3c-109">Property</span></span>|<span data-ttu-id="63f3c-110">类型</span><span class="sxs-lookup"><span data-stu-id="63f3c-110">Type</span></span>|<span data-ttu-id="63f3c-111">说明</span><span class="sxs-lookup"><span data-stu-id="63f3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63f3c-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-112">androidCount</span></span>|<span data-ttu-id="63f3c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-113">Int32</span></span>|<span data-ttu-id="63f3c-114">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="63f3c-114">Number of android device count.</span></span>|
|<span data-ttu-id="63f3c-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-115">iosCount</span></span>|<span data-ttu-id="63f3c-116">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-116">Int32</span></span>|<span data-ttu-id="63f3c-117">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="63f3c-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="63f3c-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-118">macOSCount</span></span>|<span data-ttu-id="63f3c-119">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-119">Int32</span></span>|<span data-ttu-id="63f3c-120">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="63f3c-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="63f3c-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-121">windowsMobileCount</span></span>|<span data-ttu-id="63f3c-122">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-122">Int32</span></span>|<span data-ttu-id="63f3c-123">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="63f3c-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="63f3c-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-124">windowsCount</span></span>|<span data-ttu-id="63f3c-125">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-125">Int32</span></span>|<span data-ttu-id="63f3c-126">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="63f3c-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="63f3c-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-127">unknownCount</span></span>|<span data-ttu-id="63f3c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-128">Int32</span></span>|<span data-ttu-id="63f3c-129">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="63f3c-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="63f3c-130">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-130">androidDedicatedCount</span></span>|<span data-ttu-id="63f3c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-131">Int32</span></span>|<span data-ttu-id="63f3c-132">专用 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="63f3c-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="63f3c-133">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="63f3c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-134">Int32</span></span>|<span data-ttu-id="63f3c-135">设备管理 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="63f3c-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="63f3c-136">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-136">androidFullyManagedCount</span></span>|<span data-ttu-id="63f3c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-137">Int32</span></span>|<span data-ttu-id="63f3c-138">完全管理的 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="63f3c-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="63f3c-139">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-139">androidWorkProfileCount</span></span>|<span data-ttu-id="63f3c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-140">Int32</span></span>|<span data-ttu-id="63f3c-141">工作配置文件 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="63f3c-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="63f3c-142">androidCorporateWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-142">androidCorporateWorkProfileCount</span></span>|<span data-ttu-id="63f3c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-143">Int32</span></span>|<span data-ttu-id="63f3c-144">企业工作配置文件 Android 设备的计数。</span><span class="sxs-lookup"><span data-stu-id="63f3c-144">The count of Corporate work profile Android devices.</span></span> <span data-ttu-id="63f3c-145">也称为企业拥有的个人启用 ("解决) 。</span><span class="sxs-lookup"><span data-stu-id="63f3c-145">Also known as Corporate Owned Personally Enabled (COPE).</span></span> <span data-ttu-id="63f3c-146">有效值-1 到2147483647</span><span class="sxs-lookup"><span data-stu-id="63f3c-146">Valid values -1 to 2147483647</span></span>|
|<span data-ttu-id="63f3c-147">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="63f3c-147">configMgrDeviceCount</span></span>|<span data-ttu-id="63f3c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="63f3c-148">Int32</span></span>|<span data-ttu-id="63f3c-149">ConfigMgr 托管设备的数量。</span><span class="sxs-lookup"><span data-stu-id="63f3c-149">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63f3c-150">关系</span><span class="sxs-lookup"><span data-stu-id="63f3c-150">Relationships</span></span>
<span data-ttu-id="63f3c-151">无</span><span class="sxs-lookup"><span data-stu-id="63f3c-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63f3c-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63f3c-152">JSON Representation</span></span>
<span data-ttu-id="63f3c-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63f3c-153">Here is a JSON representation of the resource.</span></span>
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
  "configMgrDeviceCount": 1024
}
```



