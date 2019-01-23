---
title: 更新 mobileAppInstallStatus
description: 更新 mobileAppInstallStatus 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e28404181248cef1deae4bec2752de51f553373b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394542"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="a8d59-103">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="a8d59-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="a8d59-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a8d59-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8d59-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8d59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8d59-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8d59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8d59-107">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a8d59-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8d59-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8d59-108">Prerequisites</span></span>
<span data-ttu-id="a8d59-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a8d59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a8d59-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8d59-111">Permission type</span></span>|<span data-ttu-id="a8d59-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a8d59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8d59-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8d59-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8d59-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8d59-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8d59-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8d59-116">Not supported.</span></span>|
|<span data-ttu-id="a8d59-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8d59-117">Application</span></span>|<span data-ttu-id="a8d59-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8d59-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8d59-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8d59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="a8d59-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8d59-120">Request headers</span></span>
|<span data-ttu-id="a8d59-121">标头</span><span class="sxs-lookup"><span data-stu-id="a8d59-121">Header</span></span>|<span data-ttu-id="a8d59-122">值</span><span class="sxs-lookup"><span data-stu-id="a8d59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8d59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8d59-123">Authorization</span></span>|<span data-ttu-id="a8d59-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a8d59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8d59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8d59-125">Accept</span></span>|<span data-ttu-id="a8d59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8d59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8d59-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8d59-127">Request body</span></span>
<span data-ttu-id="a8d59-128">在请求正文中，提供[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8d59-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="a8d59-129">下表显示时创建[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a8d59-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="a8d59-130">属性</span><span class="sxs-lookup"><span data-stu-id="a8d59-130">Property</span></span>|<span data-ttu-id="a8d59-131">类型</span><span class="sxs-lookup"><span data-stu-id="a8d59-131">Type</span></span>|<span data-ttu-id="a8d59-132">说明</span><span class="sxs-lookup"><span data-stu-id="a8d59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8d59-133">id</span><span class="sxs-lookup"><span data-stu-id="a8d59-133">id</span></span>|<span data-ttu-id="a8d59-134">String</span><span class="sxs-lookup"><span data-stu-id="a8d59-134">String</span></span>|<span data-ttu-id="a8d59-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a8d59-135">Key of the entity.</span></span>|
|<span data-ttu-id="a8d59-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="a8d59-136">deviceName</span></span>|<span data-ttu-id="a8d59-137">String</span><span class="sxs-lookup"><span data-stu-id="a8d59-137">String</span></span>|<span data-ttu-id="a8d59-138">设备名称</span><span class="sxs-lookup"><span data-stu-id="a8d59-138">Device name</span></span>|
|<span data-ttu-id="a8d59-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="a8d59-139">deviceId</span></span>|<span data-ttu-id="a8d59-140">String</span><span class="sxs-lookup"><span data-stu-id="a8d59-140">String</span></span>|<span data-ttu-id="a8d59-141">设备 ID</span><span class="sxs-lookup"><span data-stu-id="a8d59-141">Device ID</span></span>|
|<span data-ttu-id="a8d59-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a8d59-142">lastSyncDateTime</span></span>|<span data-ttu-id="a8d59-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8d59-143">DateTimeOffset</span></span>|<span data-ttu-id="a8d59-144">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="a8d59-144">Last sync date time</span></span>|
|<span data-ttu-id="a8d59-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="a8d59-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="a8d59-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="a8d59-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="a8d59-147">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="a8d59-147">The install state of the app.</span></span> <span data-ttu-id="a8d59-148">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="a8d59-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="a8d59-149">installState</span><span class="sxs-lookup"><span data-stu-id="a8d59-149">installState</span></span>|[<span data-ttu-id="a8d59-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="a8d59-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="a8d59-151">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="a8d59-151">The install state of the app.</span></span> <span data-ttu-id="a8d59-152">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="a8d59-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="a8d59-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="a8d59-153">installStateDetail</span></span>|[<span data-ttu-id="a8d59-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="a8d59-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="a8d59-155">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="a8d59-155">The install state detail of the app.</span></span> <span data-ttu-id="a8d59-156">可取值为：`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="a8d59-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="a8d59-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="a8d59-157">errorCode</span></span>|<span data-ttu-id="a8d59-158">Int32</span><span class="sxs-lookup"><span data-stu-id="a8d59-158">Int32</span></span>|<span data-ttu-id="a8d59-159">错误代码用于安装或卸载失败。</span><span class="sxs-lookup"><span data-stu-id="a8d59-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="a8d59-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="a8d59-160">osVersion</span></span>|<span data-ttu-id="a8d59-161">String</span><span class="sxs-lookup"><span data-stu-id="a8d59-161">String</span></span>|<span data-ttu-id="a8d59-162">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="a8d59-162">OS Version</span></span>|
|<span data-ttu-id="a8d59-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="a8d59-163">osDescription</span></span>|<span data-ttu-id="a8d59-164">String</span><span class="sxs-lookup"><span data-stu-id="a8d59-164">String</span></span>|<span data-ttu-id="a8d59-165">操作系统说明</span><span class="sxs-lookup"><span data-stu-id="a8d59-165">OS Description</span></span>|
|<span data-ttu-id="a8d59-166">userName</span><span class="sxs-lookup"><span data-stu-id="a8d59-166">userName</span></span>|<span data-ttu-id="a8d59-167">String</span><span class="sxs-lookup"><span data-stu-id="a8d59-167">String</span></span>|<span data-ttu-id="a8d59-168">设备用户名</span><span class="sxs-lookup"><span data-stu-id="a8d59-168">Device User Name</span></span>|
|<span data-ttu-id="a8d59-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a8d59-169">userPrincipalName</span></span>|<span data-ttu-id="a8d59-170">String</span><span class="sxs-lookup"><span data-stu-id="a8d59-170">String</span></span>|<span data-ttu-id="a8d59-171">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="a8d59-171">User Principal Name</span></span>|
|<span data-ttu-id="a8d59-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="a8d59-172">displayVersion</span></span>|<span data-ttu-id="a8d59-173">String</span><span class="sxs-lookup"><span data-stu-id="a8d59-173">String</span></span>|<span data-ttu-id="a8d59-174">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="a8d59-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="a8d59-175">响应</span><span class="sxs-lookup"><span data-stu-id="a8d59-175">Response</span></span>
<span data-ttu-id="a8d59-176">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a8d59-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8d59-177">示例</span><span class="sxs-lookup"><span data-stu-id="a8d59-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8d59-178">请求</span><span class="sxs-lookup"><span data-stu-id="a8d59-178">Request</span></span>
<span data-ttu-id="a8d59-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8d59-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="a8d59-180">响应</span><span class="sxs-lookup"><span data-stu-id="a8d59-180">Response</span></span>
<span data-ttu-id="a8d59-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8d59-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "seeInstallErrorCode",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```




