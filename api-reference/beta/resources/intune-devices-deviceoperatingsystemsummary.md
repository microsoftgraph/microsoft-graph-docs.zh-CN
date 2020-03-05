---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0427ebde59a1e6cf2edda768ecceaec642fb38be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525031"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="3e4bc-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e4bc-103">deviceOperatingSystemSummary resource type</span></span>

<span data-ttu-id="3e4bc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3e4bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e4bc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e4bc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e4bc-107">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-107">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="3e4bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="3e4bc-108">Properties</span></span>
|<span data-ttu-id="3e4bc-109">属性</span><span class="sxs-lookup"><span data-stu-id="3e4bc-109">Property</span></span>|<span data-ttu-id="3e4bc-110">类型</span><span class="sxs-lookup"><span data-stu-id="3e4bc-110">Type</span></span>|<span data-ttu-id="3e4bc-111">说明</span><span class="sxs-lookup"><span data-stu-id="3e4bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e4bc-112">androidCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-112">androidCount</span></span>|<span data-ttu-id="3e4bc-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-113">Int32</span></span>|<span data-ttu-id="3e4bc-114">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-114">Number of android device count.</span></span>|
|<span data-ttu-id="3e4bc-115">iosCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-115">iosCount</span></span>|<span data-ttu-id="3e4bc-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-116">Int32</span></span>|<span data-ttu-id="3e4bc-117">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-117">Number of iOS device count.</span></span>|
|<span data-ttu-id="3e4bc-118">macOSCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-118">macOSCount</span></span>|<span data-ttu-id="3e4bc-119">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-119">Int32</span></span>|<span data-ttu-id="3e4bc-120">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-120">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="3e4bc-121">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-121">windowsMobileCount</span></span>|<span data-ttu-id="3e4bc-122">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-122">Int32</span></span>|<span data-ttu-id="3e4bc-123">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-123">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="3e4bc-124">windowsCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-124">windowsCount</span></span>|<span data-ttu-id="3e4bc-125">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-125">Int32</span></span>|<span data-ttu-id="3e4bc-126">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-126">Number of Windows device count.</span></span>|
|<span data-ttu-id="3e4bc-127">unknownCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-127">unknownCount</span></span>|<span data-ttu-id="3e4bc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-128">Int32</span></span>|<span data-ttu-id="3e4bc-129">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-129">Number of unknown device count.</span></span>|
|<span data-ttu-id="3e4bc-130">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-130">androidDedicatedCount</span></span>|<span data-ttu-id="3e4bc-131">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-131">Int32</span></span>|<span data-ttu-id="3e4bc-132">专用 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-132">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="3e4bc-133">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-133">androidDeviceAdminCount</span></span>|<span data-ttu-id="3e4bc-134">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-134">Int32</span></span>|<span data-ttu-id="3e4bc-135">设备管理 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-135">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="3e4bc-136">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-136">androidFullyManagedCount</span></span>|<span data-ttu-id="3e4bc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-137">Int32</span></span>|<span data-ttu-id="3e4bc-138">完全管理的 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-138">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="3e4bc-139">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-139">androidWorkProfileCount</span></span>|<span data-ttu-id="3e4bc-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-140">Int32</span></span>|<span data-ttu-id="3e4bc-141">工作配置文件 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-141">Number of work profile Android devices.</span></span>|
|<span data-ttu-id="3e4bc-142">configMgrDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e4bc-142">configMgrDeviceCount</span></span>|<span data-ttu-id="3e4bc-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4bc-143">Int32</span></span>|<span data-ttu-id="3e4bc-144">ConfigMgr 托管设备的数量。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-144">Number of ConfigMgr managed devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e4bc-145">关系</span><span class="sxs-lookup"><span data-stu-id="3e4bc-145">Relationships</span></span>
<span data-ttu-id="3e4bc-146">无</span><span class="sxs-lookup"><span data-stu-id="3e4bc-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e4bc-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e4bc-147">JSON Representation</span></span>
<span data-ttu-id="3e4bc-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e4bc-148">Here is a JSON representation of the resource.</span></span>
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



