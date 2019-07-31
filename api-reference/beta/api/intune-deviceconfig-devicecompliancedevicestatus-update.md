---
title: 更新 deviceComplianceDeviceStatus
description: 更新 deviceComplianceDeviceStatus 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc9ca797d8b9d40cd9598b07947f54988c44e824
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949907"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="d9cde-103">更新 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="d9cde-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="d9cde-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d9cde-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9cde-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9cde-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9cde-106">更新 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9cde-106">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9cde-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9cde-107">Prerequisites</span></span>
<span data-ttu-id="d9cde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9cde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9cde-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9cde-110">Permission type</span></span>|<span data-ttu-id="d9cde-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9cde-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9cde-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9cde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9cde-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9cde-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9cde-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9cde-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9cde-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9cde-115">Not supported.</span></span>|
|<span data-ttu-id="d9cde-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9cde-116">Application</span></span>|<span data-ttu-id="d9cde-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9cde-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9cde-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9cde-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="d9cde-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9cde-119">Request headers</span></span>
|<span data-ttu-id="d9cde-120">标头</span><span class="sxs-lookup"><span data-stu-id="d9cde-120">Header</span></span>|<span data-ttu-id="d9cde-121">值</span><span class="sxs-lookup"><span data-stu-id="d9cde-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9cde-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9cde-122">Authorization</span></span>|<span data-ttu-id="d9cde-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9cde-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9cde-124">接受</span><span class="sxs-lookup"><span data-stu-id="d9cde-124">Accept</span></span>|<span data-ttu-id="d9cde-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9cde-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9cde-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9cde-126">Request body</span></span>
<span data-ttu-id="d9cde-127">在请求正文中，提供 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9cde-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="d9cde-128">下表显示了创建 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d9cde-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="d9cde-129">属性</span><span class="sxs-lookup"><span data-stu-id="d9cde-129">Property</span></span>|<span data-ttu-id="d9cde-130">类型</span><span class="sxs-lookup"><span data-stu-id="d9cde-130">Type</span></span>|<span data-ttu-id="d9cde-131">说明</span><span class="sxs-lookup"><span data-stu-id="d9cde-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9cde-132">id</span><span class="sxs-lookup"><span data-stu-id="d9cde-132">id</span></span>|<span data-ttu-id="d9cde-133">String</span><span class="sxs-lookup"><span data-stu-id="d9cde-133">String</span></span>|<span data-ttu-id="d9cde-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9cde-134">Key of the entity.</span></span>|
|<span data-ttu-id="d9cde-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d9cde-135">deviceDisplayName</span></span>|<span data-ttu-id="d9cde-136">String</span><span class="sxs-lookup"><span data-stu-id="d9cde-136">String</span></span>|<span data-ttu-id="d9cde-137">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="d9cde-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="d9cde-138">userName</span><span class="sxs-lookup"><span data-stu-id="d9cde-138">userName</span></span>|<span data-ttu-id="d9cde-139">String</span><span class="sxs-lookup"><span data-stu-id="d9cde-139">String</span></span>|<span data-ttu-id="d9cde-140">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="d9cde-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="d9cde-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d9cde-141">deviceModel</span></span>|<span data-ttu-id="d9cde-142">String</span><span class="sxs-lookup"><span data-stu-id="d9cde-142">String</span></span>|<span data-ttu-id="d9cde-143">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="d9cde-143">The device model that is being reported</span></span>|
|<span data-ttu-id="d9cde-144">platform</span><span class="sxs-lookup"><span data-stu-id="d9cde-144">platform</span></span>|<span data-ttu-id="d9cde-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d9cde-145">Int32</span></span>|<span data-ttu-id="d9cde-146">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="d9cde-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="d9cde-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d9cde-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d9cde-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9cde-148">DateTimeOffset</span></span>|<span data-ttu-id="d9cde-149">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="d9cde-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="d9cde-150">status</span><span class="sxs-lookup"><span data-stu-id="d9cde-150">status</span></span>|[<span data-ttu-id="d9cde-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d9cde-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d9cde-152">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="d9cde-152">Compliance status of the policy report.</span></span> <span data-ttu-id="d9cde-153">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="d9cde-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d9cde-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9cde-154">lastReportedDateTime</span></span>|<span data-ttu-id="d9cde-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9cde-155">DateTimeOffset</span></span>|<span data-ttu-id="d9cde-156">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="d9cde-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="d9cde-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d9cde-157">userPrincipalName</span></span>|<span data-ttu-id="d9cde-158">String</span><span class="sxs-lookup"><span data-stu-id="d9cde-158">String</span></span>|<span data-ttu-id="d9cde-159">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d9cde-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="d9cde-160">响应</span><span class="sxs-lookup"><span data-stu-id="d9cde-160">Response</span></span>
<span data-ttu-id="d9cde-161">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9cde-161">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9cde-162">示例</span><span class="sxs-lookup"><span data-stu-id="d9cde-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9cde-163">请求</span><span class="sxs-lookup"><span data-stu-id="d9cde-163">Request</span></span>
<span data-ttu-id="d9cde-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9cde-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
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

### <a name="response"></a><span data-ttu-id="d9cde-165">响应</span><span class="sxs-lookup"><span data-stu-id="d9cde-165">Response</span></span>
<span data-ttu-id="d9cde-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9cde-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





