---
title: 创建 remoteActionAudit
description: 创建新的 remoteActionAudit 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 47ba3de19ca5cdc9b01bb3b65eb8b04e75831d87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396880"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="9fbf6-103">创建 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="9fbf6-103">Create remoteActionAudit</span></span>

> <span data-ttu-id="9fbf6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9fbf6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fbf6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fbf6-107">创建新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-107">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fbf6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9fbf6-108">Prerequisites</span></span>
<span data-ttu-id="9fbf6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9fbf6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fbf6-111">Permission type</span></span>|<span data-ttu-id="9fbf6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9fbf6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fbf6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fbf6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fbf6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fbf6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9fbf6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fbf6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fbf6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-116">Not supported.</span></span>|
|<span data-ttu-id="9fbf6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fbf6-117">Application</span></span>|<span data-ttu-id="9fbf6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fbf6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fbf6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="9fbf6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fbf6-120">Request headers</span></span>
|<span data-ttu-id="9fbf6-121">标头</span><span class="sxs-lookup"><span data-stu-id="9fbf6-121">Header</span></span>|<span data-ttu-id="9fbf6-122">值</span><span class="sxs-lookup"><span data-stu-id="9fbf6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fbf6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fbf6-123">Authorization</span></span>|<span data-ttu-id="9fbf6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fbf6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9fbf6-125">Accept</span></span>|<span data-ttu-id="9fbf6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fbf6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fbf6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fbf6-127">Request body</span></span>
<span data-ttu-id="9fbf6-128">在请求正文中，提供 remoteActionAudit 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-128">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="9fbf6-129">下表显示时创建 remoteActionAudit 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-129">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="9fbf6-130">属性</span><span class="sxs-lookup"><span data-stu-id="9fbf6-130">Property</span></span>|<span data-ttu-id="9fbf6-131">类型</span><span class="sxs-lookup"><span data-stu-id="9fbf6-131">Type</span></span>|<span data-ttu-id="9fbf6-132">说明</span><span class="sxs-lookup"><span data-stu-id="9fbf6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fbf6-133">id</span><span class="sxs-lookup"><span data-stu-id="9fbf6-133">id</span></span>|<span data-ttu-id="9fbf6-134">String</span><span class="sxs-lookup"><span data-stu-id="9fbf6-134">String</span></span>|<span data-ttu-id="9fbf6-135">报告 id。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-135">Report Id.</span></span>|
|<span data-ttu-id="9fbf6-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9fbf6-136">deviceDisplayName</span></span>|<span data-ttu-id="9fbf6-137">String</span><span class="sxs-lookup"><span data-stu-id="9fbf6-137">String</span></span>|<span data-ttu-id="9fbf6-138">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-138">Intune device name.</span></span>|
|<span data-ttu-id="9fbf6-139">userName</span><span class="sxs-lookup"><span data-stu-id="9fbf6-139">userName</span></span>|<span data-ttu-id="9fbf6-140">String</span><span class="sxs-lookup"><span data-stu-id="9fbf6-140">String</span></span>|<span data-ttu-id="9fbf6-141">\[弃用的\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="9fbf6-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9fbf6-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="9fbf6-143">String</span><span class="sxs-lookup"><span data-stu-id="9fbf6-143">String</span></span>|<span data-ttu-id="9fbf6-144">用户启动的设备操作，格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="9fbf6-145">action</span><span class="sxs-lookup"><span data-stu-id="9fbf6-145">action</span></span>|[<span data-ttu-id="9fbf6-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="9fbf6-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="9fbf6-147">操作名称。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-147">The action name.</span></span> <span data-ttu-id="9fbf6-148">可能的值为： `unknown`， `factoryReset`， `removeCompanyData`， `resetPasscode`， `remoteLock`， `enableLostMode`， `disableLostMode`， `locateDevice`， `rebootNow`， `recoverPasscode`， `cleanWindowsDevice`， `logoutSharedAppleDeviceActiveUser`， `quickScan`， `fullScan`， `windowsDefenderUpdateSignatures`， `factoryResetKeepEnrollmentData`， `updateDeviceAccount`， `automaticRedeployment`， `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="9fbf6-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="9fbf6-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="9fbf6-149">requestDateTime</span></span>|<span data-ttu-id="9fbf6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fbf6-150">DateTimeOffset</span></span>|<span data-ttu-id="9fbf6-151">发布该操作时，给定采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="9fbf6-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9fbf6-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="9fbf6-153">String</span><span class="sxs-lookup"><span data-stu-id="9fbf6-153">String</span></span>|<span data-ttu-id="9fbf6-154">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="9fbf6-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="9fbf6-155">deviceIMEI</span></span>|<span data-ttu-id="9fbf6-156">String</span><span class="sxs-lookup"><span data-stu-id="9fbf6-156">String</span></span>|<span data-ttu-id="9fbf6-157">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-157">IMEI of the device.</span></span>|
|<span data-ttu-id="9fbf6-158">actionState</span><span class="sxs-lookup"><span data-stu-id="9fbf6-158">actionState</span></span>|[<span data-ttu-id="9fbf6-159">actionState</span><span class="sxs-lookup"><span data-stu-id="9fbf6-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9fbf6-160">操作状态。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-160">Action state.</span></span> <span data-ttu-id="9fbf6-161">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="9fbf6-162">响应</span><span class="sxs-lookup"><span data-stu-id="9fbf6-162">Response</span></span>
<span data-ttu-id="9fbf6-163">如果成功，此方法返回`201 Created`响应代码和响应正文中的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-163">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fbf6-164">示例</span><span class="sxs-lookup"><span data-stu-id="9fbf6-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fbf6-165">请求</span><span class="sxs-lookup"><span data-stu-id="9fbf6-165">Request</span></span>
<span data-ttu-id="9fbf6-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending"
}
```

### <a name="response"></a><span data-ttu-id="9fbf6-167">响应</span><span class="sxs-lookup"><span data-stu-id="9fbf6-167">Response</span></span>
<span data-ttu-id="9fbf6-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9fbf6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

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
  "actionState": "pending"
}
```




