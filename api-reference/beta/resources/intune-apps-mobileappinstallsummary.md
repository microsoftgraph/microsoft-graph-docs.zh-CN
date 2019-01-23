---
title: mobileAppInstallSummary 资源类型
description: 包含的移动应用程序安装摘要属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2bd7c30c1b00e83731766bcd80f9a9fafd8e8b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416711"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="d9912-103">mobileAppInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9912-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="d9912-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d9912-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d9912-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9912-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9912-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9912-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9912-107">包含的移动应用程序安装摘要属性。</span><span class="sxs-lookup"><span data-stu-id="d9912-107">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="d9912-108">方法</span><span class="sxs-lookup"><span data-stu-id="d9912-108">Methods</span></span>
|<span data-ttu-id="d9912-109">方法</span><span class="sxs-lookup"><span data-stu-id="d9912-109">Method</span></span>|<span data-ttu-id="d9912-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9912-110">Return Type</span></span>|<span data-ttu-id="d9912-111">说明</span><span class="sxs-lookup"><span data-stu-id="d9912-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9912-112">获取 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d9912-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="d9912-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d9912-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="d9912-114">读取属性和[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d9912-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="d9912-115">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d9912-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="d9912-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d9912-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="d9912-117">更新[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9912-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9912-118">属性</span><span class="sxs-lookup"><span data-stu-id="d9912-118">Properties</span></span>
|<span data-ttu-id="d9912-119">属性</span><span class="sxs-lookup"><span data-stu-id="d9912-119">Property</span></span>|<span data-ttu-id="d9912-120">类型</span><span class="sxs-lookup"><span data-stu-id="d9912-120">Type</span></span>|<span data-ttu-id="d9912-121">说明</span><span class="sxs-lookup"><span data-stu-id="d9912-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9912-122">id</span><span class="sxs-lookup"><span data-stu-id="d9912-122">id</span></span>|<span data-ttu-id="d9912-123">String</span><span class="sxs-lookup"><span data-stu-id="d9912-123">String</span></span>|<span data-ttu-id="d9912-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9912-124">Key of the entity.</span></span>|
|<span data-ttu-id="d9912-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9912-125">installedDeviceCount</span></span>|<span data-ttu-id="d9912-126">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-126">Int32</span></span>|<span data-ttu-id="d9912-127">已成功安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="d9912-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="d9912-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9912-128">failedDeviceCount</span></span>|<span data-ttu-id="d9912-129">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-129">Int32</span></span>|<span data-ttu-id="d9912-130">未能安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="d9912-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="d9912-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9912-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="d9912-132">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-132">Int32</span></span>|<span data-ttu-id="d9912-133">不适用于此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="d9912-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="d9912-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9912-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="d9912-135">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-135">Int32</span></span>|<span data-ttu-id="d9912-136">没有安装该应用程序的设备数目。</span><span class="sxs-lookup"><span data-stu-id="d9912-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="d9912-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d9912-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="d9912-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-138">Int32</span></span>|<span data-ttu-id="d9912-139">已被通知安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="d9912-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="d9912-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="d9912-140">installedUserCount</span></span>|<span data-ttu-id="d9912-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-141">Int32</span></span>|<span data-ttu-id="d9912-142">所有成功安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="d9912-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="d9912-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="d9912-143">failedUserCount</span></span>|<span data-ttu-id="d9912-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-144">Int32</span></span>|<span data-ttu-id="d9912-145">用户具有 1 或无法安装此应用程序的更多设备数。</span><span class="sxs-lookup"><span data-stu-id="d9912-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="d9912-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="d9912-146">notApplicableUserCount</span></span>|<span data-ttu-id="d9912-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-147">Int32</span></span>|<span data-ttu-id="d9912-148">其设备未所有适用于此应用程序的用户数。</span><span class="sxs-lookup"><span data-stu-id="d9912-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="d9912-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="d9912-149">notInstalledUserCount</span></span>|<span data-ttu-id="d9912-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-150">Int32</span></span>|<span data-ttu-id="d9912-151">未安装该应用程序的一个或多个设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="d9912-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="d9912-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="d9912-152">pendingInstallUserCount</span></span>|<span data-ttu-id="d9912-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d9912-153">Int32</span></span>|<span data-ttu-id="d9912-154">用户具有 1 或更多已经通知安装此应用程序和失败的 0 设备的设备数。</span><span class="sxs-lookup"><span data-stu-id="d9912-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9912-155">关系</span><span class="sxs-lookup"><span data-stu-id="d9912-155">Relationships</span></span>
<span data-ttu-id="d9912-156">无</span><span class="sxs-lookup"><span data-stu-id="d9912-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9912-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9912-157">JSON Representation</span></span>
<span data-ttu-id="d9912-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9912-158">Here is a JSON representation of the resource.</span></span>
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




