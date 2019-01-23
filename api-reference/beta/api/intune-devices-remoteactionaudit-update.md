---
title: 更新 remoteActionAudit
description: 更新 remoteActionAudit 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6078b3f6fd5236bd0e6e1a51f5f52cbf69a59c83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396187"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="7f31e-103">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="7f31e-103">Update remoteActionAudit</span></span>

> <span data-ttu-id="7f31e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7f31e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7f31e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7f31e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f31e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f31e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f31e-107">更新[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7f31e-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f31e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f31e-108">Prerequisites</span></span>
<span data-ttu-id="7f31e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7f31e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7f31e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f31e-111">Permission type</span></span>|<span data-ttu-id="7f31e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f31e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f31e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f31e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f31e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f31e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7f31e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f31e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f31e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f31e-116">Not supported.</span></span>|
|<span data-ttu-id="7f31e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f31e-117">Application</span></span>|<span data-ttu-id="7f31e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f31e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f31e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f31e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="7f31e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f31e-120">Request headers</span></span>
|<span data-ttu-id="7f31e-121">标头</span><span class="sxs-lookup"><span data-stu-id="7f31e-121">Header</span></span>|<span data-ttu-id="7f31e-122">值</span><span class="sxs-lookup"><span data-stu-id="7f31e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f31e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f31e-123">Authorization</span></span>|<span data-ttu-id="7f31e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f31e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f31e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f31e-125">Accept</span></span>|<span data-ttu-id="7f31e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f31e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f31e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f31e-127">Request body</span></span>
<span data-ttu-id="7f31e-128">在请求正文中，提供[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f31e-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="7f31e-129">下表显示时创建[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7f31e-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="7f31e-130">属性</span><span class="sxs-lookup"><span data-stu-id="7f31e-130">Property</span></span>|<span data-ttu-id="7f31e-131">类型</span><span class="sxs-lookup"><span data-stu-id="7f31e-131">Type</span></span>|<span data-ttu-id="7f31e-132">说明</span><span class="sxs-lookup"><span data-stu-id="7f31e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f31e-133">id</span><span class="sxs-lookup"><span data-stu-id="7f31e-133">id</span></span>|<span data-ttu-id="7f31e-134">String</span><span class="sxs-lookup"><span data-stu-id="7f31e-134">String</span></span>|<span data-ttu-id="7f31e-135">报告 id。</span><span class="sxs-lookup"><span data-stu-id="7f31e-135">Report Id.</span></span>|
|<span data-ttu-id="7f31e-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7f31e-136">deviceDisplayName</span></span>|<span data-ttu-id="7f31e-137">String</span><span class="sxs-lookup"><span data-stu-id="7f31e-137">String</span></span>|<span data-ttu-id="7f31e-138">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="7f31e-138">Intune device name.</span></span>|
|<span data-ttu-id="7f31e-139">userName</span><span class="sxs-lookup"><span data-stu-id="7f31e-139">userName</span></span>|<span data-ttu-id="7f31e-140">String</span><span class="sxs-lookup"><span data-stu-id="7f31e-140">String</span></span>|<span data-ttu-id="7f31e-141">\[弃用的\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="7f31e-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="7f31e-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7f31e-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="7f31e-143">String</span><span class="sxs-lookup"><span data-stu-id="7f31e-143">String</span></span>|<span data-ttu-id="7f31e-144">用户启动的设备操作，格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="7f31e-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="7f31e-145">action</span><span class="sxs-lookup"><span data-stu-id="7f31e-145">action</span></span>|[<span data-ttu-id="7f31e-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="7f31e-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="7f31e-147">操作名称。</span><span class="sxs-lookup"><span data-stu-id="7f31e-147">The action name.</span></span> <span data-ttu-id="7f31e-148">可能的值为： `unknown`， `factoryReset`， `removeCompanyData`， `resetPasscode`， `remoteLock`， `enableLostMode`， `disableLostMode`， `locateDevice`， `rebootNow`， `recoverPasscode`， `cleanWindowsDevice`， `logoutSharedAppleDeviceActiveUser`， `quickScan`， `fullScan`， `windowsDefenderUpdateSignatures`， `factoryResetKeepEnrollmentData`， `updateDeviceAccount`， `automaticRedeployment`， `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="7f31e-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="7f31e-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="7f31e-149">requestDateTime</span></span>|<span data-ttu-id="7f31e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f31e-150">DateTimeOffset</span></span>|<span data-ttu-id="7f31e-151">发布该操作时，给定采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="7f31e-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="7f31e-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7f31e-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="7f31e-153">String</span><span class="sxs-lookup"><span data-stu-id="7f31e-153">String</span></span>|<span data-ttu-id="7f31e-154">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="7f31e-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="7f31e-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="7f31e-155">deviceIMEI</span></span>|<span data-ttu-id="7f31e-156">String</span><span class="sxs-lookup"><span data-stu-id="7f31e-156">String</span></span>|<span data-ttu-id="7f31e-157">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="7f31e-157">IMEI of the device.</span></span>|
|<span data-ttu-id="7f31e-158">actionState</span><span class="sxs-lookup"><span data-stu-id="7f31e-158">actionState</span></span>|[<span data-ttu-id="7f31e-159">actionState</span><span class="sxs-lookup"><span data-stu-id="7f31e-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7f31e-160">操作状态。</span><span class="sxs-lookup"><span data-stu-id="7f31e-160">Action state.</span></span> <span data-ttu-id="7f31e-161">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="7f31e-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="7f31e-162">响应</span><span class="sxs-lookup"><span data-stu-id="7f31e-162">Response</span></span>
<span data-ttu-id="7f31e-163">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7f31e-163">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f31e-164">示例</span><span class="sxs-lookup"><span data-stu-id="7f31e-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f31e-165">请求</span><span class="sxs-lookup"><span data-stu-id="7f31e-165">Request</span></span>
<span data-ttu-id="7f31e-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f31e-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
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

### <a name="response"></a><span data-ttu-id="7f31e-167">响应</span><span class="sxs-lookup"><span data-stu-id="7f31e-167">Response</span></span>
<span data-ttu-id="7f31e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f31e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




