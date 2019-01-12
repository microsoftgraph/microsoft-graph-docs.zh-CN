---
title: 创建 restrictedAppsViolation
description: 创建新的 restrictedAppsViolation 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de7a461fd3591f3473ccfa8f15d85fa2dbab6808
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940566"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="e2871-103">创建 restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="e2871-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="e2871-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e2871-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2871-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2871-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2871-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e2871-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2871-107">创建新的[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2871-107">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e2871-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e2871-108">Prerequisites</span></span>
<span data-ttu-id="e2871-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e2871-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2871-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2871-111">Permission type</span></span>|<span data-ttu-id="e2871-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e2871-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2871-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2871-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2871-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2871-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2871-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2871-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2871-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2871-116">Not supported.</span></span>|
|<span data-ttu-id="e2871-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2871-117">Application</span></span>|<span data-ttu-id="e2871-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2871-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2871-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2871-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="e2871-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2871-120">Request headers</span></span>
|<span data-ttu-id="e2871-121">标头</span><span class="sxs-lookup"><span data-stu-id="e2871-121">Header</span></span>|<span data-ttu-id="e2871-122">值</span><span class="sxs-lookup"><span data-stu-id="e2871-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2871-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2871-123">Authorization</span></span>|<span data-ttu-id="e2871-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e2871-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2871-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2871-125">Accept</span></span>|<span data-ttu-id="e2871-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2871-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2871-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2871-127">Request body</span></span>
<span data-ttu-id="e2871-128">在请求正文中，提供 restrictedAppsViolation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2871-128">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="e2871-129">下表显示时创建 restrictedAppsViolation 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e2871-129">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="e2871-130">属性</span><span class="sxs-lookup"><span data-stu-id="e2871-130">Property</span></span>|<span data-ttu-id="e2871-131">类型</span><span class="sxs-lookup"><span data-stu-id="e2871-131">Type</span></span>|<span data-ttu-id="e2871-132">说明</span><span class="sxs-lookup"><span data-stu-id="e2871-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2871-133">id</span><span class="sxs-lookup"><span data-stu-id="e2871-133">id</span></span>|<span data-ttu-id="e2871-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e2871-134">String</span></span>|<span data-ttu-id="e2871-135">对象的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e2871-135">Unique identifier for the object.</span></span> <span data-ttu-id="e2871-136">由 accountId、 deviceId、 policyId 和用户 Id</span><span class="sxs-lookup"><span data-stu-id="e2871-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="e2871-137">userId</span><span class="sxs-lookup"><span data-stu-id="e2871-137">userId</span></span>|<span data-ttu-id="e2871-138">String</span><span class="sxs-lookup"><span data-stu-id="e2871-138">String</span></span>|<span data-ttu-id="e2871-139">用户的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="e2871-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="e2871-140">userName</span><span class="sxs-lookup"><span data-stu-id="e2871-140">userName</span></span>|<span data-ttu-id="e2871-141">String</span><span class="sxs-lookup"><span data-stu-id="e2871-141">String</span></span>|<span data-ttu-id="e2871-142">用户名</span><span class="sxs-lookup"><span data-stu-id="e2871-142">User name</span></span>|
|<span data-ttu-id="e2871-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="e2871-143">managedDeviceId</span></span>|<span data-ttu-id="e2871-144">字符串</span><span class="sxs-lookup"><span data-stu-id="e2871-144">String</span></span>|<span data-ttu-id="e2871-145">托管的设备的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="e2871-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="e2871-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="e2871-146">deviceName</span></span>|<span data-ttu-id="e2871-147">String</span><span class="sxs-lookup"><span data-stu-id="e2871-147">String</span></span>|<span data-ttu-id="e2871-148">设备名称</span><span class="sxs-lookup"><span data-stu-id="e2871-148">Device name</span></span>|
|<span data-ttu-id="e2871-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e2871-149">deviceConfigurationId</span></span>|<span data-ttu-id="e2871-150">字符串</span><span class="sxs-lookup"><span data-stu-id="e2871-150">String</span></span>|<span data-ttu-id="e2871-151">设备配置配置文件的唯一标识符，必须为 Guid</span><span class="sxs-lookup"><span data-stu-id="e2871-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="e2871-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="e2871-152">deviceConfigurationName</span></span>|<span data-ttu-id="e2871-153">字符串</span><span class="sxs-lookup"><span data-stu-id="e2871-153">String</span></span>|<span data-ttu-id="e2871-154">设备配置配置文件名称</span><span class="sxs-lookup"><span data-stu-id="e2871-154">Device configuration profile name</span></span>|
|<span data-ttu-id="e2871-155">platformType</span><span class="sxs-lookup"><span data-stu-id="e2871-155">platformType</span></span>|[<span data-ttu-id="e2871-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="e2871-156">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="e2871-157">平台类型。</span><span class="sxs-lookup"><span data-stu-id="e2871-157">Platform type.</span></span> <span data-ttu-id="e2871-158">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all`。</span><span class="sxs-lookup"><span data-stu-id="e2871-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="e2871-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="e2871-159">restrictedAppsState</span></span>|[<span data-ttu-id="e2871-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="e2871-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="e2871-161">受限制的应用程序状态。</span><span class="sxs-lookup"><span data-stu-id="e2871-161">Restricted apps state.</span></span> <span data-ttu-id="e2871-162">可取值为：`prohibitedApps`、`notApprovedApps`。</span><span class="sxs-lookup"><span data-stu-id="e2871-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="e2871-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="e2871-163">restrictedApps</span></span>|<span data-ttu-id="e2871-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2871-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="e2871-165">违反受限制的应用程序的列表</span><span class="sxs-lookup"><span data-stu-id="e2871-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="e2871-166">响应</span><span class="sxs-lookup"><span data-stu-id="e2871-166">Response</span></span>
<span data-ttu-id="e2871-167">如果成功，此方法返回`201 Created`响应代码和响应正文中的[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2871-167">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2871-168">示例</span><span class="sxs-lookup"><span data-stu-id="e2871-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2871-169">请求</span><span class="sxs-lookup"><span data-stu-id="e2871-169">Request</span></span>
<span data-ttu-id="e2871-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2871-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2871-171">响应</span><span class="sxs-lookup"><span data-stu-id="e2871-171">Response</span></span>
<span data-ttu-id="e2871-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2871-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





