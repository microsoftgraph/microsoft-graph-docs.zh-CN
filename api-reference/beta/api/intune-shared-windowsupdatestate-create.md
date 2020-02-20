---
title: 创建 windowsUpdateState
description: 创建新的 windowsUpdateState 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b6ad2081039a6bc6cf21259e2e6ffb4418637cd
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159883"
---
# <a name="create-windowsupdatestate"></a><span data-ttu-id="3bc54-103">创建 windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="3bc54-103">Create windowsUpdateState</span></span>

> <span data-ttu-id="3bc54-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3bc54-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bc54-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3bc54-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bc54-106">创建新的[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3bc54-106">Create a new [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bc54-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3bc54-107">Prerequisites</span></span>
<span data-ttu-id="3bc54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bc54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bc54-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bc54-110">Permission type</span></span>|<span data-ttu-id="3bc54-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3bc54-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bc54-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bc54-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3bc54-113">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="3bc54-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3bc54-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc54-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="3bc54-115">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="3bc54-115">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="3bc54-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc54-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3bc54-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bc54-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bc54-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bc54-118">Not supported.</span></span>|
|<span data-ttu-id="3bc54-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="3bc54-119">Application</span></span>||
| <span data-ttu-id="3bc54-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="3bc54-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="3bc54-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc54-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="3bc54-122">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="3bc54-122">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="3bc54-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bc54-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bc54-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bc54-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
```

## <a name="request-headers"></a><span data-ttu-id="3bc54-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bc54-125">Request headers</span></span>
|<span data-ttu-id="3bc54-126">标头</span><span class="sxs-lookup"><span data-stu-id="3bc54-126">Header</span></span>|<span data-ttu-id="3bc54-127">值</span><span class="sxs-lookup"><span data-stu-id="3bc54-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bc54-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bc54-128">Authorization</span></span>|<span data-ttu-id="3bc54-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3bc54-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bc54-130">接受</span><span class="sxs-lookup"><span data-stu-id="3bc54-130">Accept</span></span>|<span data-ttu-id="3bc54-131">application/json</span><span class="sxs-lookup"><span data-stu-id="3bc54-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bc54-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bc54-132">Request body</span></span>
<span data-ttu-id="3bc54-133">在请求正文中，提供 windowsUpdateState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bc54-133">In the request body, supply a JSON representation for the windowsUpdateState object.</span></span>

<span data-ttu-id="3bc54-134">下表显示创建 windowsUpdateState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3bc54-134">The following table shows the properties that are required when you create the windowsUpdateState.</span></span>

|<span data-ttu-id="3bc54-135">属性</span><span class="sxs-lookup"><span data-stu-id="3bc54-135">Property</span></span>|<span data-ttu-id="3bc54-136">类型</span><span class="sxs-lookup"><span data-stu-id="3bc54-136">Type</span></span>|<span data-ttu-id="3bc54-137">说明</span><span class="sxs-lookup"><span data-stu-id="3bc54-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bc54-138">id</span><span class="sxs-lookup"><span data-stu-id="3bc54-138">id</span></span>|<span data-ttu-id="3bc54-139">String</span><span class="sxs-lookup"><span data-stu-id="3bc54-139">String</span></span>|<span data-ttu-id="3bc54-140">这是实体的 Id。</span><span class="sxs-lookup"><span data-stu-id="3bc54-140">This is Id of the entity.</span></span>|
|<span data-ttu-id="3bc54-141">deviceId</span><span class="sxs-lookup"><span data-stu-id="3bc54-141">deviceId</span></span>|<span data-ttu-id="3bc54-142">String</span><span class="sxs-lookup"><span data-stu-id="3bc54-142">String</span></span>|<span data-ttu-id="3bc54-143">设备的 id。</span><span class="sxs-lookup"><span data-stu-id="3bc54-143">The id of the device.</span></span>|
|<span data-ttu-id="3bc54-144">userId</span><span class="sxs-lookup"><span data-stu-id="3bc54-144">userId</span></span>|<span data-ttu-id="3bc54-145">String</span><span class="sxs-lookup"><span data-stu-id="3bc54-145">String</span></span>|<span data-ttu-id="3bc54-146">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="3bc54-146">The id of the user.</span></span>|
|<span data-ttu-id="3bc54-147">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3bc54-147">deviceDisplayName</span></span>|<span data-ttu-id="3bc54-148">String</span><span class="sxs-lookup"><span data-stu-id="3bc54-148">String</span></span>|<span data-ttu-id="3bc54-149">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="3bc54-149">Device display name.</span></span>|
|<span data-ttu-id="3bc54-150">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3bc54-150">userPrincipalName</span></span>|<span data-ttu-id="3bc54-151">字符串</span><span class="sxs-lookup"><span data-stu-id="3bc54-151">String</span></span>|<span data-ttu-id="3bc54-152">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="3bc54-152">User principal name.</span></span>|
|<span data-ttu-id="3bc54-153">status</span><span class="sxs-lookup"><span data-stu-id="3bc54-153">status</span></span>|[<span data-ttu-id="3bc54-154">windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="3bc54-154">windowsUpdateState</span></span>](../resources/intune-shared-windowsupdatestate.md)|<span data-ttu-id="3bc54-155">Windows udpate 状态。</span><span class="sxs-lookup"><span data-stu-id="3bc54-155">Windows udpate status.</span></span> <span data-ttu-id="3bc54-156">可取值为：`upToDate`、`pendingInstallation`、`pendingReboot`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="3bc54-156">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="3bc54-157">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="3bc54-157">qualityUpdateVersion</span></span>|<span data-ttu-id="3bc54-158">String</span><span class="sxs-lookup"><span data-stu-id="3bc54-158">String</span></span>|<span data-ttu-id="3bc54-159">设备的质量更新版本。</span><span class="sxs-lookup"><span data-stu-id="3bc54-159">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="3bc54-160">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="3bc54-160">featureUpdateVersion</span></span>|<span data-ttu-id="3bc54-161">String</span><span class="sxs-lookup"><span data-stu-id="3bc54-161">String</span></span>|<span data-ttu-id="3bc54-162">设备的当前功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="3bc54-162">The current feature update version of the device.</span></span>|
|<span data-ttu-id="3bc54-163">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="3bc54-163">lastScanDateTime</span></span>|<span data-ttu-id="3bc54-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bc54-164">DateTimeOffset</span></span>|<span data-ttu-id="3bc54-165">Windows Update 代理成功扫描的日期时间。</span><span class="sxs-lookup"><span data-stu-id="3bc54-165">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="3bc54-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3bc54-166">lastSyncDateTime</span></span>|<span data-ttu-id="3bc54-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bc54-167">DateTimeOffset</span></span>|<span data-ttu-id="3bc54-168">上次与 Microsoft Intune 同步设备的日期时间。</span><span class="sxs-lookup"><span data-stu-id="3bc54-168">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="3bc54-169">响应</span><span class="sxs-lookup"><span data-stu-id="3bc54-169">Response</span></span>
<span data-ttu-id="3bc54-170">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3bc54-170">If successful, this method returns a `201 Created` response code and a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bc54-171">示例</span><span class="sxs-lookup"><span data-stu-id="3bc54-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bc54-172">请求</span><span class="sxs-lookup"><span data-stu-id="3bc54-172">Request</span></span>
<span data-ttu-id="3bc54-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3bc54-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="3bc54-174">响应</span><span class="sxs-lookup"><span data-stu-id="3bc54-174">Response</span></span>
<span data-ttu-id="3bc54-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3bc54-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "3d92af00-af00-3d92-00af-923d00af923d",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userPrincipalName": "User Principal Name value",
  "status": "pendingInstallation",
  "qualityUpdateVersion": "Quality Update Version value",
  "featureUpdateVersion": "Feature Update Version value",
  "lastScanDateTime": "2016-12-31T23:59:18.0955018-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```








