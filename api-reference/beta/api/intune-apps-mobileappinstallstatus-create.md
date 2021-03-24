---
title: 创建 mobileAppInstallStatus
description: 创建新的 mobileAppInstallStatus 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0c6f07e12240325b1f01dddf857268399026cb1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143169"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="080d3-103">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="080d3-103">Create mobileAppInstallStatus</span></span>

<span data-ttu-id="080d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="080d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="080d3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="080d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="080d3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="080d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="080d3-107">创建新的 [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="080d3-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="080d3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="080d3-108">Prerequisites</span></span>
<span data-ttu-id="080d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="080d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="080d3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="080d3-111">Permission type</span></span>|<span data-ttu-id="080d3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="080d3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="080d3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="080d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="080d3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="080d3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="080d3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="080d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="080d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="080d3-116">Not supported.</span></span>|
|<span data-ttu-id="080d3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="080d3-117">Application</span></span>|<span data-ttu-id="080d3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="080d3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="080d3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="080d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="080d3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="080d3-120">Request headers</span></span>
|<span data-ttu-id="080d3-121">标头</span><span class="sxs-lookup"><span data-stu-id="080d3-121">Header</span></span>|<span data-ttu-id="080d3-122">值</span><span class="sxs-lookup"><span data-stu-id="080d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="080d3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="080d3-123">Authorization</span></span>|<span data-ttu-id="080d3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="080d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="080d3-125">接受</span><span class="sxs-lookup"><span data-stu-id="080d3-125">Accept</span></span>|<span data-ttu-id="080d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="080d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="080d3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="080d3-127">Request body</span></span>
<span data-ttu-id="080d3-128">在请求正文中，提供 mobileAppInstallStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="080d3-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="080d3-129">下表显示创建 mobileAppInstallStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="080d3-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="080d3-130">属性</span><span class="sxs-lookup"><span data-stu-id="080d3-130">Property</span></span>|<span data-ttu-id="080d3-131">类型</span><span class="sxs-lookup"><span data-stu-id="080d3-131">Type</span></span>|<span data-ttu-id="080d3-132">说明</span><span class="sxs-lookup"><span data-stu-id="080d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="080d3-133">id</span><span class="sxs-lookup"><span data-stu-id="080d3-133">id</span></span>|<span data-ttu-id="080d3-134">String</span><span class="sxs-lookup"><span data-stu-id="080d3-134">String</span></span>|<span data-ttu-id="080d3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="080d3-135">Key of the entity.</span></span>|
|<span data-ttu-id="080d3-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="080d3-136">deviceName</span></span>|<span data-ttu-id="080d3-137">String</span><span class="sxs-lookup"><span data-stu-id="080d3-137">String</span></span>|<span data-ttu-id="080d3-138">设备名称</span><span class="sxs-lookup"><span data-stu-id="080d3-138">Device name</span></span>|
|<span data-ttu-id="080d3-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="080d3-139">deviceId</span></span>|<span data-ttu-id="080d3-140">String</span><span class="sxs-lookup"><span data-stu-id="080d3-140">String</span></span>|<span data-ttu-id="080d3-141">设备 ID</span><span class="sxs-lookup"><span data-stu-id="080d3-141">Device ID</span></span>|
|<span data-ttu-id="080d3-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="080d3-142">lastSyncDateTime</span></span>|<span data-ttu-id="080d3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="080d3-143">DateTimeOffset</span></span>|<span data-ttu-id="080d3-144">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="080d3-144">Last sync date time</span></span>|
|<span data-ttu-id="080d3-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="080d3-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="080d3-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="080d3-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="080d3-147">应用的安装状态。</span><span class="sxs-lookup"><span data-stu-id="080d3-147">The install state of the app.</span></span> <span data-ttu-id="080d3-148">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="080d3-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="080d3-149">installState</span><span class="sxs-lookup"><span data-stu-id="080d3-149">installState</span></span>|[<span data-ttu-id="080d3-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="080d3-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="080d3-151">应用的安装状态。</span><span class="sxs-lookup"><span data-stu-id="080d3-151">The install state of the app.</span></span> <span data-ttu-id="080d3-152">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="080d3-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="080d3-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="080d3-153">installStateDetail</span></span>|[<span data-ttu-id="080d3-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="080d3-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="080d3-155">应用的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="080d3-155">The install state detail of the app.</span></span> <span data-ttu-id="080d3-156">可能的值是 `noAdditionalDetails` `dependencyFailedToInstall` `dependencyWithRequirementsNotMet` ：、、、、、、、、、、 `dependencyPendingReboot` `dependencyWithAutoInstallDisabled` `iosAppStoreUpdateFailedToInstall` `vppAppHasUpdateAvailable` `userRejectedUpdate` `seeInstallErrorCode` `autoInstallDisabled` `managedAppNoLongerPresent` `userRejectedInstall` `userIsNotLoggedIntoAppStore` `seeUninstallErrorCode` `pendingReboot` `installingDependencies` `contentDownloaded` `powerShellScriptRequirementNotMet` `registryRequirementNotMet` `fileSystemRequirementNotMet` `platformNotApplicable` `minimumCpuSpeedNotMet` `minimumLogicalProcessorCountNotMet` `minimumPhysicalMemoryNotMet` `minimumOsVersionNotMet` `minimumDiskSpaceNotMet` `processorArchitectureNotApplicable` 、</span><span class="sxs-lookup"><span data-stu-id="080d3-156">Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `iosAppStoreUpdateFailedToInstall`, `vppAppHasUpdateAvailable`, `userRejectedUpdate`, `seeInstallErrorCode`, `autoInstallDisabled`, `managedAppNoLongerPresent`, `userRejectedInstall`, `userIsNotLoggedIntoAppStore`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="080d3-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="080d3-157">errorCode</span></span>|<span data-ttu-id="080d3-158">Int32</span><span class="sxs-lookup"><span data-stu-id="080d3-158">Int32</span></span>|<span data-ttu-id="080d3-159">安装或卸载失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="080d3-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="080d3-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="080d3-160">osVersion</span></span>|<span data-ttu-id="080d3-161">String</span><span class="sxs-lookup"><span data-stu-id="080d3-161">String</span></span>|<span data-ttu-id="080d3-162">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="080d3-162">OS Version</span></span>|
|<span data-ttu-id="080d3-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="080d3-163">osDescription</span></span>|<span data-ttu-id="080d3-164">String</span><span class="sxs-lookup"><span data-stu-id="080d3-164">String</span></span>|<span data-ttu-id="080d3-165">操作系统说明</span><span class="sxs-lookup"><span data-stu-id="080d3-165">OS Description</span></span>|
|<span data-ttu-id="080d3-166">userName</span><span class="sxs-lookup"><span data-stu-id="080d3-166">userName</span></span>|<span data-ttu-id="080d3-167">String</span><span class="sxs-lookup"><span data-stu-id="080d3-167">String</span></span>|<span data-ttu-id="080d3-168">设备用户名</span><span class="sxs-lookup"><span data-stu-id="080d3-168">Device User Name</span></span>|
|<span data-ttu-id="080d3-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="080d3-169">userPrincipalName</span></span>|<span data-ttu-id="080d3-170">String</span><span class="sxs-lookup"><span data-stu-id="080d3-170">String</span></span>|<span data-ttu-id="080d3-171">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="080d3-171">User Principal Name</span></span>|
|<span data-ttu-id="080d3-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="080d3-172">displayVersion</span></span>|<span data-ttu-id="080d3-173">String</span><span class="sxs-lookup"><span data-stu-id="080d3-173">String</span></span>|<span data-ttu-id="080d3-174">应用程序的可读人工版本</span><span class="sxs-lookup"><span data-stu-id="080d3-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="080d3-175">响应</span><span class="sxs-lookup"><span data-stu-id="080d3-175">Response</span></span>
<span data-ttu-id="080d3-176">如果成功，此方法在响应 `201 Created` 正文中返回 响应 [代码和 mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="080d3-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="080d3-177">示例</span><span class="sxs-lookup"><span data-stu-id="080d3-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="080d3-178">请求</span><span class="sxs-lookup"><span data-stu-id="080d3-178">Request</span></span>
<span data-ttu-id="080d3-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="080d3-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="080d3-180">响应</span><span class="sxs-lookup"><span data-stu-id="080d3-180">Response</span></span>
<span data-ttu-id="080d3-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="080d3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




