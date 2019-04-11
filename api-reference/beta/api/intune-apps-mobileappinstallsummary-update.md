---
title: 更新 mobileAppInstallSummary
description: 更新 mobileAppInstallSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17389db16c5080c3ca13fa21f77437483d0be64a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791857"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="74699-103">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="74699-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="74699-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74699-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74699-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74699-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74699-106">更新[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="74699-106">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74699-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="74699-107">Prerequisites</span></span>
<span data-ttu-id="74699-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74699-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74699-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="74699-110">Permission type</span></span>|<span data-ttu-id="74699-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="74699-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74699-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74699-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74699-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74699-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="74699-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74699-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74699-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="74699-115">Not supported.</span></span>|
|<span data-ttu-id="74699-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="74699-116">Application</span></span>|<span data-ttu-id="74699-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="74699-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74699-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74699-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="74699-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="74699-119">Request headers</span></span>
|<span data-ttu-id="74699-120">标头</span><span class="sxs-lookup"><span data-stu-id="74699-120">Header</span></span>|<span data-ttu-id="74699-121">值</span><span class="sxs-lookup"><span data-stu-id="74699-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74699-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="74699-122">Authorization</span></span>|<span data-ttu-id="74699-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="74699-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74699-124">接受</span><span class="sxs-lookup"><span data-stu-id="74699-124">Accept</span></span>|<span data-ttu-id="74699-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74699-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74699-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="74699-126">Request body</span></span>
<span data-ttu-id="74699-127">在请求正文中, 提供[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74699-127">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="74699-128">下表显示创建[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74699-128">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="74699-129">属性</span><span class="sxs-lookup"><span data-stu-id="74699-129">Property</span></span>|<span data-ttu-id="74699-130">类型</span><span class="sxs-lookup"><span data-stu-id="74699-130">Type</span></span>|<span data-ttu-id="74699-131">说明</span><span class="sxs-lookup"><span data-stu-id="74699-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74699-132">id</span><span class="sxs-lookup"><span data-stu-id="74699-132">id</span></span>|<span data-ttu-id="74699-133">String</span><span class="sxs-lookup"><span data-stu-id="74699-133">String</span></span>|<span data-ttu-id="74699-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="74699-134">Key of the entity.</span></span>|
|<span data-ttu-id="74699-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74699-135">installedDeviceCount</span></span>|<span data-ttu-id="74699-136">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-136">Int32</span></span>|<span data-ttu-id="74699-137">已成功安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="74699-137">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="74699-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74699-138">failedDeviceCount</span></span>|<span data-ttu-id="74699-139">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-139">Int32</span></span>|<span data-ttu-id="74699-140">安装此应用失败的设备数量。</span><span class="sxs-lookup"><span data-stu-id="74699-140">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="74699-141">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74699-141">notApplicableDeviceCount</span></span>|<span data-ttu-id="74699-142">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-142">Int32</span></span>|<span data-ttu-id="74699-143">不适用于此应用程序的设备数量。</span><span class="sxs-lookup"><span data-stu-id="74699-143">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="74699-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74699-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="74699-145">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-145">Int32</span></span>|<span data-ttu-id="74699-146">未安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="74699-146">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="74699-147">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="74699-147">pendingInstallDeviceCount</span></span>|<span data-ttu-id="74699-148">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-148">Int32</span></span>|<span data-ttu-id="74699-149">已通知安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="74699-149">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="74699-150">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="74699-150">installedUserCount</span></span>|<span data-ttu-id="74699-151">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-151">Int32</span></span>|<span data-ttu-id="74699-152">其设备已成功安装此应用程序的用户数。</span><span class="sxs-lookup"><span data-stu-id="74699-152">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="74699-153">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="74699-153">failedUserCount</span></span>|<span data-ttu-id="74699-154">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-154">Int32</span></span>|<span data-ttu-id="74699-155">具有1个或多个无法安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="74699-155">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="74699-156">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="74699-156">notApplicableUserCount</span></span>|<span data-ttu-id="74699-157">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-157">Int32</span></span>|<span data-ttu-id="74699-158">其设备全部不适用于此应用的用户数。</span><span class="sxs-lookup"><span data-stu-id="74699-158">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="74699-159">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="74699-159">notInstalledUserCount</span></span>|<span data-ttu-id="74699-160">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-160">Int32</span></span>|<span data-ttu-id="74699-161">具有1个或多个未安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="74699-161">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="74699-162">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="74699-162">pendingInstallUserCount</span></span>|<span data-ttu-id="74699-163">Int32</span><span class="sxs-lookup"><span data-stu-id="74699-163">Int32</span></span>|<span data-ttu-id="74699-164">具有1个或多个设备且已收到安装此应用程序并有0个设备出现故障的用户数量。</span><span class="sxs-lookup"><span data-stu-id="74699-164">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="74699-165">响应</span><span class="sxs-lookup"><span data-stu-id="74699-165">Response</span></span>
<span data-ttu-id="74699-166">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="74699-166">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74699-167">示例</span><span class="sxs-lookup"><span data-stu-id="74699-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="74699-168">请求</span><span class="sxs-lookup"><span data-stu-id="74699-168">Request</span></span>
<span data-ttu-id="74699-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74699-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```

### <a name="response"></a><span data-ttu-id="74699-170">响应</span><span class="sxs-lookup"><span data-stu-id="74699-170">Response</span></span>
<span data-ttu-id="74699-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74699-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "06a792e9-92e9-06a7-e992-a706e992a706",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notApplicableDeviceCount": 8,
  "notInstalledDeviceCount": 7,
  "pendingInstallDeviceCount": 9,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notApplicableUserCount": 6,
  "notInstalledUserCount": 5,
  "pendingInstallUserCount": 7
}
```





