---
title: 更新 mobileAppInstallStatus
description: 更新 mobileAppInstallStatus 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: efd71732f0a61f807be71ac4657eafdb921fd0f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934560"
---
# <a name="update-mobileappinstallstatus"></a><span data-ttu-id="8e4a9-103">更新 mobileAppInstallStatus</span><span class="sxs-lookup"><span data-stu-id="8e4a9-103">Update mobileAppInstallStatus</span></span>

> <span data-ttu-id="8e4a9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e4a9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e4a9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e4a9-107">更新[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-107">Update the properties of a [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e4a9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8e4a9-108">Prerequisites</span></span>
<span data-ttu-id="8e4a9-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8e4a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e4a9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8e4a9-111">Permission type</span></span>|<span data-ttu-id="8e4a9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8e4a9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e4a9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8e4a9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e4a9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e4a9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e4a9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8e4a9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e4a9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-116">Not supported.</span></span>|
|<span data-ttu-id="8e4a9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8e4a9-117">Application</span></span>|<span data-ttu-id="8e4a9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e4a9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8e4a9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/{mobileAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="8e4a9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8e4a9-120">Request headers</span></span>
|<span data-ttu-id="8e4a9-121">标头</span><span class="sxs-lookup"><span data-stu-id="8e4a9-121">Header</span></span>|<span data-ttu-id="8e4a9-122">值</span><span class="sxs-lookup"><span data-stu-id="8e4a9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e4a9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e4a9-123">Authorization</span></span>|<span data-ttu-id="8e4a9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e4a9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e4a9-125">Accept</span></span>|<span data-ttu-id="8e4a9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e4a9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e4a9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8e4a9-127">Request body</span></span>
<span data-ttu-id="8e4a9-128">在请求正文中，提供[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-128">In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object.</span></span>

<span data-ttu-id="8e4a9-129">下表显示时创建[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-129">The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md).</span></span>

|<span data-ttu-id="8e4a9-130">属性</span><span class="sxs-lookup"><span data-stu-id="8e4a9-130">Property</span></span>|<span data-ttu-id="8e4a9-131">类型</span><span class="sxs-lookup"><span data-stu-id="8e4a9-131">Type</span></span>|<span data-ttu-id="8e4a9-132">说明</span><span class="sxs-lookup"><span data-stu-id="8e4a9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e4a9-133">id</span><span class="sxs-lookup"><span data-stu-id="8e4a9-133">id</span></span>|<span data-ttu-id="8e4a9-134">String</span><span class="sxs-lookup"><span data-stu-id="8e4a9-134">String</span></span>|<span data-ttu-id="8e4a9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-135">Key of the entity.</span></span>|
|<span data-ttu-id="8e4a9-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="8e4a9-136">deviceName</span></span>|<span data-ttu-id="8e4a9-137">String</span><span class="sxs-lookup"><span data-stu-id="8e4a9-137">String</span></span>|<span data-ttu-id="8e4a9-138">设备名称</span><span class="sxs-lookup"><span data-stu-id="8e4a9-138">Device name</span></span>|
|<span data-ttu-id="8e4a9-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="8e4a9-139">deviceId</span></span>|<span data-ttu-id="8e4a9-140">String</span><span class="sxs-lookup"><span data-stu-id="8e4a9-140">String</span></span>|<span data-ttu-id="8e4a9-141">设备 ID</span><span class="sxs-lookup"><span data-stu-id="8e4a9-141">Device ID</span></span>|
|<span data-ttu-id="8e4a9-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8e4a9-142">lastSyncDateTime</span></span>|<span data-ttu-id="8e4a9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e4a9-143">DateTimeOffset</span></span>|<span data-ttu-id="8e4a9-144">上次同步日期时间</span><span class="sxs-lookup"><span data-stu-id="8e4a9-144">Last sync date time</span></span>|
|<span data-ttu-id="8e4a9-145">mobileAppInstallStatusValue</span><span class="sxs-lookup"><span data-stu-id="8e4a9-145">mobileAppInstallStatusValue</span></span>|[<span data-ttu-id="8e4a9-146">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="8e4a9-146">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="8e4a9-147">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-147">The install state of the app.</span></span> <span data-ttu-id="8e4a9-148">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-148">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="8e4a9-149">installState</span><span class="sxs-lookup"><span data-stu-id="8e4a9-149">installState</span></span>|[<span data-ttu-id="8e4a9-150">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="8e4a9-150">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="8e4a9-151">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-151">The install state of the app.</span></span> <span data-ttu-id="8e4a9-152">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-152">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="8e4a9-153">installStateDetail</span><span class="sxs-lookup"><span data-stu-id="8e4a9-153">installStateDetail</span></span>|[<span data-ttu-id="8e4a9-154">resultantAppStateDetail</span><span class="sxs-lookup"><span data-stu-id="8e4a9-154">resultantAppStateDetail</span></span>](../resources/intune-apps-resultantappstatedetail.md)|<span data-ttu-id="8e4a9-155">应用程序的安装状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-155">The install state detail of the app.</span></span> <span data-ttu-id="8e4a9-156">可取值为：`noAdditionalDetails`、`seeInstallErrorCode`、`seeUninstallErrorCode`、`pendingReboot`、`platformNotApplicable`、`minimumCpuSpeedNotMet`、`minimumLogicalProcessorCountNotMet`、`minimumPhysicalMemoryNotMet`、`minimumOsVersionNotMet`、`minimumDiskSpaceNotMet`、`processorArchitectureNotApplicable`。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-156">Possible values are: `noAdditionalDetails`, `seeInstallErrorCode`, `seeUninstallErrorCode`, `pendingReboot`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.</span></span>|
|<span data-ttu-id="8e4a9-157">errorCode</span><span class="sxs-lookup"><span data-stu-id="8e4a9-157">errorCode</span></span>|<span data-ttu-id="8e4a9-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8e4a9-158">Int32</span></span>|<span data-ttu-id="8e4a9-159">错误代码用于安装或卸载失败。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-159">The error code for install or uninstall failures.</span></span>|
|<span data-ttu-id="8e4a9-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="8e4a9-160">osVersion</span></span>|<span data-ttu-id="8e4a9-161">String</span><span class="sxs-lookup"><span data-stu-id="8e4a9-161">String</span></span>|<span data-ttu-id="8e4a9-162">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="8e4a9-162">OS Version</span></span>|
|<span data-ttu-id="8e4a9-163">osDescription</span><span class="sxs-lookup"><span data-stu-id="8e4a9-163">osDescription</span></span>|<span data-ttu-id="8e4a9-164">String</span><span class="sxs-lookup"><span data-stu-id="8e4a9-164">String</span></span>|<span data-ttu-id="8e4a9-165">操作系统说明</span><span class="sxs-lookup"><span data-stu-id="8e4a9-165">OS Description</span></span>|
|<span data-ttu-id="8e4a9-166">userName</span><span class="sxs-lookup"><span data-stu-id="8e4a9-166">userName</span></span>|<span data-ttu-id="8e4a9-167">String</span><span class="sxs-lookup"><span data-stu-id="8e4a9-167">String</span></span>|<span data-ttu-id="8e4a9-168">设备用户名</span><span class="sxs-lookup"><span data-stu-id="8e4a9-168">Device User Name</span></span>|
|<span data-ttu-id="8e4a9-169">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e4a9-169">userPrincipalName</span></span>|<span data-ttu-id="8e4a9-170">字符串</span><span class="sxs-lookup"><span data-stu-id="8e4a9-170">String</span></span>|<span data-ttu-id="8e4a9-171">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="8e4a9-171">User Principal Name</span></span>|
|<span data-ttu-id="8e4a9-172">displayVersion</span><span class="sxs-lookup"><span data-stu-id="8e4a9-172">displayVersion</span></span>|<span data-ttu-id="8e4a9-173">字符串</span><span class="sxs-lookup"><span data-stu-id="8e4a9-173">String</span></span>|<span data-ttu-id="8e4a9-174">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="8e4a9-174">Human readable version of the application</span></span>|



## <a name="response"></a><span data-ttu-id="8e4a9-175">响应</span><span class="sxs-lookup"><span data-stu-id="8e4a9-175">Response</span></span>
<span data-ttu-id="8e4a9-176">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-176">If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e4a9-177">示例</span><span class="sxs-lookup"><span data-stu-id="8e4a9-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e4a9-178">请求</span><span class="sxs-lookup"><span data-stu-id="8e4a9-178">Request</span></span>
<span data-ttu-id="8e4a9-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e4a9-180">响应</span><span class="sxs-lookup"><span data-stu-id="8e4a9-180">Response</span></span>
<span data-ttu-id="8e4a9-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8e4a9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





