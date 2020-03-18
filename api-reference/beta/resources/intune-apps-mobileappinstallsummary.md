---
title: mobileAppInstallSummary 资源类型
description: 包含移动应用程序的安装摘要的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f8f61fa7d4f23ddb86e7a02d7ad0233e6a34edd8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797802"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="d1fb8-103">mobileAppInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1fb8-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="d1fb8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1fb8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1fb8-106">包含移动应用程序的安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-106">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="d1fb8-107">方法</span><span class="sxs-lookup"><span data-stu-id="d1fb8-107">Methods</span></span>
|<span data-ttu-id="d1fb8-108">方法</span><span class="sxs-lookup"><span data-stu-id="d1fb8-108">Method</span></span>|<span data-ttu-id="d1fb8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d1fb8-109">Return Type</span></span>|<span data-ttu-id="d1fb8-110">说明</span><span class="sxs-lookup"><span data-stu-id="d1fb8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d1fb8-111">获取 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d1fb8-111">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="d1fb8-112">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d1fb8-112">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="d1fb8-113">读取[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-113">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="d1fb8-114">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d1fb8-114">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="d1fb8-115">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d1fb8-115">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="d1fb8-116">更新[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-116">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1fb8-117">属性</span><span class="sxs-lookup"><span data-stu-id="d1fb8-117">Properties</span></span>
|<span data-ttu-id="d1fb8-118">属性</span><span class="sxs-lookup"><span data-stu-id="d1fb8-118">Property</span></span>|<span data-ttu-id="d1fb8-119">类型</span><span class="sxs-lookup"><span data-stu-id="d1fb8-119">Type</span></span>|<span data-ttu-id="d1fb8-120">说明</span><span class="sxs-lookup"><span data-stu-id="d1fb8-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1fb8-121">id</span><span class="sxs-lookup"><span data-stu-id="d1fb8-121">id</span></span>|<span data-ttu-id="d1fb8-122">String</span><span class="sxs-lookup"><span data-stu-id="d1fb8-122">String</span></span>|<span data-ttu-id="d1fb8-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-123">Key of the entity.</span></span>|
|<span data-ttu-id="d1fb8-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-124">installedDeviceCount</span></span>|<span data-ttu-id="d1fb8-125">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-125">Int32</span></span>|<span data-ttu-id="d1fb8-126">已成功安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-126">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="d1fb8-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-127">failedDeviceCount</span></span>|<span data-ttu-id="d1fb8-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-128">Int32</span></span>|<span data-ttu-id="d1fb8-129">安装此应用失败的设备数量。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-129">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="d1fb8-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="d1fb8-131">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-131">Int32</span></span>|<span data-ttu-id="d1fb8-132">不适用于此应用程序的设备数量。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-132">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="d1fb8-133">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-133">notInstalledDeviceCount</span></span>|<span data-ttu-id="d1fb8-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-134">Int32</span></span>|<span data-ttu-id="d1fb8-135">未安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-135">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="d1fb8-136">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-136">pendingInstallDeviceCount</span></span>|<span data-ttu-id="d1fb8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-137">Int32</span></span>|<span data-ttu-id="d1fb8-138">已通知安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-138">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="d1fb8-139">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-139">installedUserCount</span></span>|<span data-ttu-id="d1fb8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-140">Int32</span></span>|<span data-ttu-id="d1fb8-141">其设备已成功安装此应用程序的用户数。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-141">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="d1fb8-142">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-142">failedUserCount</span></span>|<span data-ttu-id="d1fb8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-143">Int32</span></span>|<span data-ttu-id="d1fb8-144">具有1个或多个无法安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-144">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="d1fb8-145">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-145">notApplicableUserCount</span></span>|<span data-ttu-id="d1fb8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-146">Int32</span></span>|<span data-ttu-id="d1fb8-147">其设备全部不适用于此应用的用户数。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-147">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="d1fb8-148">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-148">notInstalledUserCount</span></span>|<span data-ttu-id="d1fb8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-149">Int32</span></span>|<span data-ttu-id="d1fb8-150">具有1个或多个未安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-150">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="d1fb8-151">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="d1fb8-151">pendingInstallUserCount</span></span>|<span data-ttu-id="d1fb8-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d1fb8-152">Int32</span></span>|<span data-ttu-id="d1fb8-153">具有1个或多个设备且已收到安装此应用程序并有0个设备出现故障的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-153">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1fb8-154">关系</span><span class="sxs-lookup"><span data-stu-id="d1fb8-154">Relationships</span></span>
<span data-ttu-id="d1fb8-155">无</span><span class="sxs-lookup"><span data-stu-id="d1fb8-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1fb8-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1fb8-156">JSON Representation</span></span>
<span data-ttu-id="d1fb8-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1fb8-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```



