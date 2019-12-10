---
title: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: 更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a16cd0541aea74ffa683a6a8cdf5f7779a993778
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39938696"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a><span data-ttu-id="895ce-103">更新 windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="895ce-103">Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus</span></span>

> <span data-ttu-id="895ce-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="895ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="895ce-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="895ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="895ce-106">更新[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="895ce-106">Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="895ce-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="895ce-107">Prerequisites</span></span>
<span data-ttu-id="895ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="895ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="895ce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="895ce-110">Permission type</span></span>|<span data-ttu-id="895ce-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="895ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="895ce-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="895ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="895ce-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="895ce-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="895ce-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="895ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="895ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="895ce-115">Not supported.</span></span>|
|<span data-ttu-id="895ce-116">Application</span><span class="sxs-lookup"><span data-stu-id="895ce-116">Application</span></span>|<span data-ttu-id="895ce-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="895ce-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="895ce-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="895ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="895ce-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="895ce-119">Request headers</span></span>
|<span data-ttu-id="895ce-120">标头</span><span class="sxs-lookup"><span data-stu-id="895ce-120">Header</span></span>|<span data-ttu-id="895ce-121">值</span><span class="sxs-lookup"><span data-stu-id="895ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="895ce-122">授权</span><span class="sxs-lookup"><span data-stu-id="895ce-122">Authorization</span></span>|<span data-ttu-id="895ce-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="895ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="895ce-124">接受</span><span class="sxs-lookup"><span data-stu-id="895ce-124">Accept</span></span>|<span data-ttu-id="895ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="895ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="895ce-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="895ce-126">Request body</span></span>
<span data-ttu-id="895ce-127">在请求正文中，提供[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="895ce-127">In the request body, supply a JSON representation for the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.</span></span>

<span data-ttu-id="895ce-128">下表显示创建[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="895ce-128">The following table shows the properties that are required when you create the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).</span></span>

|<span data-ttu-id="895ce-129">属性</span><span class="sxs-lookup"><span data-stu-id="895ce-129">Property</span></span>|<span data-ttu-id="895ce-130">类型</span><span class="sxs-lookup"><span data-stu-id="895ce-130">Type</span></span>|<span data-ttu-id="895ce-131">说明</span><span class="sxs-lookup"><span data-stu-id="895ce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="895ce-132">id</span><span class="sxs-lookup"><span data-stu-id="895ce-132">id</span></span>|<span data-ttu-id="895ce-133">String</span><span class="sxs-lookup"><span data-stu-id="895ce-133">String</span></span>|<span data-ttu-id="895ce-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="895ce-134">Key of the entity.</span></span>|
|<span data-ttu-id="895ce-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="895ce-135">deviceName</span></span>|<span data-ttu-id="895ce-136">String</span><span class="sxs-lookup"><span data-stu-id="895ce-136">String</span></span>|<span data-ttu-id="895ce-137">设备名称。</span><span class="sxs-lookup"><span data-stu-id="895ce-137">Device name.</span></span>|
|<span data-ttu-id="895ce-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="895ce-138">deviceId</span></span>|<span data-ttu-id="895ce-139">字符串</span><span class="sxs-lookup"><span data-stu-id="895ce-139">String</span></span>|<span data-ttu-id="895ce-140">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="895ce-140">Device ID.</span></span>|
|<span data-ttu-id="895ce-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="895ce-141">lastSyncDateTime</span></span>|<span data-ttu-id="895ce-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="895ce-142">DateTimeOffset</span></span>|<span data-ttu-id="895ce-143">上次同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="895ce-143">Last sync date time.</span></span>|
|<span data-ttu-id="895ce-144">osVersion</span><span class="sxs-lookup"><span data-stu-id="895ce-144">osVersion</span></span>|<span data-ttu-id="895ce-145">字符串</span><span class="sxs-lookup"><span data-stu-id="895ce-145">String</span></span>|<span data-ttu-id="895ce-146">Windows OS 版本。</span><span class="sxs-lookup"><span data-stu-id="895ce-146">Windows OS Version.</span></span>|
|<span data-ttu-id="895ce-147">osDescription</span><span class="sxs-lookup"><span data-stu-id="895ce-147">osDescription</span></span>|<span data-ttu-id="895ce-148">字符串</span><span class="sxs-lookup"><span data-stu-id="895ce-148">String</span></span>|<span data-ttu-id="895ce-149">Windows OS 版本说明。</span><span class="sxs-lookup"><span data-stu-id="895ce-149">Windows OS Version Description.</span></span>|
|<span data-ttu-id="895ce-150">deploymentStatus</span><span class="sxs-lookup"><span data-stu-id="895ce-150">deploymentStatus</span></span>|[<span data-ttu-id="895ce-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span><span class="sxs-lookup"><span data-stu-id="895ce-151">windowsDefenderApplicationControlSupplementalPolicyStatuses</span></span>](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|<span data-ttu-id="895ce-152">策略的部署状态。</span><span class="sxs-lookup"><span data-stu-id="895ce-152">The deployment state of the policy.</span></span> <span data-ttu-id="895ce-153">可取值为：`unknown`、`success`、`tokenError`、`notAuthorizedByToken`、`policyNotFound`。</span><span class="sxs-lookup"><span data-stu-id="895ce-153">Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.</span></span>|
|<span data-ttu-id="895ce-154">userName</span><span class="sxs-lookup"><span data-stu-id="895ce-154">userName</span></span>|<span data-ttu-id="895ce-155">String</span><span class="sxs-lookup"><span data-stu-id="895ce-155">String</span></span>|<span data-ttu-id="895ce-156">此设备的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="895ce-156">The name of the user of this device.</span></span>|
|<span data-ttu-id="895ce-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="895ce-157">userPrincipalName</span></span>|<span data-ttu-id="895ce-158">字符串</span><span class="sxs-lookup"><span data-stu-id="895ce-158">String</span></span>|<span data-ttu-id="895ce-159">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="895ce-159">User Principal Name.</span></span>|
|<span data-ttu-id="895ce-160">policyVersion</span><span class="sxs-lookup"><span data-stu-id="895ce-160">policyVersion</span></span>|<span data-ttu-id="895ce-161">字符串</span><span class="sxs-lookup"><span data-stu-id="895ce-161">String</span></span>|<span data-ttu-id="895ce-162">WindowsDefenderApplicationControl 补充策略的人工可读版本。</span><span class="sxs-lookup"><span data-stu-id="895ce-162">Human readable version of the WindowsDefenderApplicationControl supplemental policy.</span></span>|



## <a name="response"></a><span data-ttu-id="895ce-163">响应</span><span class="sxs-lookup"><span data-stu-id="895ce-163">Response</span></span>
<span data-ttu-id="895ce-164">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="895ce-164">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="895ce-165">示例</span><span class="sxs-lookup"><span data-stu-id="895ce-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="895ce-166">请求</span><span class="sxs-lookup"><span data-stu-id="895ce-166">Request</span></span>
<span data-ttu-id="895ce-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="895ce-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="895ce-168">响应</span><span class="sxs-lookup"><span data-stu-id="895ce-168">Response</span></span>
<span data-ttu-id="895ce-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="895ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





