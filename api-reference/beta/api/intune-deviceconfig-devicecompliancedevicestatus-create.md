---
title: 创建 deviceComplianceDeviceStatus
description: 创建新的 deviceComplianceDeviceStatus 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa3d9ea5e68be8656a7702b7321d8ca982328468
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42756160"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="f5249-103">创建 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f5249-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="f5249-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5249-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5249-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5249-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5249-106">创建新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5249-106">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5249-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5249-107">Prerequisites</span></span>
<span data-ttu-id="f5249-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5249-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5249-110">Permission type</span></span>|<span data-ttu-id="f5249-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5249-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5249-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5249-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5249-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5249-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5249-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5249-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5249-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5249-115">Not supported.</span></span>|
|<span data-ttu-id="f5249-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5249-116">Application</span></span>|<span data-ttu-id="f5249-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5249-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5249-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5249-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f5249-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5249-119">Request headers</span></span>
|<span data-ttu-id="f5249-120">标头</span><span class="sxs-lookup"><span data-stu-id="f5249-120">Header</span></span>|<span data-ttu-id="f5249-121">值</span><span class="sxs-lookup"><span data-stu-id="f5249-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5249-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5249-122">Authorization</span></span>|<span data-ttu-id="f5249-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5249-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5249-124">接受</span><span class="sxs-lookup"><span data-stu-id="f5249-124">Accept</span></span>|<span data-ttu-id="f5249-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5249-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5249-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5249-126">Request body</span></span>
<span data-ttu-id="f5249-127">在请求正文中，提供 deviceComplianceDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5249-127">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="f5249-128">下表显示创建 deviceComplianceDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5249-128">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="f5249-129">属性</span><span class="sxs-lookup"><span data-stu-id="f5249-129">Property</span></span>|<span data-ttu-id="f5249-130">类型</span><span class="sxs-lookup"><span data-stu-id="f5249-130">Type</span></span>|<span data-ttu-id="f5249-131">说明</span><span class="sxs-lookup"><span data-stu-id="f5249-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5249-132">id</span><span class="sxs-lookup"><span data-stu-id="f5249-132">id</span></span>|<span data-ttu-id="f5249-133">String</span><span class="sxs-lookup"><span data-stu-id="f5249-133">String</span></span>|<span data-ttu-id="f5249-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f5249-134">Key of the entity.</span></span>|
|<span data-ttu-id="f5249-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f5249-135">deviceDisplayName</span></span>|<span data-ttu-id="f5249-136">String</span><span class="sxs-lookup"><span data-stu-id="f5249-136">String</span></span>|<span data-ttu-id="f5249-137">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="f5249-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f5249-138">userName</span><span class="sxs-lookup"><span data-stu-id="f5249-138">userName</span></span>|<span data-ttu-id="f5249-139">String</span><span class="sxs-lookup"><span data-stu-id="f5249-139">String</span></span>|<span data-ttu-id="f5249-140">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="f5249-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="f5249-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f5249-141">deviceModel</span></span>|<span data-ttu-id="f5249-142">String</span><span class="sxs-lookup"><span data-stu-id="f5249-142">String</span></span>|<span data-ttu-id="f5249-143">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="f5249-143">The device model that is being reported</span></span>|
|<span data-ttu-id="f5249-144">platform</span><span class="sxs-lookup"><span data-stu-id="f5249-144">platform</span></span>|<span data-ttu-id="f5249-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f5249-145">Int32</span></span>|<span data-ttu-id="f5249-146">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="f5249-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="f5249-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f5249-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f5249-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5249-148">DateTimeOffset</span></span>|<span data-ttu-id="f5249-149">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="f5249-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f5249-150">status</span><span class="sxs-lookup"><span data-stu-id="f5249-150">status</span></span>|[<span data-ttu-id="f5249-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f5249-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f5249-152">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="f5249-152">Compliance status of the policy report.</span></span> <span data-ttu-id="f5249-153">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="f5249-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f5249-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5249-154">lastReportedDateTime</span></span>|<span data-ttu-id="f5249-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5249-155">DateTimeOffset</span></span>|<span data-ttu-id="f5249-156">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="f5249-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f5249-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f5249-157">userPrincipalName</span></span>|<span data-ttu-id="f5249-158">String</span><span class="sxs-lookup"><span data-stu-id="f5249-158">String</span></span>|<span data-ttu-id="f5249-159">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f5249-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f5249-160">响应</span><span class="sxs-lookup"><span data-stu-id="f5249-160">Response</span></span>
<span data-ttu-id="f5249-161">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和更新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5249-161">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5249-162">示例</span><span class="sxs-lookup"><span data-stu-id="f5249-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5249-163">请求</span><span class="sxs-lookup"><span data-stu-id="f5249-163">Request</span></span>
<span data-ttu-id="f5249-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5249-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="f5249-165">响应</span><span class="sxs-lookup"><span data-stu-id="f5249-165">Response</span></span>
<span data-ttu-id="f5249-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5249-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 493

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




