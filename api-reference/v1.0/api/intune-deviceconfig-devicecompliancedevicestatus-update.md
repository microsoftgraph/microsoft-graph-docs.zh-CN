---
title: 更新 deviceComplianceDeviceStatus
description: 更新 deviceComplianceDeviceStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c767cff5221d445da21c9416eb3f470677061086
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758384"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="ead29-103">更新 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="ead29-103">Update deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="ead29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ead29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ead29-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ead29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ead29-106">更新 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ead29-106">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ead29-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ead29-107">Prerequisites</span></span>
<span data-ttu-id="ead29-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ead29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ead29-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ead29-110">Permission type</span></span>|<span data-ttu-id="ead29-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ead29-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ead29-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ead29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ead29-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ead29-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ead29-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ead29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ead29-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ead29-115">Not supported.</span></span>|
|<span data-ttu-id="ead29-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ead29-116">Application</span></span>|<span data-ttu-id="ead29-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ead29-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ead29-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ead29-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ead29-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ead29-119">Request headers</span></span>
|<span data-ttu-id="ead29-120">标头</span><span class="sxs-lookup"><span data-stu-id="ead29-120">Header</span></span>|<span data-ttu-id="ead29-121">值</span><span class="sxs-lookup"><span data-stu-id="ead29-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ead29-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ead29-122">Authorization</span></span>|<span data-ttu-id="ead29-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ead29-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ead29-124">接受</span><span class="sxs-lookup"><span data-stu-id="ead29-124">Accept</span></span>|<span data-ttu-id="ead29-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ead29-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ead29-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ead29-126">Request body</span></span>
<span data-ttu-id="ead29-127">在请求正文中，提供 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ead29-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="ead29-128">下表显示了创建 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ead29-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="ead29-129">属性</span><span class="sxs-lookup"><span data-stu-id="ead29-129">Property</span></span>|<span data-ttu-id="ead29-130">类型</span><span class="sxs-lookup"><span data-stu-id="ead29-130">Type</span></span>|<span data-ttu-id="ead29-131">说明</span><span class="sxs-lookup"><span data-stu-id="ead29-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ead29-132">id</span><span class="sxs-lookup"><span data-stu-id="ead29-132">id</span></span>|<span data-ttu-id="ead29-133">String</span><span class="sxs-lookup"><span data-stu-id="ead29-133">String</span></span>|<span data-ttu-id="ead29-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ead29-134">Key of the entity.</span></span>|
|<span data-ttu-id="ead29-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ead29-135">deviceDisplayName</span></span>|<span data-ttu-id="ead29-136">String</span><span class="sxs-lookup"><span data-stu-id="ead29-136">String</span></span>|<span data-ttu-id="ead29-137">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="ead29-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ead29-138">userName</span><span class="sxs-lookup"><span data-stu-id="ead29-138">userName</span></span>|<span data-ttu-id="ead29-139">String</span><span class="sxs-lookup"><span data-stu-id="ead29-139">String</span></span>|<span data-ttu-id="ead29-140">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="ead29-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="ead29-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="ead29-141">deviceModel</span></span>|<span data-ttu-id="ead29-142">String</span><span class="sxs-lookup"><span data-stu-id="ead29-142">String</span></span>|<span data-ttu-id="ead29-143">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="ead29-143">The device model that is being reported</span></span>|
|<span data-ttu-id="ead29-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ead29-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="ead29-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ead29-145">DateTimeOffset</span></span>|<span data-ttu-id="ead29-146">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="ead29-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="ead29-147">status</span><span class="sxs-lookup"><span data-stu-id="ead29-147">status</span></span>|[<span data-ttu-id="ead29-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ead29-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ead29-149">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="ead29-149">Compliance status of the policy report.</span></span> <span data-ttu-id="ead29-150">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="ead29-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ead29-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ead29-151">lastReportedDateTime</span></span>|<span data-ttu-id="ead29-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ead29-152">DateTimeOffset</span></span>|<span data-ttu-id="ead29-153">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="ead29-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ead29-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ead29-154">userPrincipalName</span></span>|<span data-ttu-id="ead29-155">String</span><span class="sxs-lookup"><span data-stu-id="ead29-155">String</span></span>|<span data-ttu-id="ead29-156">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ead29-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="ead29-157">响应</span><span class="sxs-lookup"><span data-stu-id="ead29-157">Response</span></span>
<span data-ttu-id="ead29-158">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ead29-158">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ead29-159">示例</span><span class="sxs-lookup"><span data-stu-id="ead29-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="ead29-160">请求</span><span class="sxs-lookup"><span data-stu-id="ead29-160">Request</span></span>
<span data-ttu-id="ead29-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ead29-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ead29-162">响应</span><span class="sxs-lookup"><span data-stu-id="ead29-162">Response</span></span>
<span data-ttu-id="ead29-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ead29-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




