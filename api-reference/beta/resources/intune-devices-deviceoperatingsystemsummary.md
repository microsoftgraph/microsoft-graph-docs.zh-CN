---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 59d49f6862f8ab8df1baad1db5458131067514b4
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162489"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="ca746-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca746-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="ca746-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca746-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca746-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca746-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca746-106">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="ca746-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="ca746-107">属性</span><span class="sxs-lookup"><span data-stu-id="ca746-107">Properties</span></span>
|<span data-ttu-id="ca746-108">属性</span><span class="sxs-lookup"><span data-stu-id="ca746-108">Property</span></span>|<span data-ttu-id="ca746-109">类型</span><span class="sxs-lookup"><span data-stu-id="ca746-109">Type</span></span>|<span data-ttu-id="ca746-110">说明</span><span class="sxs-lookup"><span data-stu-id="ca746-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca746-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="ca746-111">androidCount</span></span>|<span data-ttu-id="ca746-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-112">Int32</span></span>|<span data-ttu-id="ca746-113">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ca746-113">Number of android device count.</span></span>|
|<span data-ttu-id="ca746-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="ca746-114">iosCount</span></span>|<span data-ttu-id="ca746-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-115">Int32</span></span>|<span data-ttu-id="ca746-116">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ca746-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="ca746-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="ca746-117">macOSCount</span></span>|<span data-ttu-id="ca746-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-118">Int32</span></span>|<span data-ttu-id="ca746-119">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ca746-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="ca746-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="ca746-120">windowsMobileCount</span></span>|<span data-ttu-id="ca746-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-121">Int32</span></span>|<span data-ttu-id="ca746-122">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="ca746-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="ca746-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="ca746-123">windowsCount</span></span>|<span data-ttu-id="ca746-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-124">Int32</span></span>|<span data-ttu-id="ca746-125">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ca746-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="ca746-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="ca746-126">unknownCount</span></span>|<span data-ttu-id="ca746-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-127">Int32</span></span>|<span data-ttu-id="ca746-128">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="ca746-128">Number of unknown device count.</span></span>|
|<span data-ttu-id="ca746-129">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="ca746-129">androidDedicatedCount</span></span>|<span data-ttu-id="ca746-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-130">Int32</span></span>|<span data-ttu-id="ca746-131">专用 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="ca746-131">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="ca746-132">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="ca746-132">androidDeviceAdminCount</span></span>|<span data-ttu-id="ca746-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-133">Int32</span></span>|<span data-ttu-id="ca746-134">设备管理 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="ca746-134">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="ca746-135">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="ca746-135">androidFullyManagedCount</span></span>|<span data-ttu-id="ca746-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-136">Int32</span></span>|<span data-ttu-id="ca746-137">完全管理的 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="ca746-137">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="ca746-138">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="ca746-138">androidWorkProfileCount</span></span>|<span data-ttu-id="ca746-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-139">Int32</span></span>|<span data-ttu-id="ca746-140">工作配置文件 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="ca746-140">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="ca746-141">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ca746-141">configMgrDeviceCount</span></span>|<span data-ttu-id="ca746-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ca746-142">Int32</span></span>|<span data-ttu-id="ca746-143">ConfigMgr 托管设备的数量。</span><span class="sxs-lookup"><span data-stu-id="ca746-143">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca746-144">关系</span><span class="sxs-lookup"><span data-stu-id="ca746-144">Relationships</span></span>
<span data-ttu-id="ca746-145">无</span><span class="sxs-lookup"><span data-stu-id="ca746-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca746-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca746-146">JSON Representation</span></span>
<span data-ttu-id="ca746-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca746-147">Here is a JSON representation of the resource.</span></span>
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



