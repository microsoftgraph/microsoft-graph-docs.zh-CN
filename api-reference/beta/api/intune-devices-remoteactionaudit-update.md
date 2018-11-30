---
title: 更新 remoteActionAudit
description: 更新 remoteActionAudit 对象的属性。
ms.openlocfilehash: f7b72ce26617b3ba370e5135c31b98c7c33cbd97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046877"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="d2f04-103">更新 remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d2f04-103">Update remoteActionAudit</span></span>

> <span data-ttu-id="d2f04-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2f04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2f04-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2f04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2f04-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d2f04-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2f04-107">更新[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2f04-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2f04-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2f04-108">Prerequisites</span></span>
<span data-ttu-id="d2f04-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d2f04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2f04-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2f04-111">Permission type</span></span>|<span data-ttu-id="d2f04-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2f04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2f04-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2f04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2f04-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f04-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d2f04-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2f04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2f04-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2f04-116">Not supported.</span></span>|
|<span data-ttu-id="d2f04-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2f04-117">Application</span></span>|<span data-ttu-id="d2f04-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2f04-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2f04-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2f04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="d2f04-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2f04-120">Request headers</span></span>
|<span data-ttu-id="d2f04-121">标头</span><span class="sxs-lookup"><span data-stu-id="d2f04-121">Header</span></span>|<span data-ttu-id="d2f04-122">值</span><span class="sxs-lookup"><span data-stu-id="d2f04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2f04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2f04-123">Authorization</span></span>|<span data-ttu-id="d2f04-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2f04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2f04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2f04-125">Accept</span></span>|<span data-ttu-id="d2f04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2f04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2f04-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2f04-127">Request body</span></span>
<span data-ttu-id="d2f04-128">在请求正文中，提供[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2f04-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="d2f04-129">下表显示时创建[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d2f04-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="d2f04-130">属性</span><span class="sxs-lookup"><span data-stu-id="d2f04-130">Property</span></span>|<span data-ttu-id="d2f04-131">类型</span><span class="sxs-lookup"><span data-stu-id="d2f04-131">Type</span></span>|<span data-ttu-id="d2f04-132">说明</span><span class="sxs-lookup"><span data-stu-id="d2f04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2f04-133">id</span><span class="sxs-lookup"><span data-stu-id="d2f04-133">id</span></span>|<span data-ttu-id="d2f04-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d2f04-134">String</span></span>|<span data-ttu-id="d2f04-135">报告 id。</span><span class="sxs-lookup"><span data-stu-id="d2f04-135">Report Id.</span></span>|
|<span data-ttu-id="d2f04-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d2f04-136">deviceDisplayName</span></span>|<span data-ttu-id="d2f04-137">String</span><span class="sxs-lookup"><span data-stu-id="d2f04-137">String</span></span>|<span data-ttu-id="d2f04-138">Intune 设备名称。</span><span class="sxs-lookup"><span data-stu-id="d2f04-138">Intune device name.</span></span>|
|<span data-ttu-id="d2f04-139">userName</span><span class="sxs-lookup"><span data-stu-id="d2f04-139">userName</span></span>|<span data-ttu-id="d2f04-140">String</span><span class="sxs-lookup"><span data-stu-id="d2f04-140">String</span></span>|<span data-ttu-id="d2f04-141">\[弃用的\]请改用 InitiatedByUserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d2f04-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="d2f04-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d2f04-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="d2f04-143">字符串</span><span class="sxs-lookup"><span data-stu-id="d2f04-143">String</span></span>|<span data-ttu-id="d2f04-144">用户启动的设备操作，格式为 UPN。</span><span class="sxs-lookup"><span data-stu-id="d2f04-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="d2f04-145">action</span><span class="sxs-lookup"><span data-stu-id="d2f04-145">action</span></span>|[<span data-ttu-id="d2f04-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="d2f04-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="d2f04-147">操作名称。</span><span class="sxs-lookup"><span data-stu-id="d2f04-147">The action name.</span></span> <span data-ttu-id="d2f04-148">可能的值为： `unknown`， `factoryReset`， `removeCompanyData`， `resetPasscode`， `remoteLock`， `enableLostMode`， `disableLostMode`， `locateDevice`， `rebootNow`， `recoverPasscode`， `cleanWindowsDevice`， `logoutSharedAppleDeviceActiveUser`， `quickScan`， `fullScan`， `windowsDefenderUpdateSignatures`， `factoryResetKeepEnrollmentData`， `updateDeviceAccount`， `automaticRedeployment`， `shutDown`.</span><span class="sxs-lookup"><span data-stu-id="d2f04-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="d2f04-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="d2f04-149">requestDateTime</span></span>|<span data-ttu-id="d2f04-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2f04-150">DateTimeOffset</span></span>|<span data-ttu-id="d2f04-151">发布该操作时，给定采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d2f04-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="d2f04-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d2f04-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="d2f04-153">字符串</span><span class="sxs-lookup"><span data-stu-id="d2f04-153">String</span></span>|<span data-ttu-id="d2f04-154">设备所有者的 Upn。</span><span class="sxs-lookup"><span data-stu-id="d2f04-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="d2f04-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="d2f04-155">deviceIMEI</span></span>|<span data-ttu-id="d2f04-156">字符串</span><span class="sxs-lookup"><span data-stu-id="d2f04-156">String</span></span>|<span data-ttu-id="d2f04-157">设备的 IMEI。</span><span class="sxs-lookup"><span data-stu-id="d2f04-157">IMEI of the device.</span></span>|
|<span data-ttu-id="d2f04-158">actionState</span><span class="sxs-lookup"><span data-stu-id="d2f04-158">actionState</span></span>|[<span data-ttu-id="d2f04-159">actionState</span><span class="sxs-lookup"><span data-stu-id="d2f04-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d2f04-160">操作状态。</span><span class="sxs-lookup"><span data-stu-id="d2f04-160">Action state.</span></span> <span data-ttu-id="d2f04-161">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="d2f04-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|



## <a name="response"></a><span data-ttu-id="d2f04-162">响应</span><span class="sxs-lookup"><span data-stu-id="d2f04-162">Response</span></span>
<span data-ttu-id="d2f04-163">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d2f04-163">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2f04-164">示例</span><span class="sxs-lookup"><span data-stu-id="d2f04-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2f04-165">请求</span><span class="sxs-lookup"><span data-stu-id="d2f04-165">Request</span></span>
<span data-ttu-id="d2f04-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2f04-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 399

{
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

### <a name="response"></a><span data-ttu-id="d2f04-167">响应</span><span class="sxs-lookup"><span data-stu-id="d2f04-167">Response</span></span>
<span data-ttu-id="d2f04-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2f04-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





