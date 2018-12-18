---
title: 更新 mobileAppInstallStatus
description: 更新 mobileAppInstallStatus 对象的属性。
author: tfitzmac
ms.openlocfilehash: dbf65aa07258b48a8ce64cf01db0a5ef00097f3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336321"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="374e0-103">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="374e0-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="374e0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="374e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="374e0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="374e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="374e0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="374e0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="374e0-107">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="374e0-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="374e0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="374e0-108">Prerequisites</span></span>
<span data-ttu-id="374e0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="374e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="374e0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="374e0-111">Permission type</span></span>|<span data-ttu-id="374e0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="374e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="374e0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="374e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="374e0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="374e0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="374e0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="374e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="374e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="374e0-116">Not supported.</span></span>|
|<span data-ttu-id="374e0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="374e0-117">Application</span></span>|<span data-ttu-id="374e0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="374e0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="374e0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="374e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="374e0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="374e0-120">Request headers</span></span>
|<span data-ttu-id="374e0-121">标头</span><span class="sxs-lookup"><span data-stu-id="374e0-121">Header</span></span>|<span data-ttu-id="374e0-122">值</span><span class="sxs-lookup"><span data-stu-id="374e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="374e0-123">授权</span><span class="sxs-lookup"><span data-stu-id="374e0-123">Authorization</span></span>|<span data-ttu-id="374e0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="374e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="374e0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="374e0-125">Accept</span></span>|<span data-ttu-id="374e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="374e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="374e0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="374e0-127">Request body</span></span>
<span data-ttu-id="374e0-128">在请求正文中，提供[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="374e0-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="374e0-129">下表显示时创建[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="374e0-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="374e0-130">属性</span><span class="sxs-lookup"><span data-stu-id="374e0-130">Property</span></span>|<span data-ttu-id="374e0-131">类型</span><span class="sxs-lookup"><span data-stu-id="374e0-131">Type</span></span>|<span data-ttu-id="374e0-132">说明</span><span class="sxs-lookup"><span data-stu-id="374e0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="374e0-133">id</span><span class="sxs-lookup"><span data-stu-id="374e0-133">id</span></span>|<span data-ttu-id="374e0-134">String</span><span class="sxs-lookup"><span data-stu-id="374e0-134">String</span></span>|<span data-ttu-id="374e0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="374e0-135">Key of the entity.</span></span>|
|<span data-ttu-id="374e0-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="374e0-136">deviceName</span></span>|<span data-ttu-id="374e0-137">String</span><span class="sxs-lookup"><span data-stu-id="374e0-137">String</span></span>|<span data-ttu-id="374e0-138">设备名称</span><span class="sxs-lookup"><span data-stu-id="374e0-138">Device name</span></span>|
|<span data-ttu-id="374e0-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="374e0-139">deviceId</span></span>|<span data-ttu-id="374e0-140">String</span><span class="sxs-lookup"><span data-stu-id="374e0-140">String</span></span>|<span data-ttu-id="374e0-141">设备 ID</span><span class="sxs-lookup"><span data-stu-id="374e0-141">Device ID</span></span>|
|<span data-ttu-id="374e0-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="374e0-142">lastSyncDateTime</span></span>|<span data-ttu-id="374e0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="374e0-143">DateTimeOffset</span></span>|<span data-ttu-id="374e0-144">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="374e0-144">Last sync date time</span></span>|
|<span data-ttu-id="374e0-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="374e0-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="374e0-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="374e0-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="374e0-147">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="374e0-147">The install state of the app.</span></span> <span data-ttu-id="374e0-148">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="374e0-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="374e0-149">installState</span><span class="sxs-lookup"><span data-stu-id="374e0-149">installState</span></span>|[<span data-ttu-id="374e0-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="374e0-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="374e0-151">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="374e0-151">The install state of the app.</span></span> <span data-ttu-id="374e0-152">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="374e0-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="374e0-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="374e0-153">installStateDetail</span></span>|[<span data-ttu-id="374e0-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="374e0-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="374e0-155">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="374e0-155">The install state detail of the app.</span></span> <span data-ttu-id="374e0-156">可取值为：`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="374e0-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="374e0-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="374e0-157">errorCode</span></span>|<span data-ttu-id="374e0-158">Int32</span><span class="sxs-lookup"><span data-stu-id="374e0-158">Int32</span></span>|<span data-ttu-id="374e0-159">错误代码用于安装或卸载失败。</span><span class="sxs-lookup"><span data-stu-id="374e0-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="374e0-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="374e0-160">osVersion</span></span>|<span data-ttu-id="374e0-161">String</span><span class="sxs-lookup"><span data-stu-id="374e0-161">String</span></span>|<span data-ttu-id="374e0-162">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="374e0-162">OS Version</span></span>|
|<span data-ttu-id="374e0-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="374e0-163">osDescription</span></span>|<span data-ttu-id="374e0-164">String</span><span class="sxs-lookup"><span data-stu-id="374e0-164">String</span></span>|<span data-ttu-id="374e0-165">操作系统说明</span><span class="sxs-lookup"><span data-stu-id="374e0-165">OS Description</span></span>|
|<span data-ttu-id="374e0-166">userName</span><span class="sxs-lookup"><span data-stu-id="374e0-166">userName</span></span>|<span data-ttu-id="374e0-167">String</span><span class="sxs-lookup"><span data-stu-id="374e0-167">String</span></span>|<span data-ttu-id="374e0-168">设备用户名</span><span class="sxs-lookup"><span data-stu-id="374e0-168">Device User Name</span></span>|
|<span data-ttu-id="374e0-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="374e0-169">userPrincipalName</span></span>|<span data-ttu-id="374e0-170">字符串</span><span class="sxs-lookup"><span data-stu-id="374e0-170">String</span></span>|<span data-ttu-id="374e0-171">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="374e0-171">User Principal Name</span></span>|
|<span data-ttu-id="374e0-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="374e0-172">displayVersion</span></span>|<span data-ttu-id="374e0-173">字符串</span><span class="sxs-lookup"><span data-stu-id="374e0-173">String</span></span>|<span data-ttu-id="374e0-174">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="374e0-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="374e0-175">响应</span><span class="sxs-lookup"><span data-stu-id="374e0-175">Response</span></span>
<span data-ttu-id="374e0-176">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="374e0-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="374e0-177">示例</span><span class="sxs-lookup"><span data-stu-id="374e0-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="374e0-178">请求</span><span class="sxs-lookup"><span data-stu-id="374e0-178">Request</span></span>
<span data-ttu-id="374e0-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="374e0-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
Content-type: application/json
Content-length: 488

{
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

### <a name="response"></a><span data-ttu-id="374e0-180">响应</span><span class="sxs-lookup"><span data-stu-id="374e0-180">Response</span></span>
<span data-ttu-id="374e0-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="374e0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





