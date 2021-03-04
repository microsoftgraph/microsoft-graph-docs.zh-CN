---
title: 更新 windowsUpdateState
description: 更新 windowsUpdateState 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6505707c957ad890d07c9d418512b41e09ff5109
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443795"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="825e9-103">更新 windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="825e9-103">Update windowsUpdateState</span></span>

<span data-ttu-id="825e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="825e9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="825e9-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="825e9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="825e9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="825e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="825e9-107">更新 [windowsUpdateState 对象](../resources/intune-shared-windowsupdatestate.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="825e9-107">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="825e9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="825e9-108">Prerequisites</span></span>
<span data-ttu-id="825e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="825e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="825e9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="825e9-111">Permission type</span></span>|<span data-ttu-id="825e9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="825e9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="825e9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="825e9-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="825e9-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="825e9-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="825e9-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="825e9-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="825e9-116">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="825e9-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="825e9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="825e9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="825e9-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="825e9-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="825e9-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="825e9-119">Not supported.</span></span>|
|<span data-ttu-id="825e9-120">Application</span><span class="sxs-lookup"><span data-stu-id="825e9-120">Application</span></span>||
| <span data-ttu-id="825e9-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="825e9-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="825e9-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="825e9-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="825e9-123">&nbsp;&nbsp;**软件更新**</span><span class="sxs-lookup"><span data-stu-id="825e9-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="825e9-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="825e9-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="825e9-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="825e9-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="825e9-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="825e9-126">Request headers</span></span>
|<span data-ttu-id="825e9-127">标头</span><span class="sxs-lookup"><span data-stu-id="825e9-127">Header</span></span>|<span data-ttu-id="825e9-128">值</span><span class="sxs-lookup"><span data-stu-id="825e9-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="825e9-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="825e9-129">Authorization</span></span>|<span data-ttu-id="825e9-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="825e9-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="825e9-131">接受</span><span class="sxs-lookup"><span data-stu-id="825e9-131">Accept</span></span>|<span data-ttu-id="825e9-132">application/json</span><span class="sxs-lookup"><span data-stu-id="825e9-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="825e9-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="825e9-133">Request body</span></span>
<span data-ttu-id="825e9-134">在请求正文中，提供 [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="825e9-134">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="825e9-135">下表显示创建 [windowsUpdateState 时所需的属性](../resources/intune-shared-windowsupdatestate.md)。</span><span class="sxs-lookup"><span data-stu-id="825e9-135">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="825e9-136">属性</span><span class="sxs-lookup"><span data-stu-id="825e9-136">Property</span></span>|<span data-ttu-id="825e9-137">类型</span><span class="sxs-lookup"><span data-stu-id="825e9-137">Type</span></span>|<span data-ttu-id="825e9-138">说明</span><span class="sxs-lookup"><span data-stu-id="825e9-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="825e9-139">id</span><span class="sxs-lookup"><span data-stu-id="825e9-139">id</span></span>|<span data-ttu-id="825e9-140">String</span><span class="sxs-lookup"><span data-stu-id="825e9-140">String</span></span>|<span data-ttu-id="825e9-141">这是实体的 ID。</span><span class="sxs-lookup"><span data-stu-id="825e9-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="825e9-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="825e9-142">deviceId</span></span>|<span data-ttu-id="825e9-143">String</span><span class="sxs-lookup"><span data-stu-id="825e9-143">String</span></span>|<span data-ttu-id="825e9-144">设备的 ID。</span><span class="sxs-lookup"><span data-stu-id="825e9-144">The id of the device.</span></span>|
|<span data-ttu-id="825e9-145">userId</span><span class="sxs-lookup"><span data-stu-id="825e9-145">userId</span></span>|<span data-ttu-id="825e9-146">String</span><span class="sxs-lookup"><span data-stu-id="825e9-146">String</span></span>|<span data-ttu-id="825e9-147">用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="825e9-147">The id of the user.</span></span>|
|<span data-ttu-id="825e9-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="825e9-148">deviceDisplayName</span></span>|<span data-ttu-id="825e9-149">String</span><span class="sxs-lookup"><span data-stu-id="825e9-149">String</span></span>|<span data-ttu-id="825e9-150">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="825e9-150">Device display name.</span></span>|
|<span data-ttu-id="825e9-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="825e9-151">userPrincipalName</span></span>|<span data-ttu-id="825e9-152">String</span><span class="sxs-lookup"><span data-stu-id="825e9-152">String</span></span>|<span data-ttu-id="825e9-153">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="825e9-153">User principal name.</span></span>|
|<span data-ttu-id="825e9-154">status</span><span class="sxs-lookup"><span data-stu-id="825e9-154">status</span></span>|[<span data-ttu-id="825e9-155">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="825e9-155">windowsUpdateStatus</span></span>](../resources/intune-shared-windowsupdatestatus.md)|<span data-ttu-id="825e9-156">Windows udpate 状态。</span><span class="sxs-lookup"><span data-stu-id="825e9-156">Windows udpate status.</span></span> <span data-ttu-id="825e9-157">可取值为：`upToDate`、`pendingInstallation`、`pendingReboot`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="825e9-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="825e9-158">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="825e9-158">qualityUpdateVersion</span></span>|<span data-ttu-id="825e9-159">String</span><span class="sxs-lookup"><span data-stu-id="825e9-159">String</span></span>|<span data-ttu-id="825e9-160">设备的质量更新版本。</span><span class="sxs-lookup"><span data-stu-id="825e9-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="825e9-161">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="825e9-161">featureUpdateVersion</span></span>|<span data-ttu-id="825e9-162">String</span><span class="sxs-lookup"><span data-stu-id="825e9-162">String</span></span>|<span data-ttu-id="825e9-163">设备的当前功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="825e9-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="825e9-164">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="825e9-164">lastScanDateTime</span></span>|<span data-ttu-id="825e9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="825e9-165">DateTimeOffset</span></span>|<span data-ttu-id="825e9-166">Windows 更新代理成功扫描的日期时间。</span><span class="sxs-lookup"><span data-stu-id="825e9-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="825e9-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="825e9-167">lastSyncDateTime</span></span>|<span data-ttu-id="825e9-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="825e9-168">DateTimeOffset</span></span>|<span data-ttu-id="825e9-169">设备上次与 Microsoft Intune 同步的日期时间。</span><span class="sxs-lookup"><span data-stu-id="825e9-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="825e9-170">响应</span><span class="sxs-lookup"><span data-stu-id="825e9-170">Response</span></span>
<span data-ttu-id="825e9-171">如果成功，此方法在响应正文中返回响应代码和更新 `200 OK` 的 [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="825e9-171">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="825e9-172">示例</span><span class="sxs-lookup"><span data-stu-id="825e9-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="825e9-173">请求</span><span class="sxs-lookup"><span data-stu-id="825e9-173">Request</span></span>
<span data-ttu-id="825e9-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="825e9-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
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

### <a name="response"></a><span data-ttu-id="825e9-175">响应</span><span class="sxs-lookup"><span data-stu-id="825e9-175">Response</span></span>
<span data-ttu-id="825e9-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="825e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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







