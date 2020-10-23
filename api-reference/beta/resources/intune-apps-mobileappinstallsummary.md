---
title: mobileAppInstallSummary 资源类型
description: 包含移动应用程序的安装摘要的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dbe40a14569a4a073da333d9df684069d0c457ac
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48721523"
---
# <a name="mobileappinstallsummary-resource-type"></a><span data-ttu-id="5dde9-103">mobileAppInstallSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="5dde9-103">mobileAppInstallSummary resource type</span></span>

<span data-ttu-id="5dde9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dde9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5dde9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5dde9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dde9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5dde9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dde9-107">包含移动应用程序的安装摘要的属性。</span><span class="sxs-lookup"><span data-stu-id="5dde9-107">Contains properties for the installation summary of a mobile app.</span></span>

## <a name="methods"></a><span data-ttu-id="5dde9-108">Methods</span><span class="sxs-lookup"><span data-stu-id="5dde9-108">Methods</span></span>
|<span data-ttu-id="5dde9-109">方法</span><span class="sxs-lookup"><span data-stu-id="5dde9-109">Method</span></span>|<span data-ttu-id="5dde9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5dde9-110">Return Type</span></span>|<span data-ttu-id="5dde9-111">说明</span><span class="sxs-lookup"><span data-stu-id="5dde9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5dde9-112">获取 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5dde9-112">Get mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-get.md)|[<span data-ttu-id="5dde9-113">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5dde9-113">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="5dde9-114">读取 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5dde9-114">Read properties and relationships of the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="5dde9-115">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5dde9-115">Update mobileAppInstallSummary</span></span>](../api/intune-apps-mobileappinstallsummary-update.md)|[<span data-ttu-id="5dde9-116">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="5dde9-116">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="5dde9-117">更新 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5dde9-117">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5dde9-118">属性</span><span class="sxs-lookup"><span data-stu-id="5dde9-118">Properties</span></span>
|<span data-ttu-id="5dde9-119">属性</span><span class="sxs-lookup"><span data-stu-id="5dde9-119">Property</span></span>|<span data-ttu-id="5dde9-120">类型</span><span class="sxs-lookup"><span data-stu-id="5dde9-120">Type</span></span>|<span data-ttu-id="5dde9-121">说明</span><span class="sxs-lookup"><span data-stu-id="5dde9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dde9-122">id</span><span class="sxs-lookup"><span data-stu-id="5dde9-122">id</span></span>|<span data-ttu-id="5dde9-123">String</span><span class="sxs-lookup"><span data-stu-id="5dde9-123">String</span></span>|<span data-ttu-id="5dde9-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5dde9-124">Key of the entity.</span></span>|
|<span data-ttu-id="5dde9-125">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-125">installedDeviceCount</span></span>|<span data-ttu-id="5dde9-126">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-126">Int32</span></span>|<span data-ttu-id="5dde9-127">已成功安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="5dde9-127">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="5dde9-128">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-128">failedDeviceCount</span></span>|<span data-ttu-id="5dde9-129">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-129">Int32</span></span>|<span data-ttu-id="5dde9-130">安装此应用失败的设备数量。</span><span class="sxs-lookup"><span data-stu-id="5dde9-130">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="5dde9-131">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-131">notApplicableDeviceCount</span></span>|<span data-ttu-id="5dde9-132">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-132">Int32</span></span>|<span data-ttu-id="5dde9-133">不适用于此应用程序的设备数量。</span><span class="sxs-lookup"><span data-stu-id="5dde9-133">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="5dde9-134">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-134">notInstalledDeviceCount</span></span>|<span data-ttu-id="5dde9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-135">Int32</span></span>|<span data-ttu-id="5dde9-136">未安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="5dde9-136">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="5dde9-137">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-137">pendingInstallDeviceCount</span></span>|<span data-ttu-id="5dde9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-138">Int32</span></span>|<span data-ttu-id="5dde9-139">已通知安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="5dde9-139">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="5dde9-140">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-140">installedUserCount</span></span>|<span data-ttu-id="5dde9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-141">Int32</span></span>|<span data-ttu-id="5dde9-142">其设备已成功安装此应用程序的用户数。</span><span class="sxs-lookup"><span data-stu-id="5dde9-142">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="5dde9-143">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-143">failedUserCount</span></span>|<span data-ttu-id="5dde9-144">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-144">Int32</span></span>|<span data-ttu-id="5dde9-145">具有1个或多个无法安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="5dde9-145">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="5dde9-146">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-146">notApplicableUserCount</span></span>|<span data-ttu-id="5dde9-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-147">Int32</span></span>|<span data-ttu-id="5dde9-148">其设备全部不适用于此应用的用户数。</span><span class="sxs-lookup"><span data-stu-id="5dde9-148">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="5dde9-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-149">notInstalledUserCount</span></span>|<span data-ttu-id="5dde9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-150">Int32</span></span>|<span data-ttu-id="5dde9-151">具有1个或多个未安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="5dde9-151">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="5dde9-152">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="5dde9-152">pendingInstallUserCount</span></span>|<span data-ttu-id="5dde9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5dde9-153">Int32</span></span>|<span data-ttu-id="5dde9-154">具有1个或多个设备且已收到安装此应用程序并有0个设备出现故障的用户数量。</span><span class="sxs-lookup"><span data-stu-id="5dde9-154">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dde9-155">关系</span><span class="sxs-lookup"><span data-stu-id="5dde9-155">Relationships</span></span>
<span data-ttu-id="5dde9-156">无</span><span class="sxs-lookup"><span data-stu-id="5dde9-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5dde9-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5dde9-157">JSON Representation</span></span>
<span data-ttu-id="5dde9-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dde9-158">Here is a JSON representation of the resource.</span></span>
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





