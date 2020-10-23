---
title: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c99bbcfdb697ca3ec006d7ce8cffdf858b8ac9e9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729852"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="b7221-103">更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="b7221-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="b7221-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7221-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7221-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7221-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7221-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7221-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7221-107">更新 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b7221-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7221-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b7221-108">Prerequisites</span></span>
<span data-ttu-id="b7221-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7221-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7221-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7221-111">Permission type</span></span>|<span data-ttu-id="b7221-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b7221-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7221-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7221-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7221-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7221-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7221-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7221-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7221-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7221-116">Not supported.</span></span>|
|<span data-ttu-id="b7221-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7221-117">Application</span></span>|<span data-ttu-id="b7221-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7221-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7221-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7221-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b7221-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7221-120">Request headers</span></span>
|<span data-ttu-id="b7221-121">标头</span><span class="sxs-lookup"><span data-stu-id="b7221-121">Header</span></span>|<span data-ttu-id="b7221-122">值</span><span class="sxs-lookup"><span data-stu-id="b7221-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7221-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7221-123">Authorization</span></span>|<span data-ttu-id="b7221-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b7221-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7221-125">接受</span><span class="sxs-lookup"><span data-stu-id="b7221-125">Accept</span></span>|<span data-ttu-id="b7221-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7221-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7221-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7221-127">Request body</span></span>
<span data-ttu-id="b7221-128">在请求正文中，提供 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7221-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

<span data-ttu-id="b7221-129">下表显示创建 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b7221-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).</span></span>

|<span data-ttu-id="b7221-130">属性</span><span class="sxs-lookup"><span data-stu-id="b7221-130">Property</span></span>|<span data-ttu-id="b7221-131">类型</span><span class="sxs-lookup"><span data-stu-id="b7221-131">Type</span></span>|<span data-ttu-id="b7221-132">说明</span><span class="sxs-lookup"><span data-stu-id="b7221-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7221-133">id</span><span class="sxs-lookup"><span data-stu-id="b7221-133">id</span></span>|<span data-ttu-id="b7221-134">String</span><span class="sxs-lookup"><span data-stu-id="b7221-134">String</span></span>|<span data-ttu-id="b7221-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b7221-135">Key of the entity.</span></span>|
|<span data-ttu-id="b7221-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="b7221-136">deviceName</span></span>|<span data-ttu-id="b7221-137">String</span><span class="sxs-lookup"><span data-stu-id="b7221-137">String</span></span>|<span data-ttu-id="b7221-138">设备名称。</span><span class="sxs-lookup"><span data-stu-id="b7221-138">Device name.</span></span>|
|<span data-ttu-id="b7221-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="b7221-139">deviceId</span></span>|<span data-ttu-id="b7221-140">String</span><span class="sxs-lookup"><span data-stu-id="b7221-140">String</span></span>|<span data-ttu-id="b7221-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="b7221-141">Device ID.</span></span>|
|<span data-ttu-id="b7221-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b7221-142">lastSyncDateTime</span></span>|<span data-ttu-id="b7221-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7221-143">DateTimeOffset</span></span>|<span data-ttu-id="b7221-144">上次同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="b7221-144">Last sync date time.</span></span>|
|<span data-ttu-id="b7221-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="b7221-145">osVersion</span></span>|<span data-ttu-id="b7221-146">String</span><span class="sxs-lookup"><span data-stu-id="b7221-146">String</span></span>|<span data-ttu-id="b7221-147">Windows OS 版本。</span><span class="sxs-lookup"><span data-stu-id="b7221-147">Windows OS Version.</span></span>|
|<span data-ttu-id="b7221-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="b7221-148">osDescription</span></span>|<span data-ttu-id="b7221-149">String</span><span class="sxs-lookup"><span data-stu-id="b7221-149">String</span></span>|<span data-ttu-id="b7221-150">Windows OS 版本说明。</span><span class="sxs-lookup"><span data-stu-id="b7221-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="b7221-151">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="b7221-151">deploymentStatus</span></span>|[<span data-ttu-id="b7221-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="b7221-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="b7221-153">策略的部署状态。</span><span class="sxs-lookup"><span data-stu-id="b7221-153">The deployment state of the policy.</span></span> <span data-ttu-id="b7221-154">可取值为：`unknown`、`success`、`tokenError`、`notAuthorizedByToken`、`policyNotFound`。</span><span class="sxs-lookup"><span data-stu-id="b7221-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="b7221-155">userName</span><span class="sxs-lookup"><span data-stu-id="b7221-155">userName</span></span>|<span data-ttu-id="b7221-156">String</span><span class="sxs-lookup"><span data-stu-id="b7221-156">String</span></span>|<span data-ttu-id="b7221-157">此设备的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="b7221-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="b7221-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b7221-158">userPrincipalName</span></span>|<span data-ttu-id="b7221-159">String</span><span class="sxs-lookup"><span data-stu-id="b7221-159">String</span></span>|<span data-ttu-id="b7221-160">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="b7221-160">User Principal Name.</span></span>|
|<span data-ttu-id="b7221-161">policyVersion</span><span class="sxs-lookup"><span data-stu-id="b7221-161">policyVersion</span></span>|<span data-ttu-id="b7221-162">String</span><span class="sxs-lookup"><span data-stu-id="b7221-162">String</span></span>|<span data-ttu-id="b7221-163">WindowsDefenderApplicationControl 补充策略的人工可读版本。</span><span class="sxs-lookup"><span data-stu-id="b7221-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="b7221-164">响应</span><span class="sxs-lookup"><span data-stu-id="b7221-164">Response</span></span>
<span data-ttu-id="b7221-165">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b7221-165">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7221-166">示例</span><span class="sxs-lookup"><span data-stu-id="b7221-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7221-167">请求</span><span class="sxs-lookup"><span data-stu-id="b7221-167">Request</span></span>
<span data-ttu-id="b7221-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7221-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
Content-type: application/json
Content-length: 486

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "deploymentStatus": "success",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "policyVersion": "Policy Version value"
}
```

### <a name="response"></a><span data-ttu-id="b7221-169">响应</span><span class="sxs-lookup"><span data-stu-id="b7221-169">Response</span></span>
<span data-ttu-id="b7221-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7221-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "e3c01841-1841-e3c0-4118-c0e34118c0e3",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "deploymentStatus": "success",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "policyVersion": "Policy Version value"
}
```





