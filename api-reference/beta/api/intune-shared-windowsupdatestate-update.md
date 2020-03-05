---
title: 更新 windowsUpdateState
description: 更新 windowsUpdateState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1da79ffe24542b8989ea6673a1c469447a1f64fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457901"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="44e95-103">更新 windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="44e95-103">Update windowsUpdateState</span></span>

<span data-ttu-id="44e95-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="44e95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44e95-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44e95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44e95-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44e95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44e95-107">更新[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="44e95-107">Update the properties of a [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44e95-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="44e95-108">Prerequisites</span></span>
<span data-ttu-id="44e95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44e95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44e95-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="44e95-111">Permission type</span></span>|<span data-ttu-id="44e95-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="44e95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44e95-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44e95-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="44e95-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="44e95-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="44e95-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e95-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="44e95-116">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="44e95-116">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="44e95-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e95-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="44e95-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44e95-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44e95-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="44e95-119">Not supported.</span></span>|
|<span data-ttu-id="44e95-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="44e95-120">Application</span></span>||
| <span data-ttu-id="44e95-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="44e95-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="44e95-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e95-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="44e95-123">&nbsp;&nbsp; **软件更新**</span><span class="sxs-lookup"><span data-stu-id="44e95-123">&nbsp; &nbsp; **Software Update**</span></span> | <span data-ttu-id="44e95-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44e95-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44e95-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44e95-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="44e95-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="44e95-126">Request headers</span></span>
|<span data-ttu-id="44e95-127">标头</span><span class="sxs-lookup"><span data-stu-id="44e95-127">Header</span></span>|<span data-ttu-id="44e95-128">值</span><span class="sxs-lookup"><span data-stu-id="44e95-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44e95-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="44e95-129">Authorization</span></span>|<span data-ttu-id="44e95-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="44e95-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44e95-131">接受</span><span class="sxs-lookup"><span data-stu-id="44e95-131">Accept</span></span>|<span data-ttu-id="44e95-132">application/json</span><span class="sxs-lookup"><span data-stu-id="44e95-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44e95-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="44e95-133">Request body</span></span>
<span data-ttu-id="44e95-134">在请求正文中，提供[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44e95-134">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="44e95-135">下表显示创建[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="44e95-135">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md).</span></span>

|<span data-ttu-id="44e95-136">属性</span><span class="sxs-lookup"><span data-stu-id="44e95-136">Property</span></span>|<span data-ttu-id="44e95-137">类型</span><span class="sxs-lookup"><span data-stu-id="44e95-137">Type</span></span>|<span data-ttu-id="44e95-138">说明</span><span class="sxs-lookup"><span data-stu-id="44e95-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44e95-139">id</span><span class="sxs-lookup"><span data-stu-id="44e95-139">id</span></span>|<span data-ttu-id="44e95-140">String</span><span class="sxs-lookup"><span data-stu-id="44e95-140">String</span></span>|<span data-ttu-id="44e95-141">这是实体的 Id。</span><span class="sxs-lookup"><span data-stu-id="44e95-141">This is Id of the entity.</span></span>|
|<span data-ttu-id="44e95-142">deviceId</span><span class="sxs-lookup"><span data-stu-id="44e95-142">deviceId</span></span>|<span data-ttu-id="44e95-143">String</span><span class="sxs-lookup"><span data-stu-id="44e95-143">String</span></span>|<span data-ttu-id="44e95-144">设备的 id。</span><span class="sxs-lookup"><span data-stu-id="44e95-144">The id of the device.</span></span>|
|<span data-ttu-id="44e95-145">userId</span><span class="sxs-lookup"><span data-stu-id="44e95-145">userId</span></span>|<span data-ttu-id="44e95-146">String</span><span class="sxs-lookup"><span data-stu-id="44e95-146">String</span></span>|<span data-ttu-id="44e95-147">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="44e95-147">The id of the user.</span></span>|
|<span data-ttu-id="44e95-148">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="44e95-148">deviceDisplayName</span></span>|<span data-ttu-id="44e95-149">String</span><span class="sxs-lookup"><span data-stu-id="44e95-149">String</span></span>|<span data-ttu-id="44e95-150">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="44e95-150">Device display name.</span></span>|
|<span data-ttu-id="44e95-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="44e95-151">userPrincipalName</span></span>|<span data-ttu-id="44e95-152">字符串</span><span class="sxs-lookup"><span data-stu-id="44e95-152">String</span></span>|<span data-ttu-id="44e95-153">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="44e95-153">User principal name.</span></span>|
|<span data-ttu-id="44e95-154">status</span><span class="sxs-lookup"><span data-stu-id="44e95-154">status</span></span>|[<span data-ttu-id="44e95-155">windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="44e95-155">windowsUpdateState</span></span>](../resources/intune-shared-windowsupdatestate.md)|<span data-ttu-id="44e95-156">Windows udpate 状态。</span><span class="sxs-lookup"><span data-stu-id="44e95-156">Windows udpate status.</span></span> <span data-ttu-id="44e95-157">可取值为：`upToDate`、`pendingInstallation`、`pendingReboot`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="44e95-157">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="44e95-158">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="44e95-158">qualityUpdateVersion</span></span>|<span data-ttu-id="44e95-159">String</span><span class="sxs-lookup"><span data-stu-id="44e95-159">String</span></span>|<span data-ttu-id="44e95-160">设备的质量更新版本。</span><span class="sxs-lookup"><span data-stu-id="44e95-160">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="44e95-161">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="44e95-161">featureUpdateVersion</span></span>|<span data-ttu-id="44e95-162">String</span><span class="sxs-lookup"><span data-stu-id="44e95-162">String</span></span>|<span data-ttu-id="44e95-163">设备的当前功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="44e95-163">The current feature update version of the device.</span></span>|
|<span data-ttu-id="44e95-164">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="44e95-164">lastScanDateTime</span></span>|<span data-ttu-id="44e95-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44e95-165">DateTimeOffset</span></span>|<span data-ttu-id="44e95-166">Windows Update 代理成功扫描的日期时间。</span><span class="sxs-lookup"><span data-stu-id="44e95-166">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="44e95-167">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="44e95-167">lastSyncDateTime</span></span>|<span data-ttu-id="44e95-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44e95-168">DateTimeOffset</span></span>|<span data-ttu-id="44e95-169">上次与 Microsoft Intune 同步设备的日期时间。</span><span class="sxs-lookup"><span data-stu-id="44e95-169">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="44e95-170">响应</span><span class="sxs-lookup"><span data-stu-id="44e95-170">Response</span></span>
<span data-ttu-id="44e95-171">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="44e95-171">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44e95-172">示例</span><span class="sxs-lookup"><span data-stu-id="44e95-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="44e95-173">请求</span><span class="sxs-lookup"><span data-stu-id="44e95-173">Request</span></span>
<span data-ttu-id="44e95-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44e95-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44e95-175">响应</span><span class="sxs-lookup"><span data-stu-id="44e95-175">Response</span></span>
<span data-ttu-id="44e95-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="44e95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








