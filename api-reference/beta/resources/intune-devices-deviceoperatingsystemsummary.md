---
title: deviceOperatingSystemSummary 资源类型
description: 设备操作系统摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ccb18fa2f8ec1545530dca13a7ed9d59be5a7504
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539097"
---
# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="ef1e6-103">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef1e6-103">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="ef1e6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef1e6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef1e6-106">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-106">Device operating system summary.</span></span>

## <a name="properties"></a><span data-ttu-id="ef1e6-107">属性</span><span class="sxs-lookup"><span data-stu-id="ef1e6-107">Properties</span></span>
|<span data-ttu-id="ef1e6-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef1e6-108">Property</span></span>|<span data-ttu-id="ef1e6-109">类型</span><span class="sxs-lookup"><span data-stu-id="ef1e6-109">Type</span></span>|<span data-ttu-id="ef1e6-110">说明</span><span class="sxs-lookup"><span data-stu-id="ef1e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef1e6-111">androidCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-111">androidCount</span></span>|<span data-ttu-id="ef1e6-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-112">Int32</span></span>|<span data-ttu-id="ef1e6-113">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-113">Number of android device count.</span></span>|
|<span data-ttu-id="ef1e6-114">iosCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-114">iosCount</span></span>|<span data-ttu-id="ef1e6-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-115">Int32</span></span>|<span data-ttu-id="ef1e6-116">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-116">Number of iOS device count.</span></span>|
|<span data-ttu-id="ef1e6-117">macOSCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-117">macOSCount</span></span>|<span data-ttu-id="ef1e6-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-118">Int32</span></span>|<span data-ttu-id="ef1e6-119">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-119">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="ef1e6-120">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-120">windowsMobileCount</span></span>|<span data-ttu-id="ef1e6-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-121">Int32</span></span>|<span data-ttu-id="ef1e6-122">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-122">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="ef1e6-123">windowsCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-123">windowsCount</span></span>|<span data-ttu-id="ef1e6-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-124">Int32</span></span>|<span data-ttu-id="ef1e6-125">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-125">Number of Windows device count.</span></span>|
|<span data-ttu-id="ef1e6-126">unknownCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-126">unknownCount</span></span>|<span data-ttu-id="ef1e6-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-127">Int32</span></span>|<span data-ttu-id="ef1e6-128">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-128">Number of unknown device count.</span></span>|
|<span data-ttu-id="ef1e6-129">androidDedicatedCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-129">androidDedicatedCount</span></span>|<span data-ttu-id="ef1e6-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-130">Int32</span></span>|<span data-ttu-id="ef1e6-131">专用 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-131">Number of dedicated Android devices.</span></span>|
|<span data-ttu-id="ef1e6-132">androidDeviceAdminCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-132">androidDeviceAdminCount</span></span>|<span data-ttu-id="ef1e6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-133">Int32</span></span>|<span data-ttu-id="ef1e6-134">设备管理 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-134">Number of device admin Android devices.</span></span>|
|<span data-ttu-id="ef1e6-135">androidFullyManagedCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-135">androidFullyManagedCount</span></span>|<span data-ttu-id="ef1e6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-136">Int32</span></span>|<span data-ttu-id="ef1e6-137">完全管理的 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-137">Number of fully managed Android devices.</span></span>|
|<span data-ttu-id="ef1e6-138">androidWorkProfileCount</span><span class="sxs-lookup"><span data-stu-id="ef1e6-138">androidWorkProfileCount</span></span>|<span data-ttu-id="ef1e6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1e6-139">Int32</span></span>|<span data-ttu-id="ef1e6-140">工作配置文件 Android 设备的数量。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-140">Number of work profile Android devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef1e6-141">关系</span><span class="sxs-lookup"><span data-stu-id="ef1e6-141">Relationships</span></span>
<span data-ttu-id="ef1e6-142">无</span><span class="sxs-lookup"><span data-stu-id="ef1e6-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef1e6-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef1e6-143">JSON Representation</span></span>
<span data-ttu-id="ef1e6-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef1e6-144">Here is a JSON representation of the resource.</span></span>
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
  "androidWorkProfileCount": 1024
}
```



