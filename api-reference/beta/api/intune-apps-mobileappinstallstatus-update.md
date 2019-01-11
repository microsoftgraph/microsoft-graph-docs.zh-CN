---
title: 更新 mobileAppInstallStatus
description: 更新 mobileAppInstallStatus 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a60bcf69ded37ea0b4a04430c6a837bb6df95100
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817946"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="465bf-103">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="465bf-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="465bf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="465bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="465bf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="465bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="465bf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="465bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="465bf-107">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="465bf-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="465bf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="465bf-108">Prerequisites</span></span>
<span data-ttu-id="465bf-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="465bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="465bf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="465bf-111">Permission type</span></span>|<span data-ttu-id="465bf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="465bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="465bf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="465bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="465bf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="465bf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="465bf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="465bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="465bf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="465bf-116">Not supported.</span></span>|
|<span data-ttu-id="465bf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="465bf-117">Application</span></span>|<span data-ttu-id="465bf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="465bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="465bf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="465bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="465bf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="465bf-120">Request headers</span></span>
|<span data-ttu-id="465bf-121">标头</span><span class="sxs-lookup"><span data-stu-id="465bf-121">Header</span></span>|<span data-ttu-id="465bf-122">值</span><span class="sxs-lookup"><span data-stu-id="465bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="465bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="465bf-123">Authorization</span></span>|<span data-ttu-id="465bf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="465bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="465bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="465bf-125">Accept</span></span>|<span data-ttu-id="465bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="465bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="465bf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="465bf-127">Request body</span></span>
<span data-ttu-id="465bf-128">在请求正文中，提供[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="465bf-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="465bf-129">下表显示时创建[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="465bf-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="465bf-130">属性</span><span class="sxs-lookup"><span data-stu-id="465bf-130">Property</span></span>|<span data-ttu-id="465bf-131">类型</span><span class="sxs-lookup"><span data-stu-id="465bf-131">Type</span></span>|<span data-ttu-id="465bf-132">说明</span><span class="sxs-lookup"><span data-stu-id="465bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="465bf-133">id</span><span class="sxs-lookup"><span data-stu-id="465bf-133">id</span></span>|<span data-ttu-id="465bf-134">String</span><span class="sxs-lookup"><span data-stu-id="465bf-134">String</span></span>|<span data-ttu-id="465bf-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="465bf-135">Key of the entity.</span></span>|
|<span data-ttu-id="465bf-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="465bf-136">deviceName</span></span>|<span data-ttu-id="465bf-137">String</span><span class="sxs-lookup"><span data-stu-id="465bf-137">String</span></span>|<span data-ttu-id="465bf-138">设备名称</span><span class="sxs-lookup"><span data-stu-id="465bf-138">Device name</span></span>|
|<span data-ttu-id="465bf-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="465bf-139">deviceId</span></span>|<span data-ttu-id="465bf-140">String</span><span class="sxs-lookup"><span data-stu-id="465bf-140">String</span></span>|<span data-ttu-id="465bf-141">设备 ID</span><span class="sxs-lookup"><span data-stu-id="465bf-141">Device ID</span></span>|
|<span data-ttu-id="465bf-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="465bf-142">lastSyncDateTime</span></span>|<span data-ttu-id="465bf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="465bf-143">DateTimeOffset</span></span>|<span data-ttu-id="465bf-144">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="465bf-144">Last sync date time</span></span>|
|<span data-ttu-id="465bf-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="465bf-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="465bf-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="465bf-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="465bf-147">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="465bf-147">The install state of the app.</span></span> <span data-ttu-id="465bf-148">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="465bf-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="465bf-149">installState</span><span class="sxs-lookup"><span data-stu-id="465bf-149">installState</span></span>|[<span data-ttu-id="465bf-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="465bf-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="465bf-151">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="465bf-151">The install state of the app.</span></span> <span data-ttu-id="465bf-152">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="465bf-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="465bf-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="465bf-153">installStateDetail</span></span>|[<span data-ttu-id="465bf-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="465bf-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="465bf-155">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="465bf-155">The install state detail of the app.</span></span> <span data-ttu-id="465bf-156">可取值为：`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="465bf-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="465bf-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="465bf-157">errorCode</span></span>|<span data-ttu-id="465bf-158">Int32</span><span class="sxs-lookup"><span data-stu-id="465bf-158">Int32</span></span>|<span data-ttu-id="465bf-159">错误代码用于安装或卸载失败。</span><span class="sxs-lookup"><span data-stu-id="465bf-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="465bf-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="465bf-160">osVersion</span></span>|<span data-ttu-id="465bf-161">String</span><span class="sxs-lookup"><span data-stu-id="465bf-161">String</span></span>|<span data-ttu-id="465bf-162">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="465bf-162">OS Version</span></span>|
|<span data-ttu-id="465bf-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="465bf-163">osDescription</span></span>|<span data-ttu-id="465bf-164">String</span><span class="sxs-lookup"><span data-stu-id="465bf-164">String</span></span>|<span data-ttu-id="465bf-165">操作系统说明</span><span class="sxs-lookup"><span data-stu-id="465bf-165">OS Description</span></span>|
|<span data-ttu-id="465bf-166">userName</span><span class="sxs-lookup"><span data-stu-id="465bf-166">userName</span></span>|<span data-ttu-id="465bf-167">String</span><span class="sxs-lookup"><span data-stu-id="465bf-167">String</span></span>|<span data-ttu-id="465bf-168">设备用户名</span><span class="sxs-lookup"><span data-stu-id="465bf-168">Device User Name</span></span>|
|<span data-ttu-id="465bf-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="465bf-169">userPrincipalName</span></span>|<span data-ttu-id="465bf-170">字符串</span><span class="sxs-lookup"><span data-stu-id="465bf-170">String</span></span>|<span data-ttu-id="465bf-171">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="465bf-171">User Principal Name</span></span>|
|<span data-ttu-id="465bf-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="465bf-172">displayVersion</span></span>|<span data-ttu-id="465bf-173">字符串</span><span class="sxs-lookup"><span data-stu-id="465bf-173">String</span></span>|<span data-ttu-id="465bf-174">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="465bf-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="465bf-175">响应</span><span class="sxs-lookup"><span data-stu-id="465bf-175">Response</span></span>
<span data-ttu-id="465bf-176">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="465bf-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="465bf-177">示例</span><span class="sxs-lookup"><span data-stu-id="465bf-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="465bf-178">请求</span><span class="sxs-lookup"><span data-stu-id="465bf-178">Request</span></span>
<span data-ttu-id="465bf-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="465bf-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="465bf-180">响应</span><span class="sxs-lookup"><span data-stu-id="465bf-180">Response</span></span>
<span data-ttu-id="465bf-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="465bf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





