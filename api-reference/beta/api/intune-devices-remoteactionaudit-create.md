---
title: 创建 remoteActionAudit
description: 创建新的 remoteActionAudit 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2643ba37f92e7ff11d5f9a8ea070948fe2f44a55
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612054"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="ee6fe-103">创建 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="ee6fe-103">Create remoteActionAudit</span></span>

<span data-ttu-id="ee6fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee6fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ee6fe-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee6fe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee6fe-107">创建新的 [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-107">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee6fe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ee6fe-108">Prerequisites</span></span>
<span data-ttu-id="ee6fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee6fe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee6fe-111">Permission type</span></span>|<span data-ttu-id="ee6fe-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee6fe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee6fe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee6fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee6fe-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee6fe-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ee6fe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee6fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee6fe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-116">Not supported.</span></span>|
|<span data-ttu-id="ee6fe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee6fe-117">Application</span></span>|<span data-ttu-id="ee6fe-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee6fe-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee6fe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee6fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="ee6fe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee6fe-120">Request headers</span></span>
|<span data-ttu-id="ee6fe-121">标头</span><span class="sxs-lookup"><span data-stu-id="ee6fe-121">Header</span></span>|<span data-ttu-id="ee6fe-122">值</span><span class="sxs-lookup"><span data-stu-id="ee6fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee6fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee6fe-123">Authorization</span></span>|<span data-ttu-id="ee6fe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee6fe-125">接受</span><span class="sxs-lookup"><span data-stu-id="ee6fe-125">Accept</span></span>|<span data-ttu-id="ee6fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee6fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee6fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee6fe-127">Request body</span></span>
<span data-ttu-id="ee6fe-128">在请求正文中，提供 remoteActionAudit 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-128">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="ee6fe-129">下表显示创建 remoteActionAudit 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-129">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="ee6fe-130">属性</span><span class="sxs-lookup"><span data-stu-id="ee6fe-130">Property</span></span>|<span data-ttu-id="ee6fe-131">类型</span><span class="sxs-lookup"><span data-stu-id="ee6fe-131">Type</span></span>|<span data-ttu-id="ee6fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="ee6fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee6fe-133">id</span><span class="sxs-lookup"><span data-stu-id="ee6fe-133">id</span></span>|<span data-ttu-id="ee6fe-134">String</span><span class="sxs-lookup"><span data-stu-id="ee6fe-134">String</span></span>|<span data-ttu-id="ee6fe-135">报告 ID。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-135">Report Id.</span></span>|
|<span data-ttu-id="ee6fe-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ee6fe-136">deviceDisplayName</span></span>|<span data-ttu-id="ee6fe-137">String</span><span class="sxs-lookup"><span data-stu-id="ee6fe-137">String</span></span>|<span data-ttu-id="ee6fe-138">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-138">Intune device name.</span></span>|
|<span data-ttu-id="ee6fe-139">userName</span><span class="sxs-lookup"><span data-stu-id="ee6fe-139">userName</span></span>|<span data-ttu-id="ee6fe-140">String</span><span class="sxs-lookup"><span data-stu-id="ee6fe-140">String</span></span>|<span data-ttu-id="ee6fe-141">\[已弃用 \] 请改为使用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="ee6fe-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee6fe-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="ee6fe-143">String</span><span class="sxs-lookup"><span data-stu-id="ee6fe-143">String</span></span>|<span data-ttu-id="ee6fe-144">启动设备操作的用户，格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="ee6fe-145">action</span><span class="sxs-lookup"><span data-stu-id="ee6fe-145">action</span></span>|[<span data-ttu-id="ee6fe-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="ee6fe-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="ee6fe-147">操作名称。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-147">The action name.</span></span> <span data-ttu-id="ee6fe-148">可能的值是 `unknown` `factoryReset` `removeCompanyData` ：、、、、、、、、、、 `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName` 。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="ee6fe-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="ee6fe-149">requestDateTime</span></span>|<span data-ttu-id="ee6fe-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee6fe-150">DateTimeOffset</span></span>|<span data-ttu-id="ee6fe-151">发出操作的时间（以 UTC 表示）。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="ee6fe-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee6fe-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="ee6fe-153">String</span><span class="sxs-lookup"><span data-stu-id="ee6fe-153">String</span></span>|<span data-ttu-id="ee6fe-154">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="ee6fe-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="ee6fe-155">deviceIMEI</span></span>|<span data-ttu-id="ee6fe-156">String</span><span class="sxs-lookup"><span data-stu-id="ee6fe-156">String</span></span>|<span data-ttu-id="ee6fe-157">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-157">IMEI of the device.</span></span>|
|<span data-ttu-id="ee6fe-158">actionState</span><span class="sxs-lookup"><span data-stu-id="ee6fe-158">actionState</span></span>|[<span data-ttu-id="ee6fe-159">actionState</span><span class="sxs-lookup"><span data-stu-id="ee6fe-159">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="ee6fe-160">操作状态。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-160">Action state.</span></span> <span data-ttu-id="ee6fe-161">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed` 或 `notSupported`。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ee6fe-162">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ee6fe-162">managedDeviceId</span></span>|<span data-ttu-id="ee6fe-163">String</span><span class="sxs-lookup"><span data-stu-id="ee6fe-163">String</span></span>|<span data-ttu-id="ee6fe-164">操作目标。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-164">Action target.</span></span>|



## <a name="response"></a><span data-ttu-id="ee6fe-165">响应</span><span class="sxs-lookup"><span data-stu-id="ee6fe-165">Response</span></span>
<span data-ttu-id="ee6fe-166">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-166">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee6fe-167">示例</span><span class="sxs-lookup"><span data-stu-id="ee6fe-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee6fe-168">请求</span><span class="sxs-lookup"><span data-stu-id="ee6fe-168">Request</span></span>
<span data-ttu-id="ee6fe-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee6fe-170">响应</span><span class="sxs-lookup"><span data-stu-id="ee6fe-170">Response</span></span>
<span data-ttu-id="ee6fe-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ee6fe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




