---
title: 更新 mobileAppInstallSummary
description: 更新 mobileAppInstallSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9ecf2214cd2853112a23c4dab105d32a2e1a839e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143148"
---
# <a name="update-mobileappinstallsummary"></a><span data-ttu-id="d64ff-103">更新 mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d64ff-103">Update mobileAppInstallSummary</span></span>

<span data-ttu-id="d64ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d64ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d64ff-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d64ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d64ff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d64ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d64ff-107">更新 [mobileAppInstallSummary 对象](../resources/intune-apps-mobileappinstallsummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d64ff-107">Update the properties of a [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d64ff-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d64ff-108">Prerequisites</span></span>
<span data-ttu-id="d64ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d64ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d64ff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d64ff-111">Permission type</span></span>|<span data-ttu-id="d64ff-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d64ff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d64ff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d64ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d64ff-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64ff-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d64ff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d64ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d64ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d64ff-116">Not supported.</span></span>|
|<span data-ttu-id="d64ff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d64ff-117">Application</span></span>|<span data-ttu-id="d64ff-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64ff-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d64ff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d64ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="d64ff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d64ff-120">Request headers</span></span>
|<span data-ttu-id="d64ff-121">标头</span><span class="sxs-lookup"><span data-stu-id="d64ff-121">Header</span></span>|<span data-ttu-id="d64ff-122">值</span><span class="sxs-lookup"><span data-stu-id="d64ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d64ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d64ff-123">Authorization</span></span>|<span data-ttu-id="d64ff-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d64ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d64ff-125">接受</span><span class="sxs-lookup"><span data-stu-id="d64ff-125">Accept</span></span>|<span data-ttu-id="d64ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d64ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d64ff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d64ff-127">Request body</span></span>
<span data-ttu-id="d64ff-128">在请求正文中，提供 [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d64ff-128">In the request body, supply a JSON representation for the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object.</span></span>

<span data-ttu-id="d64ff-129">下表显示创建 [mobileAppInstallSummary 时所需的属性](../resources/intune-apps-mobileappinstallsummary.md)。</span><span class="sxs-lookup"><span data-stu-id="d64ff-129">The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md).</span></span>

|<span data-ttu-id="d64ff-130">属性</span><span class="sxs-lookup"><span data-stu-id="d64ff-130">Property</span></span>|<span data-ttu-id="d64ff-131">类型</span><span class="sxs-lookup"><span data-stu-id="d64ff-131">Type</span></span>|<span data-ttu-id="d64ff-132">说明</span><span class="sxs-lookup"><span data-stu-id="d64ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d64ff-133">id</span><span class="sxs-lookup"><span data-stu-id="d64ff-133">id</span></span>|<span data-ttu-id="d64ff-134">String</span><span class="sxs-lookup"><span data-stu-id="d64ff-134">String</span></span>|<span data-ttu-id="d64ff-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d64ff-135">Key of the entity.</span></span>|
|<span data-ttu-id="d64ff-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-136">installedDeviceCount</span></span>|<span data-ttu-id="d64ff-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-137">Int32</span></span>|<span data-ttu-id="d64ff-138">已成功安装此应用的设备数。</span><span class="sxs-lookup"><span data-stu-id="d64ff-138">Number of Devices that have successfully installed this app.</span></span>|
|<span data-ttu-id="d64ff-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-139">failedDeviceCount</span></span>|<span data-ttu-id="d64ff-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-140">Int32</span></span>|<span data-ttu-id="d64ff-141">未能安装此应用的设备数。</span><span class="sxs-lookup"><span data-stu-id="d64ff-141">Number of Devices that have failed to install this app.</span></span>|
|<span data-ttu-id="d64ff-142">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-142">notApplicableDeviceCount</span></span>|<span data-ttu-id="d64ff-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-143">Int32</span></span>|<span data-ttu-id="d64ff-144">不适用于此应用的设备数。</span><span class="sxs-lookup"><span data-stu-id="d64ff-144">Number of Devices that are not applicable for this app.</span></span>|
|<span data-ttu-id="d64ff-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="d64ff-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-146">Int32</span></span>|<span data-ttu-id="d64ff-147">未安装此应用的设备数。</span><span class="sxs-lookup"><span data-stu-id="d64ff-147">Number of Devices that does not have this app installed.</span></span>|
|<span data-ttu-id="d64ff-148">pendingInstallDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-148">pendingInstallDeviceCount</span></span>|<span data-ttu-id="d64ff-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-149">Int32</span></span>|<span data-ttu-id="d64ff-150">已通知安装此应用的设备数。</span><span class="sxs-lookup"><span data-stu-id="d64ff-150">Number of Devices that have been notified to install this app.</span></span>|
|<span data-ttu-id="d64ff-151">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-151">installedUserCount</span></span>|<span data-ttu-id="d64ff-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-152">Int32</span></span>|<span data-ttu-id="d64ff-153">其设备全部成功安装此应用的用户数。</span><span class="sxs-lookup"><span data-stu-id="d64ff-153">Number of Users whose devices have all succeeded to install this app.</span></span>|
|<span data-ttu-id="d64ff-154">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-154">failedUserCount</span></span>|<span data-ttu-id="d64ff-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-155">Int32</span></span>|<span data-ttu-id="d64ff-156">拥有 1 台或多台设备未能安装此应用的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d64ff-156">Number of Users that have 1 or more device that failed to install this app.</span></span>|
|<span data-ttu-id="d64ff-157">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-157">notApplicableUserCount</span></span>|<span data-ttu-id="d64ff-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-158">Int32</span></span>|<span data-ttu-id="d64ff-159">其设备均不适用于此应用的用户数。</span><span class="sxs-lookup"><span data-stu-id="d64ff-159">Number of Users whose devices were all not applicable for this app.</span></span>|
|<span data-ttu-id="d64ff-160">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-160">notInstalledUserCount</span></span>|<span data-ttu-id="d64ff-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-161">Int32</span></span>|<span data-ttu-id="d64ff-162">具有 1 台或多台设备未安装此应用的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d64ff-162">Number of Users that have 1 or more devices that did not install this app.</span></span>|
|<span data-ttu-id="d64ff-163">pendingInstallUserCount</span><span class="sxs-lookup"><span data-stu-id="d64ff-163">pendingInstallUserCount</span></span>|<span data-ttu-id="d64ff-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d64ff-164">Int32</span></span>|<span data-ttu-id="d64ff-165">拥有 1 台或多台设备且已收到通知安装此应用且设备有 0 台失败的用户数。</span><span class="sxs-lookup"><span data-stu-id="d64ff-165">Number of Users that have 1 or more device that have been notified to install this app and have 0 devices with failures.</span></span>|



## <a name="response"></a><span data-ttu-id="d64ff-166">响应</span><span class="sxs-lookup"><span data-stu-id="d64ff-166">Response</span></span>
<span data-ttu-id="d64ff-167">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d64ff-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d64ff-168">示例</span><span class="sxs-lookup"><span data-stu-id="d64ff-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="d64ff-169">请求</span><span class="sxs-lookup"><span data-stu-id="d64ff-169">Request</span></span>
<span data-ttu-id="d64ff-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d64ff-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d64ff-171">响应</span><span class="sxs-lookup"><span data-stu-id="d64ff-171">Response</span></span>
<span data-ttu-id="d64ff-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d64ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




