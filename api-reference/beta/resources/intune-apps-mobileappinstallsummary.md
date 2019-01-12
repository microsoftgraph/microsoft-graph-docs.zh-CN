---
title: mobileAppInstallSummary 资源类型
description: 包含的移动应用程序安装摘要属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a75dba8303d254aff911cc66931d52abb8b76c07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916024"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="7d5c5-103">mobileAppInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d5c5-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="7d5c5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d5c5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d5c5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d5c5-107">包含的移动应用程序安装摘要属性。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-107">Contains properties for the installation summary of a mobile app.</span></span>
## <a name="methods"></a><span data-ttu-id="7d5c5-108">方法</span><span class="sxs-lookup"><span data-stu-id="7d5c5-108">Methods</span></span>
|<span data-ttu-id="7d5c5-109">方法</span><span class="sxs-lookup"><span data-stu-id="7d5c5-109">Method</span></span>|<span data-ttu-id="7d5c5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7d5c5-110">Return Type</span></span>|<span data-ttu-id="7d5c5-111">说明</span><span class="sxs-lookup"><span data-stu-id="7d5c5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7d5c5-112">获取 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7d5c5-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="7d5c5-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7d5c5-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="7d5c5-114">读取属性和[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="7d5c5-115">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7d5c5-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="7d5c5-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7d5c5-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="7d5c5-117">更新[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7d5c5-118">属性</span><span class="sxs-lookup"><span data-stu-id="7d5c5-118">Properties</span></span>
|<span data-ttu-id="7d5c5-119">属性</span><span class="sxs-lookup"><span data-stu-id="7d5c5-119">Property</span></span>|<span data-ttu-id="7d5c5-120">类型</span><span class="sxs-lookup"><span data-stu-id="7d5c5-120">Type</span></span>|<span data-ttu-id="7d5c5-121">说明</span><span class="sxs-lookup"><span data-stu-id="7d5c5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d5c5-122">id</span><span class="sxs-lookup"><span data-stu-id="7d5c5-122">id</span></span>|<span data-ttu-id="7d5c5-123">String</span><span class="sxs-lookup"><span data-stu-id="7d5c5-123">String</span></span>|<span data-ttu-id="7d5c5-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-124">Key of the entity.</span></span>|
|<span data-ttu-id="7d5c5-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-125">installedDeviceCount</span></span>|<span data-ttu-id="7d5c5-126">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-126">Int32</span></span>|<span data-ttu-id="7d5c5-127">已成功安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="7d5c5-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-128">failedDeviceCount</span></span>|<span data-ttu-id="7d5c5-129">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-129">Int32</span></span>|<span data-ttu-id="7d5c5-130">未能安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="7d5c5-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="7d5c5-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-132">Int32</span></span>|<span data-ttu-id="7d5c5-133">不适用于此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="7d5c5-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="7d5c5-135">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-135">Int32</span></span>|<span data-ttu-id="7d5c5-136">没有安装该应用程序的设备数目。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="7d5c5-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="7d5c5-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-138">Int32</span></span>|<span data-ttu-id="7d5c5-139">已被通知安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="7d5c5-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-140">installedUserCount</span></span>|<span data-ttu-id="7d5c5-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-141">Int32</span></span>|<span data-ttu-id="7d5c5-142">所有成功安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="7d5c5-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-143">failedUserCount</span></span>|<span data-ttu-id="7d5c5-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-144">Int32</span></span>|<span data-ttu-id="7d5c5-145">用户具有 1 或无法安装此应用程序的更多设备数。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="7d5c5-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-146">notApplicableUserCount</span></span>|<span data-ttu-id="7d5c5-147">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-147">Int32</span></span>|<span data-ttu-id="7d5c5-148">其设备未所有适用于此应用程序的用户数。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="7d5c5-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-149">notInstalledUserCount</span></span>|<span data-ttu-id="7d5c5-150">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-150">Int32</span></span>|<span data-ttu-id="7d5c5-151">未安装该应用程序的一个或多个设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="7d5c5-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="7d5c5-152">pendingInstallUserCount</span></span>|<span data-ttu-id="7d5c5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7d5c5-153">Int32</span></span>|<span data-ttu-id="7d5c5-154">用户具有 1 或更多已经通知安装此应用程序和失败的 0 设备的设备数。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d5c5-155">Relationships</span><span class="sxs-lookup"><span data-stu-id="7d5c5-155">Relationships</span></span>
<span data-ttu-id="7d5c5-156">无</span><span class="sxs-lookup"><span data-stu-id="7d5c5-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d5c5-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d5c5-157">JSON Representation</span></span>
<span data-ttu-id="7d5c5-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d5c5-158">Here is a JSON representation of the resource.</span></span>
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





