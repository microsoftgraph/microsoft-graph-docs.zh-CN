---
title: 更新 mobileAppInstallStatus
description: 更新 mobileAppInstallStatus 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4c10190f7cc675b5444a6238060703b852d44b4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973752"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="52726-103">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="52726-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="52726-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="52726-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52726-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="52726-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52726-106">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="52726-106">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52726-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="52726-107">Prerequisites</span></span>
<span data-ttu-id="52726-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52726-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52726-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="52726-110">Permission type</span></span>|<span data-ttu-id="52726-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="52726-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52726-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52726-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52726-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52726-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52726-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52726-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52726-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="52726-115">Not supported.</span></span>|
|<span data-ttu-id="52726-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="52726-116">Application</span></span>|<span data-ttu-id="52726-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="52726-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52726-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52726-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="52726-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="52726-119">Request headers</span></span>
|<span data-ttu-id="52726-120">标头</span><span class="sxs-lookup"><span data-stu-id="52726-120">Header</span></span>|<span data-ttu-id="52726-121">值</span><span class="sxs-lookup"><span data-stu-id="52726-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52726-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52726-122">Authorization</span></span>|<span data-ttu-id="52726-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="52726-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52726-124">接受</span><span class="sxs-lookup"><span data-stu-id="52726-124">Accept</span></span>|<span data-ttu-id="52726-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52726-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52726-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="52726-126">Request body</span></span>
<span data-ttu-id="52726-127">在请求正文中, 提供[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52726-127">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="52726-128">下表显示创建[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="52726-128">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="52726-129">属性</span><span class="sxs-lookup"><span data-stu-id="52726-129">Property</span></span>|<span data-ttu-id="52726-130">类型</span><span class="sxs-lookup"><span data-stu-id="52726-130">Type</span></span>|<span data-ttu-id="52726-131">说明</span><span class="sxs-lookup"><span data-stu-id="52726-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52726-132">id</span><span class="sxs-lookup"><span data-stu-id="52726-132">id</span></span>|<span data-ttu-id="52726-133">String</span><span class="sxs-lookup"><span data-stu-id="52726-133">String</span></span>|<span data-ttu-id="52726-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="52726-134">Key of the entity.</span></span>|
|<span data-ttu-id="52726-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="52726-135">deviceName</span></span>|<span data-ttu-id="52726-136">String</span><span class="sxs-lookup"><span data-stu-id="52726-136">String</span></span>|<span data-ttu-id="52726-137">设备名称</span><span class="sxs-lookup"><span data-stu-id="52726-137">Device name</span></span>|
|<span data-ttu-id="52726-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="52726-138">deviceId</span></span>|<span data-ttu-id="52726-139">String</span><span class="sxs-lookup"><span data-stu-id="52726-139">String</span></span>|<span data-ttu-id="52726-140">设备 ID</span><span class="sxs-lookup"><span data-stu-id="52726-140">Device ID</span></span>|
|<span data-ttu-id="52726-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="52726-141">lastSyncDateTime</span></span>|<span data-ttu-id="52726-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52726-142">DateTimeOffset</span></span>|<span data-ttu-id="52726-143">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="52726-143">Last sync date time</span></span>|
|<span data-ttu-id="52726-144">将 mobileappinstallstatusvalue</span><span class="sxs-lookup"><span data-stu-id="52726-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="52726-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="52726-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="52726-146">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="52726-146">The install state of the app.</span></span> <span data-ttu-id="52726-147">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="52726-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="52726-148">installState</span><span class="sxs-lookup"><span data-stu-id="52726-148">installState</span></span>|[<span data-ttu-id="52726-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="52726-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="52726-150">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="52726-150">The install state of the app.</span></span> <span data-ttu-id="52726-151">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="52726-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="52726-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="52726-152">installStateDetail</span></span>|[<span data-ttu-id="52726-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="52726-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="52726-154">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="52726-154">The install state detail of the app.</span></span> <span data-ttu-id="52726-155">可能的值为`noAdditionalDetails`: `dependencyFailedToInstall`、 `dependencyWithRequirementsNotMet`、 `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`、、、、、、、、、、、、、、、、 `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="52726-155">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="52726-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="52726-156">errorCode</span></span>|<span data-ttu-id="52726-157">Int32</span><span class="sxs-lookup"><span data-stu-id="52726-157">Int32</span></span>|<span data-ttu-id="52726-158">安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="52726-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="52726-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="52726-159">osVersion</span></span>|<span data-ttu-id="52726-160">String</span><span class="sxs-lookup"><span data-stu-id="52726-160">String</span></span>|<span data-ttu-id="52726-161">OS 版本</span><span class="sxs-lookup"><span data-stu-id="52726-161">OS Version</span></span>|
|<span data-ttu-id="52726-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="52726-162">osDescription</span></span>|<span data-ttu-id="52726-163">String</span><span class="sxs-lookup"><span data-stu-id="52726-163">String</span></span>|<span data-ttu-id="52726-164">OS 说明</span><span class="sxs-lookup"><span data-stu-id="52726-164">OS Description</span></span>|
|<span data-ttu-id="52726-165">userName</span><span class="sxs-lookup"><span data-stu-id="52726-165">userName</span></span>|<span data-ttu-id="52726-166">String</span><span class="sxs-lookup"><span data-stu-id="52726-166">String</span></span>|<span data-ttu-id="52726-167">设备用户名</span><span class="sxs-lookup"><span data-stu-id="52726-167">Device User Name</span></span>|
|<span data-ttu-id="52726-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="52726-168">userPrincipalName</span></span>|<span data-ttu-id="52726-169">String</span><span class="sxs-lookup"><span data-stu-id="52726-169">String</span></span>|<span data-ttu-id="52726-170">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="52726-170">User Principal Name</span></span>|
|<span data-ttu-id="52726-171">displayVersion</span><span class="sxs-lookup"><span data-stu-id="52726-171">displayVersion</span></span>|<span data-ttu-id="52726-172">String</span><span class="sxs-lookup"><span data-stu-id="52726-172">String</span></span>|<span data-ttu-id="52726-173">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="52726-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="52726-174">响应</span><span class="sxs-lookup"><span data-stu-id="52726-174">Response</span></span>
<span data-ttu-id="52726-175">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="52726-175">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52726-176">示例</span><span class="sxs-lookup"><span data-stu-id="52726-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="52726-177">请求</span><span class="sxs-lookup"><span data-stu-id="52726-177">Request</span></span>
<span data-ttu-id="52726-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="52726-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "dependencyFailedToInstall",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### <a name="response"></a><span data-ttu-id="52726-179">响应</span><span class="sxs-lookup"><span data-stu-id="52726-179">Response</span></span>
<span data-ttu-id="52726-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="52726-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 604

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "7560ee45-ee45-7560-45ee-607545ee6075",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "mobileAppInstallStatusValue": "failed",
  "installState": "failed",
  "installStateDetail": "dependencyFailedToInstall",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```





