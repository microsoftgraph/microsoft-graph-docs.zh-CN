---
title: 创建 mobileAppInstallStatus
description: 创建新的 mobileAppInstallStatus 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 123a07d7b7576bfc94011e20d45a6d0c8e65abc0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394192"
---
# <a name="create-mobileappinstallstatus"></a><span data-ttu-id="0ee0e-103">创建 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="0ee0e-103">Create mobileAppInstallStatus</span></span>

> <span data-ttu-id="0ee0e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ee0e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ee0e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee0e-107">创建新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-107">Create a new [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ee0e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ee0e-108">Prerequisites</span></span>
<span data-ttu-id="0ee0e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ee0e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ee0e-111">Permission type</span></span>|<span data-ttu-id="0ee0e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ee0e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ee0e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ee0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ee0e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ee0e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0ee0e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ee0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ee0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-116">Not supported.</span></span>|
|<span data-ttu-id="0ee0e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ee0e-117">Application</span></span>|<span data-ttu-id="0ee0e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ee0e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ee0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0ee0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ee0e-120">Request headers</span></span>
|<span data-ttu-id="0ee0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="0ee0e-121">Header</span></span>|<span data-ttu-id="0ee0e-122">值</span><span class="sxs-lookup"><span data-stu-id="0ee0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ee0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ee0e-123">Authorization</span></span>|<span data-ttu-id="0ee0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ee0e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ee0e-125">Accept</span></span>|<span data-ttu-id="0ee0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ee0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ee0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ee0e-127">Request body</span></span>
<span data-ttu-id="0ee0e-128">在请求正文中，提供 mobileAppInstallStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-128">In the request body, supply a JSON representation for the mobileAppInstallStatus object.</span></span>

<span data-ttu-id="0ee0e-129">下表显示时创建 mobileAppInstallStatus 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-129">The following table shows the properties that are required when you create the mobileAppInstallStatus.</span></span>

|<span data-ttu-id="0ee0e-130">属性</span><span class="sxs-lookup"><span data-stu-id="0ee0e-130">Property</span></span>|<span data-ttu-id="0ee0e-131">类型</span><span class="sxs-lookup"><span data-stu-id="0ee0e-131">Type</span></span>|<span data-ttu-id="0ee0e-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ee0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee0e-133">id</span><span class="sxs-lookup"><span data-stu-id="0ee0e-133">id</span></span>|<span data-ttu-id="0ee0e-134">String</span><span class="sxs-lookup"><span data-stu-id="0ee0e-134">String</span></span>|<span data-ttu-id="0ee0e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-135">Key of the entity.</span></span>|
|<span data-ttu-id="0ee0e-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="0ee0e-136">deviceName</span></span>|<span data-ttu-id="0ee0e-137">String</span><span class="sxs-lookup"><span data-stu-id="0ee0e-137">String</span></span>|<span data-ttu-id="0ee0e-138">设备名称</span><span class="sxs-lookup"><span data-stu-id="0ee0e-138">Device name</span></span>|
|<span data-ttu-id="0ee0e-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="0ee0e-139">deviceId</span></span>|<span data-ttu-id="0ee0e-140">String</span><span class="sxs-lookup"><span data-stu-id="0ee0e-140">String</span></span>|<span data-ttu-id="0ee0e-141">设备 ID</span><span class="sxs-lookup"><span data-stu-id="0ee0e-141">Device ID</span></span>|
|<span data-ttu-id="0ee0e-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0ee0e-142">lastSyncDateTime</span></span>|<span data-ttu-id="0ee0e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ee0e-143">DateTimeOffset</span></span>|<span data-ttu-id="0ee0e-144">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="0ee0e-144">Last sync date time</span></span>|
|<span data-ttu-id="0ee0e-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="0ee0e-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="0ee0e-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="0ee0e-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="0ee0e-147">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-147">The install state of the app.</span></span> <span data-ttu-id="0ee0e-148">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="0ee0e-149">installState</span><span class="sxs-lookup"><span data-stu-id="0ee0e-149">installState</span></span>|[<span data-ttu-id="0ee0e-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="0ee0e-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="0ee0e-151">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-151">The install state of the app.</span></span> <span data-ttu-id="0ee0e-152">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="0ee0e-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="0ee0e-153">installStateDetail</span></span>|[<span data-ttu-id="0ee0e-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="0ee0e-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="0ee0e-155">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-155">The install state detail of the app.</span></span> <span data-ttu-id="0ee0e-156">可取值为：`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="0ee0e-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="0ee0e-157">errorCode</span></span>|<span data-ttu-id="0ee0e-158">Int32</span><span class="sxs-lookup"><span data-stu-id="0ee0e-158">Int32</span></span>|<span data-ttu-id="0ee0e-159">错误代码用于安装或卸载失败。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="0ee0e-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="0ee0e-160">osVersion</span></span>|<span data-ttu-id="0ee0e-161">String</span><span class="sxs-lookup"><span data-stu-id="0ee0e-161">String</span></span>|<span data-ttu-id="0ee0e-162">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="0ee0e-162">OS Version</span></span>|
|<span data-ttu-id="0ee0e-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="0ee0e-163">osDescription</span></span>|<span data-ttu-id="0ee0e-164">String</span><span class="sxs-lookup"><span data-stu-id="0ee0e-164">String</span></span>|<span data-ttu-id="0ee0e-165">操作系统说明</span><span class="sxs-lookup"><span data-stu-id="0ee0e-165">OS Description</span></span>|
|<span data-ttu-id="0ee0e-166">userName</span><span class="sxs-lookup"><span data-stu-id="0ee0e-166">userName</span></span>|<span data-ttu-id="0ee0e-167">String</span><span class="sxs-lookup"><span data-stu-id="0ee0e-167">String</span></span>|<span data-ttu-id="0ee0e-168">设备用户名</span><span class="sxs-lookup"><span data-stu-id="0ee0e-168">Device User Name</span></span>|
|<span data-ttu-id="0ee0e-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0ee0e-169">userPrincipalName</span></span>|<span data-ttu-id="0ee0e-170">String</span><span class="sxs-lookup"><span data-stu-id="0ee0e-170">String</span></span>|<span data-ttu-id="0ee0e-171">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="0ee0e-171">User Principal Name</span></span>|
|<span data-ttu-id="0ee0e-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="0ee0e-172">displayVersion</span></span>|<span data-ttu-id="0ee0e-173">String</span><span class="sxs-lookup"><span data-stu-id="0ee0e-173">String</span></span>|<span data-ttu-id="0ee0e-174">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="0ee0e-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="0ee0e-175">响应</span><span class="sxs-lookup"><span data-stu-id="0ee0e-175">Response</span></span>
<span data-ttu-id="0ee0e-176">如果成功，此方法返回`201 Created`响应代码和响应正文中的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-176">If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ee0e-177">示例</span><span class="sxs-lookup"><span data-stu-id="0ee0e-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ee0e-178">请求</span><span class="sxs-lookup"><span data-stu-id="0ee0e-178">Request</span></span>
<span data-ttu-id="0ee0e-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="0ee0e-180">响应</span><span class="sxs-lookup"><span data-stu-id="0ee0e-180">Response</span></span>
<span data-ttu-id="0ee0e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ee0e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




