---
title: mobileAppInstallSummary 资源类型
description: 包含移动应用程序的安装摘要的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9747d53c56f9e505b61e1fa38bf5abdc27d14e42
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150762"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="13961-103">mobileAppInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="13961-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="13961-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13961-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13961-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13961-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13961-106">包含移动应用程序的安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="13961-106">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="13961-107">方法</span><span class="sxs-lookup"><span data-stu-id="13961-107">Methods</span></span>
|<span data-ttu-id="13961-108">方法</span><span class="sxs-lookup"><span data-stu-id="13961-108">Method</span></span>|<span data-ttu-id="13961-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="13961-109">Return Type</span></span>|<span data-ttu-id="13961-110">说明</span><span class="sxs-lookup"><span data-stu-id="13961-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13961-111">获取 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="13961-111">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="13961-112">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="13961-112">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="13961-113">读取[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13961-113">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="13961-114">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="13961-114">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="13961-115">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="13961-115">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="13961-116">更新[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13961-116">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13961-117">属性</span><span class="sxs-lookup"><span data-stu-id="13961-117">Properties</span></span>
|<span data-ttu-id="13961-118">属性</span><span class="sxs-lookup"><span data-stu-id="13961-118">Property</span></span>|<span data-ttu-id="13961-119">类型</span><span class="sxs-lookup"><span data-stu-id="13961-119">Type</span></span>|<span data-ttu-id="13961-120">说明</span><span class="sxs-lookup"><span data-stu-id="13961-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13961-121">id</span><span class="sxs-lookup"><span data-stu-id="13961-121">id</span></span>|<span data-ttu-id="13961-122">String</span><span class="sxs-lookup"><span data-stu-id="13961-122">String</span></span>|<span data-ttu-id="13961-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="13961-123">Key of the entity.</span></span>|
|<span data-ttu-id="13961-124">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13961-124">installedDeviceCount</span></span>|<span data-ttu-id="13961-125">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-125">Int32</span></span>|<span data-ttu-id="13961-126">已成功安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="13961-126">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="13961-127">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13961-127">failedDeviceCount</span></span>|<span data-ttu-id="13961-128">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-128">Int32</span></span>|<span data-ttu-id="13961-129">安装此应用失败的设备数量。</span><span class="sxs-lookup"><span data-stu-id="13961-129">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="13961-130">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13961-130">notApplicableDeviceCount</span></span>|<span data-ttu-id="13961-131">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-131">Int32</span></span>|<span data-ttu-id="13961-132">不适用于此应用程序的设备数量。</span><span class="sxs-lookup"><span data-stu-id="13961-132">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="13961-133">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13961-133">notInstalledDeviceCount</span></span>|<span data-ttu-id="13961-134">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-134">Int32</span></span>|<span data-ttu-id="13961-135">未安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="13961-135">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="13961-136">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="13961-136">pendingInstallDeviceCount</span></span>|<span data-ttu-id="13961-137">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-137">Int32</span></span>|<span data-ttu-id="13961-138">已通知安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="13961-138">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="13961-139">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="13961-139">installedUserCount</span></span>|<span data-ttu-id="13961-140">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-140">Int32</span></span>|<span data-ttu-id="13961-141">其设备已成功安装此应用程序的用户数。</span><span class="sxs-lookup"><span data-stu-id="13961-141">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="13961-142">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="13961-142">failedUserCount</span></span>|<span data-ttu-id="13961-143">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-143">Int32</span></span>|<span data-ttu-id="13961-144">具有1个或多个无法安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="13961-144">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="13961-145">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="13961-145">notApplicableUserCount</span></span>|<span data-ttu-id="13961-146">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-146">Int32</span></span>|<span data-ttu-id="13961-147">其设备全部不适用于此应用的用户数。</span><span class="sxs-lookup"><span data-stu-id="13961-147">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="13961-148">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="13961-148">notInstalledUserCount</span></span>|<span data-ttu-id="13961-149">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-149">Int32</span></span>|<span data-ttu-id="13961-150">具有1个或多个未安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="13961-150">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="13961-151">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="13961-151">pendingInstallUserCount</span></span>|<span data-ttu-id="13961-152">Int32</span><span class="sxs-lookup"><span data-stu-id="13961-152">Int32</span></span>|<span data-ttu-id="13961-153">具有1个或多个设备且已收到安装此应用程序并有0个设备出现故障的用户数量。</span><span class="sxs-lookup"><span data-stu-id="13961-153">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13961-154">关系</span><span class="sxs-lookup"><span data-stu-id="13961-154">Relationships</span></span>
<span data-ttu-id="13961-155">无</span><span class="sxs-lookup"><span data-stu-id="13961-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13961-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13961-156">JSON Representation</span></span>
<span data-ttu-id="13961-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13961-157">Here is a JSON representation of the resource.</span></span>
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




