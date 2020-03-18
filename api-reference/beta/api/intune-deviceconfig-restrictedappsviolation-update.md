---
title: 更新 restrictedAppsViolation
description: 更新 restrictedAppsViolation 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5dd783a68ffe608265d0b65f9404678d244b705d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42742391"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="66857-103">更新 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="66857-103">Update restrictedAppsViolation</span></span>

> <span data-ttu-id="66857-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66857-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66857-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66857-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66857-106">更新[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="66857-106">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66857-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="66857-107">Prerequisites</span></span>
<span data-ttu-id="66857-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66857-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="66857-110">Permission type</span></span>|<span data-ttu-id="66857-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66857-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66857-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66857-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66857-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66857-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66857-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66857-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66857-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66857-115">Not supported.</span></span>|
|<span data-ttu-id="66857-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="66857-116">Application</span></span>|<span data-ttu-id="66857-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66857-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66857-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66857-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="66857-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="66857-119">Request headers</span></span>
|<span data-ttu-id="66857-120">标头</span><span class="sxs-lookup"><span data-stu-id="66857-120">Header</span></span>|<span data-ttu-id="66857-121">值</span><span class="sxs-lookup"><span data-stu-id="66857-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66857-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66857-122">Authorization</span></span>|<span data-ttu-id="66857-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66857-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66857-124">接受</span><span class="sxs-lookup"><span data-stu-id="66857-124">Accept</span></span>|<span data-ttu-id="66857-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66857-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66857-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="66857-126">Request body</span></span>
<span data-ttu-id="66857-127">在请求正文中，提供[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66857-127">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="66857-128">下表显示创建[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66857-128">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="66857-129">属性</span><span class="sxs-lookup"><span data-stu-id="66857-129">Property</span></span>|<span data-ttu-id="66857-130">类型</span><span class="sxs-lookup"><span data-stu-id="66857-130">Type</span></span>|<span data-ttu-id="66857-131">说明</span><span class="sxs-lookup"><span data-stu-id="66857-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66857-132">id</span><span class="sxs-lookup"><span data-stu-id="66857-132">id</span></span>|<span data-ttu-id="66857-133">字符串</span><span class="sxs-lookup"><span data-stu-id="66857-133">String</span></span>|<span data-ttu-id="66857-134">对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="66857-134">Unique identifier for the object.</span></span> <span data-ttu-id="66857-135">由 accountId、deviceId、policyId 和 userId 组成</span><span class="sxs-lookup"><span data-stu-id="66857-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="66857-136">userId</span><span class="sxs-lookup"><span data-stu-id="66857-136">userId</span></span>|<span data-ttu-id="66857-137">String</span><span class="sxs-lookup"><span data-stu-id="66857-137">String</span></span>|<span data-ttu-id="66857-138">用户唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="66857-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="66857-139">userName</span><span class="sxs-lookup"><span data-stu-id="66857-139">userName</span></span>|<span data-ttu-id="66857-140">String</span><span class="sxs-lookup"><span data-stu-id="66857-140">String</span></span>|<span data-ttu-id="66857-141">用户名</span><span class="sxs-lookup"><span data-stu-id="66857-141">User name</span></span>|
|<span data-ttu-id="66857-142">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="66857-142">managedDeviceId</span></span>|<span data-ttu-id="66857-143">String</span><span class="sxs-lookup"><span data-stu-id="66857-143">String</span></span>|<span data-ttu-id="66857-144">托管设备唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="66857-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="66857-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="66857-145">deviceName</span></span>|<span data-ttu-id="66857-146">String</span><span class="sxs-lookup"><span data-stu-id="66857-146">String</span></span>|<span data-ttu-id="66857-147">设备名称</span><span class="sxs-lookup"><span data-stu-id="66857-147">Device name</span></span>|
|<span data-ttu-id="66857-148">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="66857-148">deviceConfigurationId</span></span>|<span data-ttu-id="66857-149">String</span><span class="sxs-lookup"><span data-stu-id="66857-149">String</span></span>|<span data-ttu-id="66857-150">设备配置文件唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="66857-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="66857-151">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="66857-151">deviceConfigurationName</span></span>|<span data-ttu-id="66857-152">String</span><span class="sxs-lookup"><span data-stu-id="66857-152">String</span></span>|<span data-ttu-id="66857-153">设备配置文件名称</span><span class="sxs-lookup"><span data-stu-id="66857-153">Device configuration profile name</span></span>|
|<span data-ttu-id="66857-154">platformType</span><span class="sxs-lookup"><span data-stu-id="66857-154">platformType</span></span>|[<span data-ttu-id="66857-155">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="66857-155">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="66857-156">平台类型。</span><span class="sxs-lookup"><span data-stu-id="66857-156">Platform type.</span></span> <span data-ttu-id="66857-157">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="66857-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="66857-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="66857-158">restrictedAppsState</span></span>|[<span data-ttu-id="66857-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="66857-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="66857-160">受限制的应用程序状态。</span><span class="sxs-lookup"><span data-stu-id="66857-160">Restricted apps state.</span></span> <span data-ttu-id="66857-161">可取值为：`prohibitedApps`、`notApprovedApps`。</span><span class="sxs-lookup"><span data-stu-id="66857-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="66857-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="66857-162">restrictedApps</span></span>|<span data-ttu-id="66857-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="66857-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="66857-164">违反受限制的应用程序的列表</span><span class="sxs-lookup"><span data-stu-id="66857-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="66857-165">响应</span><span class="sxs-lookup"><span data-stu-id="66857-165">Response</span></span>
<span data-ttu-id="66857-166">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66857-166">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66857-167">示例</span><span class="sxs-lookup"><span data-stu-id="66857-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="66857-168">请求</span><span class="sxs-lookup"><span data-stu-id="66857-168">Request</span></span>
<span data-ttu-id="66857-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66857-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="66857-170">响应</span><span class="sxs-lookup"><span data-stu-id="66857-170">Response</span></span>
<span data-ttu-id="66857-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66857-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "53f99903-9903-53f9-0399-f9530399f953",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```




