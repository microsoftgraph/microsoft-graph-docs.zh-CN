---
title: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 16d8addb2a23d3a4eb75b7178a1e67b7f0889c42
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209848"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="0dbf4-103">更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="0dbf4-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

<span data-ttu-id="0dbf4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dbf4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dbf4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dbf4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dbf4-107">更新 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-107">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0dbf4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0dbf4-108">Prerequisites</span></span>
<span data-ttu-id="0dbf4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dbf4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0dbf4-111">Permission type</span></span>|<span data-ttu-id="0dbf4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0dbf4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dbf4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0dbf4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0dbf4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dbf4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0dbf4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0dbf4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dbf4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-116">Not supported.</span></span>|
|<span data-ttu-id="0dbf4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0dbf4-117">Application</span></span>|<span data-ttu-id="0dbf4-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dbf4-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dbf4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0dbf4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="0dbf4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0dbf4-120">Request headers</span></span>
|<span data-ttu-id="0dbf4-121">标头</span><span class="sxs-lookup"><span data-stu-id="0dbf4-121">Header</span></span>|<span data-ttu-id="0dbf4-122">值</span><span class="sxs-lookup"><span data-stu-id="0dbf4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dbf4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dbf4-123">Authorization</span></span>|<span data-ttu-id="0dbf4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dbf4-125">接受</span><span class="sxs-lookup"><span data-stu-id="0dbf4-125">Accept</span></span>|<span data-ttu-id="0dbf4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0dbf4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dbf4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0dbf4-127">Request body</span></span>
<span data-ttu-id="0dbf4-128">在请求正文中，提供 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-128">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

<span data-ttu-id="0dbf4-129">下表显示创建 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-129">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).</span></span>

|<span data-ttu-id="0dbf4-130">属性</span><span class="sxs-lookup"><span data-stu-id="0dbf4-130">Property</span></span>|<span data-ttu-id="0dbf4-131">类型</span><span class="sxs-lookup"><span data-stu-id="0dbf4-131">Type</span></span>|<span data-ttu-id="0dbf4-132">说明</span><span class="sxs-lookup"><span data-stu-id="0dbf4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dbf4-133">id</span><span class="sxs-lookup"><span data-stu-id="0dbf4-133">id</span></span>|<span data-ttu-id="0dbf4-134">String</span><span class="sxs-lookup"><span data-stu-id="0dbf4-134">String</span></span>|<span data-ttu-id="0dbf4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-135">Key of the entity.</span></span>|
|<span data-ttu-id="0dbf4-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="0dbf4-136">deviceName</span></span>|<span data-ttu-id="0dbf4-137">String</span><span class="sxs-lookup"><span data-stu-id="0dbf4-137">String</span></span>|<span data-ttu-id="0dbf4-138">设备名称。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-138">Device name.</span></span>|
|<span data-ttu-id="0dbf4-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="0dbf4-139">deviceId</span></span>|<span data-ttu-id="0dbf4-140">String</span><span class="sxs-lookup"><span data-stu-id="0dbf4-140">String</span></span>|<span data-ttu-id="0dbf4-141">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-141">Device ID.</span></span>|
|<span data-ttu-id="0dbf4-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0dbf4-142">lastSyncDateTime</span></span>|<span data-ttu-id="0dbf4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dbf4-143">DateTimeOffset</span></span>|<span data-ttu-id="0dbf4-144">上次同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-144">Last sync date time.</span></span>|
|<span data-ttu-id="0dbf4-145">osVersion</span><span class="sxs-lookup"><span data-stu-id="0dbf4-145">osVersion</span></span>|<span data-ttu-id="0dbf4-146">String</span><span class="sxs-lookup"><span data-stu-id="0dbf4-146">String</span></span>|<span data-ttu-id="0dbf4-147">Windows OS 版本。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-147">Windows OS Version.</span></span>|
|<span data-ttu-id="0dbf4-148">osDescription</span><span class="sxs-lookup"><span data-stu-id="0dbf4-148">osDescription</span></span>|<span data-ttu-id="0dbf4-149">String</span><span class="sxs-lookup"><span data-stu-id="0dbf4-149">String</span></span>|<span data-ttu-id="0dbf4-150">Windows OS 版本说明。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-150">Windows OS Version Description.</span></span>|
|<span data-ttu-id="0dbf4-151">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="0dbf4-151">deploymentStatus</span></span>|[<span data-ttu-id="0dbf4-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="0dbf4-152">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="0dbf4-153">策略的部署状态。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-153">The deployment state of the policy.</span></span> <span data-ttu-id="0dbf4-154">可取值为：`unknown`、`success`、`tokenError`、`notAuthorizedByToken`、`policyNotFound`。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-154">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="0dbf4-155">userName</span><span class="sxs-lookup"><span data-stu-id="0dbf4-155">userName</span></span>|<span data-ttu-id="0dbf4-156">String</span><span class="sxs-lookup"><span data-stu-id="0dbf4-156">String</span></span>|<span data-ttu-id="0dbf4-157">此设备的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-157">The name of the user of this device.</span></span>|
|<span data-ttu-id="0dbf4-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0dbf4-158">userPrincipalName</span></span>|<span data-ttu-id="0dbf4-159">String</span><span class="sxs-lookup"><span data-stu-id="0dbf4-159">String</span></span>|<span data-ttu-id="0dbf4-160">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-160">User Principal Name.</span></span>|
|<span data-ttu-id="0dbf4-161">policyVersion</span><span class="sxs-lookup"><span data-stu-id="0dbf4-161">policyVersion</span></span>|<span data-ttu-id="0dbf4-162">String</span><span class="sxs-lookup"><span data-stu-id="0dbf4-162">String</span></span>|<span data-ttu-id="0dbf4-163">WindowsDefenderApplicationControl 补充策略的人工可读版本。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-163">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="0dbf4-164">响应</span><span class="sxs-lookup"><span data-stu-id="0dbf4-164">Response</span></span>
<span data-ttu-id="0dbf4-165">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-165">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dbf4-166">示例</span><span class="sxs-lookup"><span data-stu-id="0dbf4-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="0dbf4-167">请求</span><span class="sxs-lookup"><span data-stu-id="0dbf4-167">Request</span></span>
<span data-ttu-id="0dbf4-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0dbf4-169">响应</span><span class="sxs-lookup"><span data-stu-id="0dbf4-169">Response</span></span>
<span data-ttu-id="0dbf4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0dbf4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




