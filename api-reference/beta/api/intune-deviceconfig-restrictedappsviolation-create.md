---
title: 创建 restrictedAppsViolation
description: 创建新的 restrictedAppsViolation 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1c207bc34403f831d86d9849faf2287210d7bb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518182"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="96f03-103">创建 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="96f03-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="96f03-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96f03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96f03-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96f03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96f03-106">创建新的[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96f03-106">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96f03-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="96f03-107">Prerequisites</span></span>
<span data-ttu-id="96f03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96f03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96f03-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="96f03-110">Permission type</span></span>|<span data-ttu-id="96f03-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96f03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96f03-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96f03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96f03-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96f03-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96f03-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96f03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96f03-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="96f03-115">Not supported.</span></span>|
|<span data-ttu-id="96f03-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="96f03-116">Application</span></span>|<span data-ttu-id="96f03-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="96f03-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96f03-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96f03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="96f03-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="96f03-119">Request headers</span></span>
|<span data-ttu-id="96f03-120">标头</span><span class="sxs-lookup"><span data-stu-id="96f03-120">Header</span></span>|<span data-ttu-id="96f03-121">值</span><span class="sxs-lookup"><span data-stu-id="96f03-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96f03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96f03-122">Authorization</span></span>|<span data-ttu-id="96f03-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="96f03-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96f03-124">接受</span><span class="sxs-lookup"><span data-stu-id="96f03-124">Accept</span></span>|<span data-ttu-id="96f03-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96f03-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96f03-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="96f03-126">Request body</span></span>
<span data-ttu-id="96f03-127">在请求正文中, 提供 restrictedAppsViolation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96f03-127">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="96f03-128">下表显示创建 restrictedAppsViolation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="96f03-128">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="96f03-129">属性</span><span class="sxs-lookup"><span data-stu-id="96f03-129">Property</span></span>|<span data-ttu-id="96f03-130">类型</span><span class="sxs-lookup"><span data-stu-id="96f03-130">Type</span></span>|<span data-ttu-id="96f03-131">说明</span><span class="sxs-lookup"><span data-stu-id="96f03-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96f03-132">id</span><span class="sxs-lookup"><span data-stu-id="96f03-132">id</span></span>|<span data-ttu-id="96f03-133">String</span><span class="sxs-lookup"><span data-stu-id="96f03-133">String</span></span>|<span data-ttu-id="96f03-134">对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="96f03-134">Unique identifier for the object.</span></span> <span data-ttu-id="96f03-135">由 accountId、deviceId、policyId 和 userId 组成</span><span class="sxs-lookup"><span data-stu-id="96f03-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="96f03-136">userId</span><span class="sxs-lookup"><span data-stu-id="96f03-136">userId</span></span>|<span data-ttu-id="96f03-137">字符串</span><span class="sxs-lookup"><span data-stu-id="96f03-137">String</span></span>|<span data-ttu-id="96f03-138">用户唯一标识符, 必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="96f03-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="96f03-139">userName</span><span class="sxs-lookup"><span data-stu-id="96f03-139">userName</span></span>|<span data-ttu-id="96f03-140">String</span><span class="sxs-lookup"><span data-stu-id="96f03-140">String</span></span>|<span data-ttu-id="96f03-141">用户名</span><span class="sxs-lookup"><span data-stu-id="96f03-141">User name</span></span>|
|<span data-ttu-id="96f03-142">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="96f03-142">managedDeviceId</span></span>|<span data-ttu-id="96f03-143">字符串</span><span class="sxs-lookup"><span data-stu-id="96f03-143">String</span></span>|<span data-ttu-id="96f03-144">托管设备唯一标识符, 必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="96f03-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="96f03-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="96f03-145">deviceName</span></span>|<span data-ttu-id="96f03-146">字符串</span><span class="sxs-lookup"><span data-stu-id="96f03-146">String</span></span>|<span data-ttu-id="96f03-147">设备名称</span><span class="sxs-lookup"><span data-stu-id="96f03-147">Device name</span></span>|
|<span data-ttu-id="96f03-148">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="96f03-148">deviceConfigurationId</span></span>|<span data-ttu-id="96f03-149">字符串</span><span class="sxs-lookup"><span data-stu-id="96f03-149">String</span></span>|<span data-ttu-id="96f03-150">设备配置文件唯一标识符, 必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="96f03-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="96f03-151">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="96f03-151">deviceConfigurationName</span></span>|<span data-ttu-id="96f03-152">字符串</span><span class="sxs-lookup"><span data-stu-id="96f03-152">String</span></span>|<span data-ttu-id="96f03-153">设备配置文件名称</span><span class="sxs-lookup"><span data-stu-id="96f03-153">Device configuration profile name</span></span>|
|<span data-ttu-id="96f03-154">platformType</span><span class="sxs-lookup"><span data-stu-id="96f03-154">platformType</span></span>|[<span data-ttu-id="96f03-155">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="96f03-155">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="96f03-156">平台类型。</span><span class="sxs-lookup"><span data-stu-id="96f03-156">Platform type.</span></span> <span data-ttu-id="96f03-157">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="96f03-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="96f03-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="96f03-158">restrictedAppsState</span></span>|[<span data-ttu-id="96f03-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="96f03-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="96f03-160">受限制的应用程序状态。</span><span class="sxs-lookup"><span data-stu-id="96f03-160">Restricted apps state.</span></span> <span data-ttu-id="96f03-161">可取值为：`prohibitedApps`、`notApprovedApps`。</span><span class="sxs-lookup"><span data-stu-id="96f03-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="96f03-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="96f03-162">restrictedApps</span></span>|<span data-ttu-id="96f03-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="96f03-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="96f03-164">违反受限制的应用程序的列表</span><span class="sxs-lookup"><span data-stu-id="96f03-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="96f03-165">响应</span><span class="sxs-lookup"><span data-stu-id="96f03-165">Response</span></span>
<span data-ttu-id="96f03-166">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96f03-166">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96f03-167">示例</span><span class="sxs-lookup"><span data-stu-id="96f03-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="96f03-168">请求</span><span class="sxs-lookup"><span data-stu-id="96f03-168">Request</span></span>
<span data-ttu-id="96f03-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96f03-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96f03-170">响应</span><span class="sxs-lookup"><span data-stu-id="96f03-170">Response</span></span>
<span data-ttu-id="96f03-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96f03-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





