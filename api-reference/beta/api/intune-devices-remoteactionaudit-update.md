---
title: 更新 remoteActionAudit
description: 更新 remoteActionAudit 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02c2af28995b72246bc82f7af8d27e1f1171adc0
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51609498"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="a2b28-103">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="a2b28-103">Update remoteActionAudit</span></span>

<span data-ttu-id="a2b28-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2b28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2b28-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2b28-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2b28-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2b28-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2b28-107">更新 [remoteActionAudit 对象](../resources/intune-devices-remoteactionaudit.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a2b28-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2b28-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2b28-108">Prerequisites</span></span>
<span data-ttu-id="a2b28-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a2b28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2b28-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2b28-111">Permission type</span></span>|<span data-ttu-id="a2b28-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a2b28-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2b28-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2b28-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b28-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a2b28-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2b28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2b28-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2b28-116">Not supported.</span></span>|
|<span data-ttu-id="a2b28-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2b28-117">Application</span></span>|<span data-ttu-id="a2b28-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2b28-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2b28-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2b28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="a2b28-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2b28-120">Request headers</span></span>
|<span data-ttu-id="a2b28-121">标头</span><span class="sxs-lookup"><span data-stu-id="a2b28-121">Header</span></span>|<span data-ttu-id="a2b28-122">值</span><span class="sxs-lookup"><span data-stu-id="a2b28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2b28-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2b28-123">Authorization</span></span>|<span data-ttu-id="a2b28-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2b28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2b28-125">接受</span><span class="sxs-lookup"><span data-stu-id="a2b28-125">Accept</span></span>|<span data-ttu-id="a2b28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2b28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2b28-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2b28-127">Request body</span></span>
<span data-ttu-id="a2b28-128">在请求正文中，提供 [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2b28-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="a2b28-129">下表显示创建 [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2b28-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="a2b28-130">属性</span><span class="sxs-lookup"><span data-stu-id="a2b28-130">Property</span></span>|<span data-ttu-id="a2b28-131">类型</span><span class="sxs-lookup"><span data-stu-id="a2b28-131">Type</span></span>|<span data-ttu-id="a2b28-132">说明</span><span class="sxs-lookup"><span data-stu-id="a2b28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2b28-133">id</span><span class="sxs-lookup"><span data-stu-id="a2b28-133">id</span></span>|<span data-ttu-id="a2b28-134">String</span><span class="sxs-lookup"><span data-stu-id="a2b28-134">String</span></span>|<span data-ttu-id="a2b28-135">报告 ID。</span><span class="sxs-lookup"><span data-stu-id="a2b28-135">Report Id.</span></span>|
|<span data-ttu-id="a2b28-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a2b28-136">deviceDisplayName</span></span>|<span data-ttu-id="a2b28-137">String</span><span class="sxs-lookup"><span data-stu-id="a2b28-137">String</span></span>|<span data-ttu-id="a2b28-138">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="a2b28-138">Intune device name.</span></span>|
|<span data-ttu-id="a2b28-139">userName</span><span class="sxs-lookup"><span data-stu-id="a2b28-139">userName</span></span>|<span data-ttu-id="a2b28-140">String</span><span class="sxs-lookup"><span data-stu-id="a2b28-140">String</span></span>|<span data-ttu-id="a2b28-141">\[已弃用 \] 请改为使用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="a2b28-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="a2b28-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a2b28-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="a2b28-143">String</span><span class="sxs-lookup"><span data-stu-id="a2b28-143">String</span></span>|<span data-ttu-id="a2b28-144">启动设备操作的用户，格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="a2b28-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="a2b28-145">action</span><span class="sxs-lookup"><span data-stu-id="a2b28-145">action</span></span>|[<span data-ttu-id="a2b28-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="a2b28-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="a2b28-147">操作名称。</span><span class="sxs-lookup"><span data-stu-id="a2b28-147">The action name.</span></span> <span data-ttu-id="a2b28-148">可能的值是 `unknown` `factoryReset` `removeCompanyData` ：、、、、、、、、、、 `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName` 。</span><span class="sxs-lookup"><span data-stu-id="a2b28-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="a2b28-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="a2b28-149">requestDateTime</span></span>|<span data-ttu-id="a2b28-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2b28-150">DateTimeOffset</span></span>|<span data-ttu-id="a2b28-151">发出操作的时间（以 UTC 表示）。</span><span class="sxs-lookup"><span data-stu-id="a2b28-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="a2b28-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a2b28-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="a2b28-153">String</span><span class="sxs-lookup"><span data-stu-id="a2b28-153">String</span></span>|<span data-ttu-id="a2b28-154">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="a2b28-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="a2b28-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="a2b28-155">deviceIMEI</span></span>|<span data-ttu-id="a2b28-156">String</span><span class="sxs-lookup"><span data-stu-id="a2b28-156">String</span></span>|<span data-ttu-id="a2b28-157">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="a2b28-157">IMEI of the device.</span></span>|
|<span data-ttu-id="a2b28-158">actionState</span><span class="sxs-lookup"><span data-stu-id="a2b28-158">actionState</span></span>|[<span data-ttu-id="a2b28-159">actionState</span><span class="sxs-lookup"><span data-stu-id="a2b28-159">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="a2b28-160">操作状态。</span><span class="sxs-lookup"><span data-stu-id="a2b28-160">Action state.</span></span> <span data-ttu-id="a2b28-161">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="a2b28-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a2b28-162">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a2b28-162">managedDeviceId</span></span>|<span data-ttu-id="a2b28-163">String</span><span class="sxs-lookup"><span data-stu-id="a2b28-163">String</span></span>|<span data-ttu-id="a2b28-164">操作目标。</span><span class="sxs-lookup"><span data-stu-id="a2b28-164">Action target.</span></span>|



## <a name="response"></a><span data-ttu-id="a2b28-165">响应</span><span class="sxs-lookup"><span data-stu-id="a2b28-165">Response</span></span>
<span data-ttu-id="a2b28-166">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2b28-166">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2b28-167">示例</span><span class="sxs-lookup"><span data-stu-id="a2b28-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2b28-168">请求</span><span class="sxs-lookup"><span data-stu-id="a2b28-168">Request</span></span>
<span data-ttu-id="a2b28-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2b28-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2b28-170">响应</span><span class="sxs-lookup"><span data-stu-id="a2b28-170">Response</span></span>
<span data-ttu-id="a2b28-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2b28-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




