---
title: 创建 restrictedAppsViolation
description: 创建新的 restrictedAppsViolation 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3c614e14193945c84fd60f46205d7803b91da55
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155055"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="7a865-103">创建 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="7a865-103">Create restrictedAppsViolation</span></span>

<span data-ttu-id="7a865-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a865-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7a865-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a865-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a865-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a865-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a865-107">创建新的 [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a865-107">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7a865-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7a865-108">Prerequisites</span></span>
<span data-ttu-id="7a865-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a865-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a865-111">Permission type</span></span>|<span data-ttu-id="7a865-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a865-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a865-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a865-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a865-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a865-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a865-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a865-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a865-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a865-116">Not supported.</span></span>|
|<span data-ttu-id="7a865-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a865-117">Application</span></span>|<span data-ttu-id="7a865-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a865-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a865-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a865-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="7a865-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a865-120">Request headers</span></span>
|<span data-ttu-id="7a865-121">标头</span><span class="sxs-lookup"><span data-stu-id="7a865-121">Header</span></span>|<span data-ttu-id="7a865-122">值</span><span class="sxs-lookup"><span data-stu-id="7a865-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a865-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a865-123">Authorization</span></span>|<span data-ttu-id="7a865-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7a865-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a865-125">接受</span><span class="sxs-lookup"><span data-stu-id="7a865-125">Accept</span></span>|<span data-ttu-id="7a865-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a865-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a865-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a865-127">Request body</span></span>
<span data-ttu-id="7a865-128">在请求正文中，提供 restrictedAppsViolation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a865-128">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="7a865-129">下表显示创建 restrictedAppsViolation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7a865-129">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="7a865-130">属性</span><span class="sxs-lookup"><span data-stu-id="7a865-130">Property</span></span>|<span data-ttu-id="7a865-131">类型</span><span class="sxs-lookup"><span data-stu-id="7a865-131">Type</span></span>|<span data-ttu-id="7a865-132">说明</span><span class="sxs-lookup"><span data-stu-id="7a865-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a865-133">id</span><span class="sxs-lookup"><span data-stu-id="7a865-133">id</span></span>|<span data-ttu-id="7a865-134">String</span><span class="sxs-lookup"><span data-stu-id="7a865-134">String</span></span>|<span data-ttu-id="7a865-135">对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="7a865-135">Unique identifier for the object.</span></span> <span data-ttu-id="7a865-136">由 accountId、deviceId、policyId 和 userId 组成</span><span class="sxs-lookup"><span data-stu-id="7a865-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="7a865-137">userId</span><span class="sxs-lookup"><span data-stu-id="7a865-137">userId</span></span>|<span data-ttu-id="7a865-138">String</span><span class="sxs-lookup"><span data-stu-id="7a865-138">String</span></span>|<span data-ttu-id="7a865-139">用户唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="7a865-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="7a865-140">userName</span><span class="sxs-lookup"><span data-stu-id="7a865-140">userName</span></span>|<span data-ttu-id="7a865-141">String</span><span class="sxs-lookup"><span data-stu-id="7a865-141">String</span></span>|<span data-ttu-id="7a865-142">用户名</span><span class="sxs-lookup"><span data-stu-id="7a865-142">User name</span></span>|
|<span data-ttu-id="7a865-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="7a865-143">managedDeviceId</span></span>|<span data-ttu-id="7a865-144">String</span><span class="sxs-lookup"><span data-stu-id="7a865-144">String</span></span>|<span data-ttu-id="7a865-145">托管设备唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="7a865-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="7a865-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="7a865-146">deviceName</span></span>|<span data-ttu-id="7a865-147">String</span><span class="sxs-lookup"><span data-stu-id="7a865-147">String</span></span>|<span data-ttu-id="7a865-148">设备名称</span><span class="sxs-lookup"><span data-stu-id="7a865-148">Device name</span></span>|
|<span data-ttu-id="7a865-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="7a865-149">deviceConfigurationId</span></span>|<span data-ttu-id="7a865-150">String</span><span class="sxs-lookup"><span data-stu-id="7a865-150">String</span></span>|<span data-ttu-id="7a865-151">设备配置文件的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="7a865-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="7a865-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="7a865-152">deviceConfigurationName</span></span>|<span data-ttu-id="7a865-153">String</span><span class="sxs-lookup"><span data-stu-id="7a865-153">String</span></span>|<span data-ttu-id="7a865-154">设备配置文件名称</span><span class="sxs-lookup"><span data-stu-id="7a865-154">Device configuration profile name</span></span>|
|<span data-ttu-id="7a865-155">platformType</span><span class="sxs-lookup"><span data-stu-id="7a865-155">platformType</span></span>|[<span data-ttu-id="7a865-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="7a865-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="7a865-157">平台类型。</span><span class="sxs-lookup"><span data-stu-id="7a865-157">Platform type.</span></span> <span data-ttu-id="7a865-158">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`windows10XProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="7a865-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="7a865-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="7a865-159">restrictedAppsState</span></span>|[<span data-ttu-id="7a865-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="7a865-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="7a865-161">受限制的应用状态。</span><span class="sxs-lookup"><span data-stu-id="7a865-161">Restricted apps state.</span></span> <span data-ttu-id="7a865-162">可取值为：`prohibitedApps`、`notApprovedApps`。</span><span class="sxs-lookup"><span data-stu-id="7a865-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="7a865-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="7a865-163">restrictedApps</span></span>|<span data-ttu-id="7a865-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7a865-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="7a865-165">违反的受限应用列表</span><span class="sxs-lookup"><span data-stu-id="7a865-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="7a865-166">响应</span><span class="sxs-lookup"><span data-stu-id="7a865-166">Response</span></span>
<span data-ttu-id="7a865-167">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7a865-167">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a865-168">示例</span><span class="sxs-lookup"><span data-stu-id="7a865-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="7a865-169">请求</span><span class="sxs-lookup"><span data-stu-id="7a865-169">Request</span></span>
<span data-ttu-id="7a865-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a865-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
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

### <a name="response"></a><span data-ttu-id="7a865-171">响应</span><span class="sxs-lookup"><span data-stu-id="7a865-171">Response</span></span>
<span data-ttu-id="7a865-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a865-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




