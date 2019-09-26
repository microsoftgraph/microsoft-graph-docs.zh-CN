---
title: 创建 mobileAppInstallStatus
description: 创建新的 mobileAppInstallStatus 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1e50bedbf47296552251a3b23314233572b496a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37172574"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="d0dd8-103">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="d0dd8-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="d0dd8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0dd8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0dd8-106">创建新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-106">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0dd8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0dd8-107">Prerequisites</span></span>
<span data-ttu-id="d0dd8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0dd8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0dd8-110">Permission type</span></span>|<span data-ttu-id="d0dd8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d0dd8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0dd8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0dd8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0dd8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0dd8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d0dd8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0dd8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0dd8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-115">Not supported.</span></span>|
|<span data-ttu-id="d0dd8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0dd8-116">Application</span></span>|<span data-ttu-id="d0dd8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0dd8-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0dd8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0dd8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="d0dd8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0dd8-119">Request headers</span></span>
|<span data-ttu-id="d0dd8-120">标头</span><span class="sxs-lookup"><span data-stu-id="d0dd8-120">Header</span></span>|<span data-ttu-id="d0dd8-121">值</span><span class="sxs-lookup"><span data-stu-id="d0dd8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0dd8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0dd8-122">Authorization</span></span>|<span data-ttu-id="d0dd8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0dd8-124">接受</span><span class="sxs-lookup"><span data-stu-id="d0dd8-124">Accept</span></span>|<span data-ttu-id="d0dd8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0dd8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0dd8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0dd8-126">Request body</span></span>
<span data-ttu-id="d0dd8-127">在请求正文中，提供 mobileAppInstallStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-127">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="d0dd8-128">下表显示创建 mobileAppInstallStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-128">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="d0dd8-129">属性</span><span class="sxs-lookup"><span data-stu-id="d0dd8-129">Property</span></span>|<span data-ttu-id="d0dd8-130">类型</span><span class="sxs-lookup"><span data-stu-id="d0dd8-130">Type</span></span>|<span data-ttu-id="d0dd8-131">说明</span><span class="sxs-lookup"><span data-stu-id="d0dd8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0dd8-132">id</span><span class="sxs-lookup"><span data-stu-id="d0dd8-132">id</span></span>|<span data-ttu-id="d0dd8-133">String</span><span class="sxs-lookup"><span data-stu-id="d0dd8-133">String</span></span>|<span data-ttu-id="d0dd8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-134">Key of the entity.</span></span>|
|<span data-ttu-id="d0dd8-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="d0dd8-135">deviceName</span></span>|<span data-ttu-id="d0dd8-136">String</span><span class="sxs-lookup"><span data-stu-id="d0dd8-136">String</span></span>|<span data-ttu-id="d0dd8-137">设备名称</span><span class="sxs-lookup"><span data-stu-id="d0dd8-137">Device name</span></span>|
|<span data-ttu-id="d0dd8-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="d0dd8-138">deviceId</span></span>|<span data-ttu-id="d0dd8-139">String</span><span class="sxs-lookup"><span data-stu-id="d0dd8-139">String</span></span>|<span data-ttu-id="d0dd8-140">设备 ID</span><span class="sxs-lookup"><span data-stu-id="d0dd8-140">Device ID</span></span>|
|<span data-ttu-id="d0dd8-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d0dd8-141">lastSyncDateTime</span></span>|<span data-ttu-id="d0dd8-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0dd8-142">DateTimeOffset</span></span>|<span data-ttu-id="d0dd8-143">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="d0dd8-143">Last sync date time</span></span>|
|<span data-ttu-id="d0dd8-144">将 mobileappinstallstatusvalue</span><span class="sxs-lookup"><span data-stu-id="d0dd8-144">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="d0dd8-145">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d0dd8-145">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d0dd8-146">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-146">The install state of the app.</span></span> <span data-ttu-id="d0dd8-147">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-147">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d0dd8-148">installState</span><span class="sxs-lookup"><span data-stu-id="d0dd8-148">installState</span></span>|[<span data-ttu-id="d0dd8-149">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="d0dd8-149">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="d0dd8-150">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-150">The install state of the app.</span></span> <span data-ttu-id="d0dd8-151">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-151">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="d0dd8-152">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="d0dd8-152">installStateDetail</span></span>|[<span data-ttu-id="d0dd8-153">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="d0dd8-153">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="d0dd8-154">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-154">The install state detail of the app.</span></span> <span data-ttu-id="d0dd8-155">可能的值为`noAdditionalDetails`： `dependencyFailedToInstall`、 `dependencyWithRequirementsNotMet`、 `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `seeInstallErrorCode` `autoInstallDisabled` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet`、、、、、、、、、、、、、、、、 `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span><span class="sxs-lookup"><span data-stu-id="d0dd8-155">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="d0dd8-156">errorCode</span><span class="sxs-lookup"><span data-stu-id="d0dd8-156">errorCode</span></span>|<span data-ttu-id="d0dd8-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d0dd8-157">Int32</span></span>|<span data-ttu-id="d0dd8-158">安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-158">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="d0dd8-159">osVersion</span><span class="sxs-lookup"><span data-stu-id="d0dd8-159">osVersion</span></span>|<span data-ttu-id="d0dd8-160">String</span><span class="sxs-lookup"><span data-stu-id="d0dd8-160">String</span></span>|<span data-ttu-id="d0dd8-161">OS 版本</span><span class="sxs-lookup"><span data-stu-id="d0dd8-161">OS Version</span></span>|
|<span data-ttu-id="d0dd8-162">osDescription</span><span class="sxs-lookup"><span data-stu-id="d0dd8-162">osDescription</span></span>|<span data-ttu-id="d0dd8-163">String</span><span class="sxs-lookup"><span data-stu-id="d0dd8-163">String</span></span>|<span data-ttu-id="d0dd8-164">OS 说明</span><span class="sxs-lookup"><span data-stu-id="d0dd8-164">OS Description</span></span>|
|<span data-ttu-id="d0dd8-165">userName</span><span class="sxs-lookup"><span data-stu-id="d0dd8-165">userName</span></span>|<span data-ttu-id="d0dd8-166">String</span><span class="sxs-lookup"><span data-stu-id="d0dd8-166">String</span></span>|<span data-ttu-id="d0dd8-167">设备用户名</span><span class="sxs-lookup"><span data-stu-id="d0dd8-167">Device User Name</span></span>|
|<span data-ttu-id="d0dd8-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0dd8-168">userPrincipalName</span></span>|<span data-ttu-id="d0dd8-169">String</span><span class="sxs-lookup"><span data-stu-id="d0dd8-169">String</span></span>|<span data-ttu-id="d0dd8-170">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d0dd8-170">User Principal Name</span></span>|
|<span data-ttu-id="d0dd8-171">displayVersion</span><span class="sxs-lookup"><span data-stu-id="d0dd8-171">displayVersion</span></span>|<span data-ttu-id="d0dd8-172">String</span><span class="sxs-lookup"><span data-stu-id="d0dd8-172">String</span></span>|<span data-ttu-id="d0dd8-173">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="d0dd8-173">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="d0dd8-174">响应</span><span class="sxs-lookup"><span data-stu-id="d0dd8-174">Response</span></span>
<span data-ttu-id="d0dd8-175">如果成功，此方法在响应`201 Created`正文中返回响应代码和[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-175">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0dd8-176">示例</span><span class="sxs-lookup"><span data-stu-id="d0dd8-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0dd8-177">请求</span><span class="sxs-lookup"><span data-stu-id="d0dd8-177">Request</span></span>
<span data-ttu-id="d0dd8-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="d0dd8-179">响应</span><span class="sxs-lookup"><span data-stu-id="d0dd8-179">Response</span></span>
<span data-ttu-id="d0dd8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0dd8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




