---
title: 更新 windowsUpdateState
description: 更新 windowsUpdateState 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 35a56a0dea3174a7f196a3cee62a46edd35eafce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344131"
---
# <a name="update-windowsupdatestate"></a><span data-ttu-id="36477-103">更新 windowsUpdateState</span><span class="sxs-lookup"><span data-stu-id="36477-103">Update windowsUpdateState</span></span>

> <span data-ttu-id="36477-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="36477-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36477-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="36477-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36477-106">更新[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="36477-106">Update the properties of a [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36477-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="36477-107">Prerequisites</span></span>
<span data-ttu-id="36477-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36477-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="36477-110">Permission type</span></span>|<span data-ttu-id="36477-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="36477-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36477-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36477-112">Delegated (work or school account)</span></span>|<span data-ttu-id="36477-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36477-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="36477-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36477-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36477-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="36477-115">Not supported.</span></span>|
|<span data-ttu-id="36477-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="36477-116">Application</span></span>|<span data-ttu-id="36477-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36477-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36477-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36477-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsUpdateForBusinessConfiguration/deviceUpdateStates/{windowsUpdateStateId}
```

## <a name="request-headers"></a><span data-ttu-id="36477-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="36477-119">Request headers</span></span>
|<span data-ttu-id="36477-120">标头</span><span class="sxs-lookup"><span data-stu-id="36477-120">Header</span></span>|<span data-ttu-id="36477-121">值</span><span class="sxs-lookup"><span data-stu-id="36477-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36477-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="36477-122">Authorization</span></span>|<span data-ttu-id="36477-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="36477-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36477-124">接受</span><span class="sxs-lookup"><span data-stu-id="36477-124">Accept</span></span>|<span data-ttu-id="36477-125">application/json</span><span class="sxs-lookup"><span data-stu-id="36477-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36477-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="36477-126">Request body</span></span>
<span data-ttu-id="36477-127">在请求正文中, 提供[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="36477-127">In the request body, supply a JSON representation for the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object.</span></span>

<span data-ttu-id="36477-128">下表显示创建[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="36477-128">The following table shows the properties that are required when you create the [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md).</span></span>

|<span data-ttu-id="36477-129">属性</span><span class="sxs-lookup"><span data-stu-id="36477-129">Property</span></span>|<span data-ttu-id="36477-130">类型</span><span class="sxs-lookup"><span data-stu-id="36477-130">Type</span></span>|<span data-ttu-id="36477-131">说明</span><span class="sxs-lookup"><span data-stu-id="36477-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36477-132">id</span><span class="sxs-lookup"><span data-stu-id="36477-132">id</span></span>|<span data-ttu-id="36477-133">String</span><span class="sxs-lookup"><span data-stu-id="36477-133">String</span></span>|<span data-ttu-id="36477-134">这是实体的 Id。</span><span class="sxs-lookup"><span data-stu-id="36477-134">This is Id of the entity.</span></span>|
|<span data-ttu-id="36477-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="36477-135">deviceId</span></span>|<span data-ttu-id="36477-136">String</span><span class="sxs-lookup"><span data-stu-id="36477-136">String</span></span>|<span data-ttu-id="36477-137">设备的 id。</span><span class="sxs-lookup"><span data-stu-id="36477-137">The id of the device.</span></span>|
|<span data-ttu-id="36477-138">userId</span><span class="sxs-lookup"><span data-stu-id="36477-138">userId</span></span>|<span data-ttu-id="36477-139">String</span><span class="sxs-lookup"><span data-stu-id="36477-139">String</span></span>|<span data-ttu-id="36477-140">用户的 id。</span><span class="sxs-lookup"><span data-stu-id="36477-140">The id of the user.</span></span>|
|<span data-ttu-id="36477-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="36477-141">deviceDisplayName</span></span>|<span data-ttu-id="36477-142">String</span><span class="sxs-lookup"><span data-stu-id="36477-142">String</span></span>|<span data-ttu-id="36477-143">设备显示名称。</span><span class="sxs-lookup"><span data-stu-id="36477-143">Device display name.</span></span>|
|<span data-ttu-id="36477-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="36477-144">userPrincipalName</span></span>|<span data-ttu-id="36477-145">字符串</span><span class="sxs-lookup"><span data-stu-id="36477-145">String</span></span>|<span data-ttu-id="36477-146">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="36477-146">User principal name.</span></span>|
|<span data-ttu-id="36477-147">status</span><span class="sxs-lookup"><span data-stu-id="36477-147">status</span></span>|[<span data-ttu-id="36477-148">windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="36477-148">windowsUpdateStatus</span></span>](../resources/intune-deviceconfig-windowsupdatestatus.md)|<span data-ttu-id="36477-149">Windows udpate 状态。</span><span class="sxs-lookup"><span data-stu-id="36477-149">Windows udpate status.</span></span> <span data-ttu-id="36477-150">可取值为：`upToDate`、`pendingInstallation`、`pendingReboot`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="36477-150">Possible values are: `upToDate`, `pendingInstallation`, `pendingReboot`, `failed`.</span></span>|
|<span data-ttu-id="36477-151">qualityUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="36477-151">qualityUpdateVersion</span></span>|<span data-ttu-id="36477-152">String</span><span class="sxs-lookup"><span data-stu-id="36477-152">String</span></span>|<span data-ttu-id="36477-153">设备的质量更新版本。</span><span class="sxs-lookup"><span data-stu-id="36477-153">The Quality Update Version of the device.</span></span>|
|<span data-ttu-id="36477-154">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="36477-154">featureUpdateVersion</span></span>|<span data-ttu-id="36477-155">String</span><span class="sxs-lookup"><span data-stu-id="36477-155">String</span></span>|<span data-ttu-id="36477-156">设备的当前功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="36477-156">The current feature update version of the device.</span></span>|
|<span data-ttu-id="36477-157">lastScanDateTime</span><span class="sxs-lookup"><span data-stu-id="36477-157">lastScanDateTime</span></span>|<span data-ttu-id="36477-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36477-158">DateTimeOffset</span></span>|<span data-ttu-id="36477-159">Windows Update 代理成功扫描的日期时间。</span><span class="sxs-lookup"><span data-stu-id="36477-159">The date time that the Windows Update Agent did a successful scan.</span></span>|
|<span data-ttu-id="36477-160">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="36477-160">lastSyncDateTime</span></span>|<span data-ttu-id="36477-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36477-161">DateTimeOffset</span></span>|<span data-ttu-id="36477-162">上次与 Microsoft Intune 同步设备的日期时间。</span><span class="sxs-lookup"><span data-stu-id="36477-162">Last date time that the device sync with with Microsoft Intune.</span></span>|



## <a name="response"></a><span data-ttu-id="36477-163">响应</span><span class="sxs-lookup"><span data-stu-id="36477-163">Response</span></span>
<span data-ttu-id="36477-164">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="36477-164">If successful, this method returns a `200 OK` response code and an updated [windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36477-165">示例</span><span class="sxs-lookup"><span data-stu-id="36477-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="36477-166">请求</span><span class="sxs-lookup"><span data-stu-id="36477-166">Request</span></span>
<span data-ttu-id="36477-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="36477-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="36477-168">响应</span><span class="sxs-lookup"><span data-stu-id="36477-168">Response</span></span>
<span data-ttu-id="36477-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="36477-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






