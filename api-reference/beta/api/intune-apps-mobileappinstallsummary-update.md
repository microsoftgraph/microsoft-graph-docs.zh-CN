---
title: 更新 mobileAppInstallSummary
description: 更新 mobileAppInstallSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4efc32b475500150a0ab3685c7ff153593e426ee
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723698"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="f4cad-103">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="f4cad-103">Update mobileAppInstallSummary</span></span>

<span data-ttu-id="f4cad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4cad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4cad-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4cad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4cad-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4cad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4cad-107">更新 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4cad-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4cad-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4cad-108">Prerequisites</span></span>
<span data-ttu-id="f4cad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4cad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4cad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4cad-111">Permission type</span></span>|<span data-ttu-id="f4cad-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4cad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4cad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4cad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4cad-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4cad-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f4cad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4cad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4cad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4cad-116">Not supported.</span></span>|
|<span data-ttu-id="f4cad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4cad-117">Application</span></span>|<span data-ttu-id="f4cad-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4cad-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4cad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4cad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="f4cad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4cad-120">Request headers</span></span>
|<span data-ttu-id="f4cad-121">标头</span><span class="sxs-lookup"><span data-stu-id="f4cad-121">Header</span></span>|<span data-ttu-id="f4cad-122">值</span><span class="sxs-lookup"><span data-stu-id="f4cad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4cad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4cad-123">Authorization</span></span>|<span data-ttu-id="f4cad-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4cad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4cad-125">接受</span><span class="sxs-lookup"><span data-stu-id="f4cad-125">Accept</span></span>|<span data-ttu-id="f4cad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4cad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4cad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4cad-127">Request body</span></span>
<span data-ttu-id="f4cad-128">在请求正文中，提供 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4cad-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="f4cad-129">下表显示创建 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4cad-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="f4cad-130">属性</span><span class="sxs-lookup"><span data-stu-id="f4cad-130">Property</span></span>|<span data-ttu-id="f4cad-131">类型</span><span class="sxs-lookup"><span data-stu-id="f4cad-131">Type</span></span>|<span data-ttu-id="f4cad-132">说明</span><span class="sxs-lookup"><span data-stu-id="f4cad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4cad-133">id</span><span class="sxs-lookup"><span data-stu-id="f4cad-133">id</span></span>|<span data-ttu-id="f4cad-134">String</span><span class="sxs-lookup"><span data-stu-id="f4cad-134">String</span></span>|<span data-ttu-id="f4cad-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4cad-135">Key of the entity.</span></span>|
|<span data-ttu-id="f4cad-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-136">installedDeviceCount</span></span>|<span data-ttu-id="f4cad-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-137">Int32</span></span>|<span data-ttu-id="f4cad-138">已成功安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f4cad-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="f4cad-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-139">failedDeviceCount</span></span>|<span data-ttu-id="f4cad-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-140">Int32</span></span>|<span data-ttu-id="f4cad-141">安装此应用失败的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f4cad-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="f4cad-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="f4cad-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-143">Int32</span></span>|<span data-ttu-id="f4cad-144">不适用于此应用程序的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f4cad-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="f4cad-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="f4cad-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-146">Int32</span></span>|<span data-ttu-id="f4cad-147">未安装此应用的设备数量。</span><span class="sxs-lookup"><span data-stu-id="f4cad-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="f4cad-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="f4cad-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-149">Int32</span></span>|<span data-ttu-id="f4cad-150">已通知安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="f4cad-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="f4cad-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-151">installedUserCount</span></span>|<span data-ttu-id="f4cad-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-152">Int32</span></span>|<span data-ttu-id="f4cad-153">其设备已成功安装此应用程序的用户数。</span><span class="sxs-lookup"><span data-stu-id="f4cad-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="f4cad-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-154">failedUserCount</span></span>|<span data-ttu-id="f4cad-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-155">Int32</span></span>|<span data-ttu-id="f4cad-156">具有1个或多个无法安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="f4cad-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="f4cad-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-157">notApplicableUserCount</span></span>|<span data-ttu-id="f4cad-158">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-158">Int32</span></span>|<span data-ttu-id="f4cad-159">其设备全部不适用于此应用的用户数。</span><span class="sxs-lookup"><span data-stu-id="f4cad-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="f4cad-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-160">notInstalledUserCount</span></span>|<span data-ttu-id="f4cad-161">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-161">Int32</span></span>|<span data-ttu-id="f4cad-162">具有1个或多个未安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="f4cad-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="f4cad-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="f4cad-163">pendingInstallUserCount</span></span>|<span data-ttu-id="f4cad-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f4cad-164">Int32</span></span>|<span data-ttu-id="f4cad-165">具有1个或多个设备且已收到安装此应用程序并有0个设备出现故障的用户数量。</span><span class="sxs-lookup"><span data-stu-id="f4cad-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="f4cad-166">响应</span><span class="sxs-lookup"><span data-stu-id="f4cad-166">Response</span></span>
<span data-ttu-id="f4cad-167">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4cad-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4cad-168">示例</span><span class="sxs-lookup"><span data-stu-id="f4cad-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4cad-169">请求</span><span class="sxs-lookup"><span data-stu-id="f4cad-169">Request</span></span>
<span data-ttu-id="f4cad-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4cad-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f4cad-171">响应</span><span class="sxs-lookup"><span data-stu-id="f4cad-171">Response</span></span>
<span data-ttu-id="f4cad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4cad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





