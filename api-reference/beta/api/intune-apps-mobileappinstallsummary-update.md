---
title: 更新 mobileAppInstallSummary
description: 更新 mobileAppInstallSummary 对象的属性。
ms.openlocfilehash: 0fa1343d52fa82c69f6511d3e320ebae2d98a084
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043233"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="2e120-103">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="2e120-103">Update mobileAppInstallSummary</span></span>

> <span data-ttu-id="2e120-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2e120-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e120-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2e120-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e120-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2e120-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e120-107">更新[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2e120-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e120-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2e120-108">Prerequisites</span></span>
<span data-ttu-id="2e120-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2e120-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e120-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e120-111">Permission type</span></span>|<span data-ttu-id="2e120-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2e120-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e120-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e120-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e120-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e120-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e120-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e120-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e120-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e120-116">Not supported.</span></span>|
|<span data-ttu-id="2e120-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e120-117">Application</span></span>|<span data-ttu-id="2e120-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e120-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e120-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e120-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="2e120-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e120-120">Request headers</span></span>
|<span data-ttu-id="2e120-121">标头</span><span class="sxs-lookup"><span data-stu-id="2e120-121">Header</span></span>|<span data-ttu-id="2e120-122">值</span><span class="sxs-lookup"><span data-stu-id="2e120-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e120-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e120-123">Authorization</span></span>|<span data-ttu-id="2e120-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2e120-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e120-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2e120-125">Accept</span></span>|<span data-ttu-id="2e120-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e120-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e120-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e120-127">Request body</span></span>
<span data-ttu-id="2e120-128">在请求正文中，提供[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e120-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="2e120-129">下表显示时创建[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2e120-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="2e120-130">属性</span><span class="sxs-lookup"><span data-stu-id="2e120-130">Property</span></span>|<span data-ttu-id="2e120-131">类型</span><span class="sxs-lookup"><span data-stu-id="2e120-131">Type</span></span>|<span data-ttu-id="2e120-132">说明</span><span class="sxs-lookup"><span data-stu-id="2e120-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e120-133">id</span><span class="sxs-lookup"><span data-stu-id="2e120-133">id</span></span>|<span data-ttu-id="2e120-134">String</span><span class="sxs-lookup"><span data-stu-id="2e120-134">String</span></span>|<span data-ttu-id="2e120-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2e120-135">Key of the entity.</span></span>|
|<span data-ttu-id="2e120-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e120-136">installedDeviceCount</span></span>|<span data-ttu-id="2e120-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-137">Int32</span></span>|<span data-ttu-id="2e120-138">已成功安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="2e120-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="2e120-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e120-139">failedDeviceCount</span></span>|<span data-ttu-id="2e120-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-140">Int32</span></span>|<span data-ttu-id="2e120-141">未能安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="2e120-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="2e120-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e120-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="2e120-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-143">Int32</span></span>|<span data-ttu-id="2e120-144">不适用于此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="2e120-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="2e120-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e120-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="2e120-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-146">Int32</span></span>|<span data-ttu-id="2e120-147">没有安装该应用程序的设备数目。</span><span class="sxs-lookup"><span data-stu-id="2e120-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="2e120-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2e120-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="2e120-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-149">Int32</span></span>|<span data-ttu-id="2e120-150">已被通知安装此应用程序的设备数。</span><span class="sxs-lookup"><span data-stu-id="2e120-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="2e120-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="2e120-151">installedUserCount</span></span>|<span data-ttu-id="2e120-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-152">Int32</span></span>|<span data-ttu-id="2e120-153">所有成功安装此应用程序的设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="2e120-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="2e120-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="2e120-154">failedUserCount</span></span>|<span data-ttu-id="2e120-155">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-155">Int32</span></span>|<span data-ttu-id="2e120-156">用户具有 1 或无法安装此应用程序的更多设备数。</span><span class="sxs-lookup"><span data-stu-id="2e120-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="2e120-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="2e120-157">notApplicableUserCount</span></span>|<span data-ttu-id="2e120-158">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-158">Int32</span></span>|<span data-ttu-id="2e120-159">其设备未所有适用于此应用程序的用户数。</span><span class="sxs-lookup"><span data-stu-id="2e120-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="2e120-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="2e120-160">notInstalledUserCount</span></span>|<span data-ttu-id="2e120-161">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-161">Int32</span></span>|<span data-ttu-id="2e120-162">未安装该应用程序的一个或多个设备的用户数。</span><span class="sxs-lookup"><span data-stu-id="2e120-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="2e120-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="2e120-163">pendingInstallUserCount</span></span>|<span data-ttu-id="2e120-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2e120-164">Int32</span></span>|<span data-ttu-id="2e120-165">用户具有 1 或更多已经通知安装此应用程序和失败的 0 设备的设备数。</span><span class="sxs-lookup"><span data-stu-id="2e120-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="2e120-166">响应</span><span class="sxs-lookup"><span data-stu-id="2e120-166">Response</span></span>
<span data-ttu-id="2e120-167">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2e120-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e120-168">示例</span><span class="sxs-lookup"><span data-stu-id="2e120-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e120-169">请求</span><span class="sxs-lookup"><span data-stu-id="2e120-169">Request</span></span>
<span data-ttu-id="2e120-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e120-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-type: application/json
Content-length: 312

{
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

### <a name="response"></a><span data-ttu-id="2e120-171">响应</span><span class="sxs-lookup"><span data-stu-id="2e120-171">Response</span></span>
<span data-ttu-id="2e120-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e120-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





