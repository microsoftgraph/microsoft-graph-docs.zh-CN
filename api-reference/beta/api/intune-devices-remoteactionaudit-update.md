---
title: 更新 remoteActionAudit
description: 更新 remoteActionAudit 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb260dd46ebd99888edb9348dad55032b19a573b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468598"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="d308c-103">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d308c-103">Update remoteActionAudit</span></span>

<span data-ttu-id="d308c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d308c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d308c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d308c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d308c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d308c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d308c-107">更新[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d308c-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d308c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d308c-108">Prerequisites</span></span>
<span data-ttu-id="d308c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d308c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d308c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d308c-111">Permission type</span></span>|<span data-ttu-id="d308c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d308c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d308c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d308c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d308c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d308c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d308c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d308c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d308c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d308c-116">Not supported.</span></span>|
|<span data-ttu-id="d308c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d308c-117">Application</span></span>|<span data-ttu-id="d308c-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d308c-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d308c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d308c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="d308c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d308c-120">Request headers</span></span>
|<span data-ttu-id="d308c-121">标头</span><span class="sxs-lookup"><span data-stu-id="d308c-121">Header</span></span>|<span data-ttu-id="d308c-122">值</span><span class="sxs-lookup"><span data-stu-id="d308c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d308c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d308c-123">Authorization</span></span>|<span data-ttu-id="d308c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d308c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d308c-125">接受</span><span class="sxs-lookup"><span data-stu-id="d308c-125">Accept</span></span>|<span data-ttu-id="d308c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d308c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d308c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d308c-127">Request body</span></span>
<span data-ttu-id="d308c-128">在请求正文中，提供[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d308c-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="d308c-129">下表显示创建[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d308c-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="d308c-130">属性</span><span class="sxs-lookup"><span data-stu-id="d308c-130">Property</span></span>|<span data-ttu-id="d308c-131">类型</span><span class="sxs-lookup"><span data-stu-id="d308c-131">Type</span></span>|<span data-ttu-id="d308c-132">说明</span><span class="sxs-lookup"><span data-stu-id="d308c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d308c-133">id</span><span class="sxs-lookup"><span data-stu-id="d308c-133">id</span></span>|<span data-ttu-id="d308c-134">String</span><span class="sxs-lookup"><span data-stu-id="d308c-134">String</span></span>|<span data-ttu-id="d308c-135">报告 Id。</span><span class="sxs-lookup"><span data-stu-id="d308c-135">Report Id.</span></span>|
|<span data-ttu-id="d308c-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d308c-136">deviceDisplayName</span></span>|<span data-ttu-id="d308c-137">String</span><span class="sxs-lookup"><span data-stu-id="d308c-137">String</span></span>|<span data-ttu-id="d308c-138">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="d308c-138">Intune device name.</span></span>|
|<span data-ttu-id="d308c-139">userName</span><span class="sxs-lookup"><span data-stu-id="d308c-139">userName</span></span>|<span data-ttu-id="d308c-140">String</span><span class="sxs-lookup"><span data-stu-id="d308c-140">String</span></span>|<span data-ttu-id="d308c-141">\[弃用\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d308c-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="d308c-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d308c-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="d308c-143">String</span><span class="sxs-lookup"><span data-stu-id="d308c-143">String</span></span>|<span data-ttu-id="d308c-144">启动设备操作的用户的格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="d308c-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="d308c-145">action</span><span class="sxs-lookup"><span data-stu-id="d308c-145">action</span></span>|[<span data-ttu-id="d308c-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="d308c-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="d308c-147">操作名称。</span><span class="sxs-lookup"><span data-stu-id="d308c-147">The action name.</span></span> <span data-ttu-id="d308c-148">可能的值为`unknown`： `factoryReset`、 `removeCompanyData`、 `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `getFileVaultKey` `setDeviceName`、、、、、、、、、、、、、、、、、、、、。 `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey`</span><span class="sxs-lookup"><span data-stu-id="d308c-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="d308c-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="d308c-149">requestDateTime</span></span>|<span data-ttu-id="d308c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d308c-150">DateTimeOffset</span></span>|<span data-ttu-id="d308c-151">发出操作的时间，以 UTC 表示。</span><span class="sxs-lookup"><span data-stu-id="d308c-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="d308c-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d308c-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="d308c-153">String</span><span class="sxs-lookup"><span data-stu-id="d308c-153">String</span></span>|<span data-ttu-id="d308c-154">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="d308c-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="d308c-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="d308c-155">deviceIMEI</span></span>|<span data-ttu-id="d308c-156">String</span><span class="sxs-lookup"><span data-stu-id="d308c-156">String</span></span>|<span data-ttu-id="d308c-157">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="d308c-157">IMEI of the device.</span></span>|
|<span data-ttu-id="d308c-158">actionState</span><span class="sxs-lookup"><span data-stu-id="d308c-158">actionState</span></span>|[<span data-ttu-id="d308c-159">actionState</span><span class="sxs-lookup"><span data-stu-id="d308c-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d308c-160">动作状态。</span><span class="sxs-lookup"><span data-stu-id="d308c-160">Action state.</span></span> <span data-ttu-id="d308c-161">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d308c-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d308c-162">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d308c-162">managedDeviceId</span></span>|<span data-ttu-id="d308c-163">String</span><span class="sxs-lookup"><span data-stu-id="d308c-163">String</span></span>|<span data-ttu-id="d308c-164">操作目标。</span><span class="sxs-lookup"><span data-stu-id="d308c-164">Action target.</span></span>|



## <a name="response"></a><span data-ttu-id="d308c-165">响应</span><span class="sxs-lookup"><span data-stu-id="d308c-165">Response</span></span>
<span data-ttu-id="d308c-166">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d308c-166">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d308c-167">示例</span><span class="sxs-lookup"><span data-stu-id="d308c-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="d308c-168">请求</span><span class="sxs-lookup"><span data-stu-id="d308c-168">Request</span></span>
<span data-ttu-id="d308c-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d308c-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
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

### <a name="response"></a><span data-ttu-id="d308c-170">响应</span><span class="sxs-lookup"><span data-stu-id="d308c-170">Response</span></span>
<span data-ttu-id="d308c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d308c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





