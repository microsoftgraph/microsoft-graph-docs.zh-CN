---
title: 创建 remoteActionAudit
description: 创建新的 remoteActionAudit 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f320a3e8e2539e138aaafca98a6957d599784c7d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188246"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="24b41-103">创建 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="24b41-103">Create remoteActionAudit</span></span>

> <span data-ttu-id="24b41-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24b41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24b41-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24b41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24b41-106">创建新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="24b41-106">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24b41-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="24b41-107">Prerequisites</span></span>
<span data-ttu-id="24b41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24b41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24b41-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="24b41-110">Permission type</span></span>|<span data-ttu-id="24b41-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24b41-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24b41-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24b41-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24b41-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24b41-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="24b41-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24b41-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24b41-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="24b41-115">Not supported.</span></span>|
|<span data-ttu-id="24b41-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="24b41-116">Application</span></span>|<span data-ttu-id="24b41-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24b41-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24b41-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24b41-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="24b41-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="24b41-119">Request headers</span></span>
|<span data-ttu-id="24b41-120">标头</span><span class="sxs-lookup"><span data-stu-id="24b41-120">Header</span></span>|<span data-ttu-id="24b41-121">值</span><span class="sxs-lookup"><span data-stu-id="24b41-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24b41-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="24b41-122">Authorization</span></span>|<span data-ttu-id="24b41-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24b41-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24b41-124">接受</span><span class="sxs-lookup"><span data-stu-id="24b41-124">Accept</span></span>|<span data-ttu-id="24b41-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24b41-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24b41-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="24b41-126">Request body</span></span>
<span data-ttu-id="24b41-127">在请求正文中，提供 remoteActionAudit 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24b41-127">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="24b41-128">下表显示创建 remoteActionAudit 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="24b41-128">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="24b41-129">属性</span><span class="sxs-lookup"><span data-stu-id="24b41-129">Property</span></span>|<span data-ttu-id="24b41-130">类型</span><span class="sxs-lookup"><span data-stu-id="24b41-130">Type</span></span>|<span data-ttu-id="24b41-131">说明</span><span class="sxs-lookup"><span data-stu-id="24b41-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b41-132">id</span><span class="sxs-lookup"><span data-stu-id="24b41-132">id</span></span>|<span data-ttu-id="24b41-133">String</span><span class="sxs-lookup"><span data-stu-id="24b41-133">String</span></span>|<span data-ttu-id="24b41-134">报告 Id。</span><span class="sxs-lookup"><span data-stu-id="24b41-134">Report Id.</span></span>|
|<span data-ttu-id="24b41-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="24b41-135">deviceDisplayName</span></span>|<span data-ttu-id="24b41-136">String</span><span class="sxs-lookup"><span data-stu-id="24b41-136">String</span></span>|<span data-ttu-id="24b41-137">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="24b41-137">Intune device name.</span></span>|
|<span data-ttu-id="24b41-138">userName</span><span class="sxs-lookup"><span data-stu-id="24b41-138">userName</span></span>|<span data-ttu-id="24b41-139">String</span><span class="sxs-lookup"><span data-stu-id="24b41-139">String</span></span>|<span data-ttu-id="24b41-140">\[弃用\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="24b41-140">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="24b41-141">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="24b41-141">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="24b41-142">String</span><span class="sxs-lookup"><span data-stu-id="24b41-142">String</span></span>|<span data-ttu-id="24b41-143">启动设备操作的用户的格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="24b41-143">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="24b41-144">action</span><span class="sxs-lookup"><span data-stu-id="24b41-144">action</span></span>|[<span data-ttu-id="24b41-145">remoteAction</span><span class="sxs-lookup"><span data-stu-id="24b41-145">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="24b41-146">操作名称。</span><span class="sxs-lookup"><span data-stu-id="24b41-146">The action name.</span></span> <span data-ttu-id="24b41-147">可能的值为`unknown`： `factoryReset`、 `removeCompanyData`、 `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan`、、、、、、、、、、、、、、、、 `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span><span class="sxs-lookup"><span data-stu-id="24b41-147">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="24b41-148">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="24b41-148">requestDateTime</span></span>|<span data-ttu-id="24b41-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24b41-149">DateTimeOffset</span></span>|<span data-ttu-id="24b41-150">发出操作的时间，以 UTC 表示。</span><span class="sxs-lookup"><span data-stu-id="24b41-150">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="24b41-151">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="24b41-151">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="24b41-152">String</span><span class="sxs-lookup"><span data-stu-id="24b41-152">String</span></span>|<span data-ttu-id="24b41-153">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="24b41-153">Upn of the device owner.</span></span>|
|<span data-ttu-id="24b41-154">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="24b41-154">deviceIMEI</span></span>|<span data-ttu-id="24b41-155">String</span><span class="sxs-lookup"><span data-stu-id="24b41-155">String</span></span>|<span data-ttu-id="24b41-156">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="24b41-156">IMEI of the device.</span></span>|
|<span data-ttu-id="24b41-157">actionState</span><span class="sxs-lookup"><span data-stu-id="24b41-157">actionState</span></span>|[<span data-ttu-id="24b41-158">actionState</span><span class="sxs-lookup"><span data-stu-id="24b41-158">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="24b41-159">动作状态。</span><span class="sxs-lookup"><span data-stu-id="24b41-159">Action state.</span></span> <span data-ttu-id="24b41-160">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="24b41-160">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="24b41-161">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="24b41-161">managedDeviceId</span></span>|<span data-ttu-id="24b41-162">String</span><span class="sxs-lookup"><span data-stu-id="24b41-162">String</span></span>|<span data-ttu-id="24b41-163">操作目标。</span><span class="sxs-lookup"><span data-stu-id="24b41-163">Action target.</span></span>|



## <a name="response"></a><span data-ttu-id="24b41-164">响应</span><span class="sxs-lookup"><span data-stu-id="24b41-164">Response</span></span>
<span data-ttu-id="24b41-165">如果成功，此方法在响应`201 Created`正文中返回响应代码和[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="24b41-165">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24b41-166">示例</span><span class="sxs-lookup"><span data-stu-id="24b41-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="24b41-167">请求</span><span class="sxs-lookup"><span data-stu-id="24b41-167">Request</span></span>
<span data-ttu-id="24b41-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24b41-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="24b41-169">响应</span><span class="sxs-lookup"><span data-stu-id="24b41-169">Response</span></span>
<span data-ttu-id="24b41-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24b41-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```




