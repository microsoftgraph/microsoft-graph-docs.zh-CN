---
title: 创建 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: 创建新的 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fef6d21122855587f2b107b861c63381ba0d4dd5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223099"
---
# <a name="create-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="022e7-103">创建 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="022e7-103">Create windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="022e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="022e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="022e7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="022e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="022e7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="022e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="022e7-107">创建新的 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="022e7-107">Create a new [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="022e7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="022e7-108">Prerequisites</span></span>
<span data-ttu-id="022e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="022e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="022e7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="022e7-111">Permission type</span></span>|<span data-ttu-id="022e7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="022e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="022e7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="022e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="022e7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="022e7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="022e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="022e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="022e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="022e7-116">Not supported.</span></span>|
|<span data-ttu-id="022e7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="022e7-117">Application</span></span>|<span data-ttu-id="022e7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="022e7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="022e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="022e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="022e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="022e7-120">Request headers</span></span>
|<span data-ttu-id="022e7-121">标头</span><span class="sxs-lookup"><span data-stu-id="022e7-121">Header</span></span>|<span data-ttu-id="022e7-122">值</span><span class="sxs-lookup"><span data-stu-id="022e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="022e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="022e7-123">Authorization</span></span>|<span data-ttu-id="022e7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="022e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="022e7-125">接受</span><span class="sxs-lookup"><span data-stu-id="022e7-125">Accept</span></span>|<span data-ttu-id="022e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="022e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="022e7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="022e7-127">Request body</span></span>
<span data-ttu-id="022e7-128">在请求正文中，提供 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="022e7-128">In the request body, supply a JSON representation for the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object.</span></span>

<span data-ttu-id="022e7-129">下表显示创建 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="022e7-129">The following table shows the properties that are required when you create the windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.</span></span>

|<span data-ttu-id="022e7-130">属性</span><span class="sxs-lookup"><span data-stu-id="022e7-130">Property</span></span>|<span data-ttu-id="022e7-131">类型</span><span class="sxs-lookup"><span data-stu-id="022e7-131">Type</span></span>|<span data-ttu-id="022e7-132">说明</span><span class="sxs-lookup"><span data-stu-id="022e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="022e7-133">id</span><span class="sxs-lookup"><span data-stu-id="022e7-133">id</span></span>|<span data-ttu-id="022e7-134">String</span><span class="sxs-lookup"><span data-stu-id="022e7-134">String</span></span>|<span data-ttu-id="022e7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="022e7-135">Key of the entity.</span></span>|
|<span data-ttu-id="022e7-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="022e7-136">deviceName</span></span>|<span data-ttu-id="022e7-137">String</span><span class="sxs-lookup"><span data-stu-id="022e7-137">String</span></span>|<span data-ttu-id="022e7-138">设备名称。</span><span class="sxs-lookup"><span data-stu-id="022e7-138">Device name.</span></span>|
|<span data-ttu-id="022e7-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="022e7-139">deviceId</span></span>|<span data-ttu-id="022e7-140">String</span><span class="sxs-lookup"><span data-stu-id="022e7-140">String</span></span>|<span data-ttu-id="022e7-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="022e7-141">Device ID.</span></span>|
|<span data-ttu-id="022e7-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="022e7-142">lastSyncDateTime</span></span>|<span data-ttu-id="022e7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="022e7-143">DateTimeOffset</span></span>|<span data-ttu-id="022e7-144">上次同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="022e7-144">Last sync date time.</span></span>|
|<span data-ttu-id="022e7-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="022e7-145">osVersion</span></span>|<span data-ttu-id="022e7-146">String</span><span class="sxs-lookup"><span data-stu-id="022e7-146">String</span></span>|<span data-ttu-id="022e7-147">Windows OS 版本。</span><span class="sxs-lookup"><span data-stu-id="022e7-147">Windows OS Version.</span></span>|
|<span data-ttu-id="022e7-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="022e7-148">osDescription</span></span>|<span data-ttu-id="022e7-149">String</span><span class="sxs-lookup"><span data-stu-id="022e7-149">String</span></span>|<span data-ttu-id="022e7-150">Windows OS 版本说明。</span><span class="sxs-lookup"><span data-stu-id="022e7-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="022e7-151">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="022e7-151">deploymentStatus</span></span>|[<span data-ttu-id="022e7-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="022e7-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="022e7-153">策略的部署状态。</span><span class="sxs-lookup"><span data-stu-id="022e7-153">The deployment state of the policy.</span></span> <span data-ttu-id="022e7-154">可取值为：`unknown`、`success`、`tokenError`、`notAuthorizedByToken`、`policyNotFound`。</span><span class="sxs-lookup"><span data-stu-id="022e7-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="022e7-155">userName</span><span class="sxs-lookup"><span data-stu-id="022e7-155">userName</span></span>|<span data-ttu-id="022e7-156">String</span><span class="sxs-lookup"><span data-stu-id="022e7-156">String</span></span>|<span data-ttu-id="022e7-157">此设备的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="022e7-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="022e7-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="022e7-158">userPrincipalName</span></span>|<span data-ttu-id="022e7-159">String</span><span class="sxs-lookup"><span data-stu-id="022e7-159">String</span></span>|<span data-ttu-id="022e7-160">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="022e7-160">User Principal Name.</span></span>|
|<span data-ttu-id="022e7-161">policyVersion</span><span class="sxs-lookup"><span data-stu-id="022e7-161">policyVersion</span></span>|<span data-ttu-id="022e7-162">String</span><span class="sxs-lookup"><span data-stu-id="022e7-162">String</span></span>|<span data-ttu-id="022e7-163">WindowsDefenderApplicationControl 补充策略的人工可读版本。</span><span class="sxs-lookup"><span data-stu-id="022e7-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="022e7-164">响应</span><span class="sxs-lookup"><span data-stu-id="022e7-164">Response</span></span>
<span data-ttu-id="022e7-165">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="022e7-165">If successful, this method returns a `201 Created` response code and a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="022e7-166">示例</span><span class="sxs-lookup"><span data-stu-id="022e7-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="022e7-167">请求</span><span class="sxs-lookup"><span data-stu-id="022e7-167">Request</span></span>
<span data-ttu-id="022e7-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="022e7-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="022e7-169">响应</span><span class="sxs-lookup"><span data-stu-id="022e7-169">Response</span></span>
<span data-ttu-id="022e7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="022e7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




