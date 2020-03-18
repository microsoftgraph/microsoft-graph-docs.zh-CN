---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a88a86a420aa10b32f44e44bc25276040fc9d99c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42784145"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="371d8-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="371d8-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="371d8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="371d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="371d8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="371d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="371d8-106">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="371d8-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="371d8-107">属性</span><span class="sxs-lookup"><span data-stu-id="371d8-107">Properties</span></span>
|<span data-ttu-id="371d8-108">属性</span><span class="sxs-lookup"><span data-stu-id="371d8-108">Property</span></span>|<span data-ttu-id="371d8-109">类型</span><span class="sxs-lookup"><span data-stu-id="371d8-109">Type</span></span>|<span data-ttu-id="371d8-110">说明</span><span class="sxs-lookup"><span data-stu-id="371d8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="371d8-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="371d8-111">androidCount</span></span>|<span data-ttu-id="371d8-112">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-112">Int32</span></span>|<span data-ttu-id="371d8-113">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="371d8-113">Number of android device count.</span></span>|
|<span data-ttu-id="371d8-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="371d8-114">iosCount</span></span>|<span data-ttu-id="371d8-115">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-115">Int32</span></span>|<span data-ttu-id="371d8-116">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="371d8-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="371d8-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="371d8-117">macOSCount</span></span>|<span data-ttu-id="371d8-118">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-118">Int32</span></span>|<span data-ttu-id="371d8-119">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="371d8-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="371d8-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="371d8-120">windowsMobileCount</span></span>|<span data-ttu-id="371d8-121">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-121">Int32</span></span>|<span data-ttu-id="371d8-122">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="371d8-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="371d8-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="371d8-123">windowsCount</span></span>|<span data-ttu-id="371d8-124">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-124">Int32</span></span>|<span data-ttu-id="371d8-125">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="371d8-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="371d8-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="371d8-126">unknownCount</span></span>|<span data-ttu-id="371d8-127">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-127">Int32</span></span>|<span data-ttu-id="371d8-128">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="371d8-128">Number of unknown device count.</span></span>|
|<span data-ttu-id="371d8-129">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="371d8-129">androidDedicatedCount</span></span>|<span data-ttu-id="371d8-130">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-130">Int32</span></span>|<span data-ttu-id="371d8-131">专用 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="371d8-131">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="371d8-132">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="371d8-132">androidDeviceAdminCount</span></span>|<span data-ttu-id="371d8-133">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-133">Int32</span></span>|<span data-ttu-id="371d8-134">设备管理 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="371d8-134">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="371d8-135">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="371d8-135">androidFullyManagedCount</span></span>|<span data-ttu-id="371d8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-136">Int32</span></span>|<span data-ttu-id="371d8-137">完全管理的 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="371d8-137">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="371d8-138">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="371d8-138">androidWorkProfileCount</span></span>|<span data-ttu-id="371d8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-139">Int32</span></span>|<span data-ttu-id="371d8-140">工作配置文件 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="371d8-140">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="371d8-141">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="371d8-141">configMgrDeviceCount</span></span>|<span data-ttu-id="371d8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="371d8-142">Int32</span></span>|<span data-ttu-id="371d8-143">ConfigMgr 托管设备的数量。</span><span class="sxs-lookup"><span data-stu-id="371d8-143">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="371d8-144">关系</span><span class="sxs-lookup"><span data-stu-id="371d8-144">Relationships</span></span>
<span data-ttu-id="371d8-145">无</span><span class="sxs-lookup"><span data-stu-id="371d8-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="371d8-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="371d8-146">JSON Representation</span></span>
<span data-ttu-id="371d8-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="371d8-147">Here is a JSON representation of the resource.</span></span>
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



