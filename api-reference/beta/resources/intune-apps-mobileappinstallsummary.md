---
title: mobileAppInstallSummary 资源类型
description: 包含的移动应用程序安装摘要属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3b730f73b8a86c8acba531ab0d30a67b2f8e7a7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820354"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="cce49-103">mobileAppInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="cce49-103">mobileAppInstallSummary resource type</span></span>

> <span data-ttu-id="cce49-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cce49-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cce49-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cce49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cce49-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cce49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cce49-107">包含的移动应用程序安装摘要属性。</span><span class="sxs-lookup"><span data-stu-id="cce49-107">Contains properties for the installation summary of a mobile app.</span></span>
## <a name="methods"></a><span data-ttu-id="cce49-108">方法</span><span class="sxs-lookup"><span data-stu-id="cce49-108">Methods</span></span>
|<span data-ttu-id="cce49-109">方法</span><span class="sxs-lookup"><span data-stu-id="cce49-109">Method</span></span>|<span data-ttu-id="cce49-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cce49-110">Return Type</span></span>|<span data-ttu-id="cce49-111">说明</span><span class="sxs-lookup"><span data-stu-id="cce49-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cce49-112">获取 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cce49-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="cce49-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cce49-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="cce49-114">读取属性和[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="cce49-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="cce49-115">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cce49-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="cce49-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="cce49-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="cce49-117">更新[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cce49-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cce49-118">属性</span><span class="sxs-lookup"><span data-stu-id="cce49-118">Properties</span></span>
|<span data-ttu-id="cce49-119">属性</span><span class="sxs-lookup"><span data-stu-id="cce49-119">Property</span></span>|<span data-ttu-id="cce49-120">类型</span><span class="sxs-lookup"><span data-stu-id="cce49-120">Type</span></span>|<span data-ttu-id="cce49-121">说明</span><span class="sxs-lookup"><span data-stu-id="cce49-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cce49-122">id</span><span class="sxs-lookup"><span data-stu-id="cce49-122">id</span></span>|<span data-ttu-id="cce49-123">String</span><span class="sxs-lookup"><span data-stu-id="cce49-123">String</span></span>|<span data-ttu-id="cce49-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cce49-124">Key of the entity.</span></span>|
|<span data-ttu-id="cce49-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cce49-125">installedDeviceCount</span></span>|<span data-ttu-id="cce49-126">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-126">Int32</span></span>|<span data-ttu-id="cce49-127">已成功安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="cce49-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="cce49-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cce49-128">failedDeviceCount</span></span>|<span data-ttu-id="cce49-129">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-129">Int32</span></span>|<span data-ttu-id="cce49-130">未能安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="cce49-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="cce49-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cce49-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="cce49-132">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-132">Int32</span></span>|<span data-ttu-id="cce49-133">不适用于此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="cce49-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="cce49-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cce49-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="cce49-135">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-135">Int32</span></span>|<span data-ttu-id="cce49-136">没有安装该应用程序的设备数目。</span><span class="sxs-lookup"><span data-stu-id="cce49-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="cce49-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cce49-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="cce49-138">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-138">Int32</span></span>|<span data-ttu-id="cce49-139">已被通知安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="cce49-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="cce49-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="cce49-140">installedUserCount</span></span>|<span data-ttu-id="cce49-141">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-141">Int32</span></span>|<span data-ttu-id="cce49-142">所有成功安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="cce49-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="cce49-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="cce49-143">failedUserCount</span></span>|<span data-ttu-id="cce49-144">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-144">Int32</span></span>|<span data-ttu-id="cce49-145">用户具有 1 或无法安装此应用程序的更多设备数。</span><span class="sxs-lookup"><span data-stu-id="cce49-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="cce49-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="cce49-146">notApplicableUserCount</span></span>|<span data-ttu-id="cce49-147">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-147">Int32</span></span>|<span data-ttu-id="cce49-148">其设备未所有适用于此应用程序的用户数。</span><span class="sxs-lookup"><span data-stu-id="cce49-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="cce49-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="cce49-149">notInstalledUserCount</span></span>|<span data-ttu-id="cce49-150">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-150">Int32</span></span>|<span data-ttu-id="cce49-151">未安装该应用程序的一个或多个设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="cce49-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="cce49-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="cce49-152">pendingInstallUserCount</span></span>|<span data-ttu-id="cce49-153">Int32</span><span class="sxs-lookup"><span data-stu-id="cce49-153">Int32</span></span>|<span data-ttu-id="cce49-154">用户具有 1 或更多已经通知安装此应用程序和失败的 0 设备的设备数。</span><span class="sxs-lookup"><span data-stu-id="cce49-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cce49-155">Relationships</span><span class="sxs-lookup"><span data-stu-id="cce49-155">Relationships</span></span>
<span data-ttu-id="cce49-156">无</span><span class="sxs-lookup"><span data-stu-id="cce49-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cce49-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cce49-157">JSON Representation</span></span>
<span data-ttu-id="cce49-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cce49-158">Here is a JSON representation of the resource.</span></span>
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





