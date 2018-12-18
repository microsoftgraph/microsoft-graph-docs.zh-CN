---
title: 更新 deviceComplianceDeviceStatus
description: 更新 deviceComplianceDeviceStatus 对象的属性。
author: tfitzmac
ms.openlocfilehash: 5f894c325e6f7732cb41b7472e85e3dbb8361e3b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343678"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="b0849-103">更新 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b0849-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="b0849-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b0849-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0849-105">更新 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b0849-105">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0849-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0849-106">Prerequisites</span></span>
<span data-ttu-id="b0849-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b0849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0849-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0849-109">Permission type</span></span>|<span data-ttu-id="b0849-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b0849-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0849-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0849-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0849-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0849-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0849-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0849-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0849-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0849-114">Not supported.</span></span>|
|<span data-ttu-id="b0849-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0849-115">Application</span></span>|<span data-ttu-id="b0849-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0849-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0849-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0849-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b0849-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0849-118">Request headers</span></span>
|<span data-ttu-id="b0849-119">标头</span><span class="sxs-lookup"><span data-stu-id="b0849-119">Header</span></span>|<span data-ttu-id="b0849-120">值</span><span class="sxs-lookup"><span data-stu-id="b0849-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0849-121">授权</span><span class="sxs-lookup"><span data-stu-id="b0849-121">Authorization</span></span>|<span data-ttu-id="b0849-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0849-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0849-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b0849-123">Accept</span></span>|<span data-ttu-id="b0849-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b0849-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0849-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0849-125">Request body</span></span>
<span data-ttu-id="b0849-126">在请求正文中，提供 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0849-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="b0849-127">下表显示了创建 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b0849-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="b0849-128">属性</span><span class="sxs-lookup"><span data-stu-id="b0849-128">Property</span></span>|<span data-ttu-id="b0849-129">类型</span><span class="sxs-lookup"><span data-stu-id="b0849-129">Type</span></span>|<span data-ttu-id="b0849-130">说明</span><span class="sxs-lookup"><span data-stu-id="b0849-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0849-131">id</span><span class="sxs-lookup"><span data-stu-id="b0849-131">id</span></span>|<span data-ttu-id="b0849-132">String</span><span class="sxs-lookup"><span data-stu-id="b0849-132">String</span></span>|<span data-ttu-id="b0849-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b0849-133">Key of the entity.</span></span>|
|<span data-ttu-id="b0849-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b0849-134">deviceDisplayName</span></span>|<span data-ttu-id="b0849-135">String</span><span class="sxs-lookup"><span data-stu-id="b0849-135">String</span></span>|<span data-ttu-id="b0849-136">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="b0849-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b0849-137">userName</span><span class="sxs-lookup"><span data-stu-id="b0849-137">userName</span></span>|<span data-ttu-id="b0849-138">String</span><span class="sxs-lookup"><span data-stu-id="b0849-138">String</span></span>|<span data-ttu-id="b0849-139">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="b0849-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="b0849-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b0849-140">deviceModel</span></span>|<span data-ttu-id="b0849-141">String</span><span class="sxs-lookup"><span data-stu-id="b0849-141">String</span></span>|<span data-ttu-id="b0849-142">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="b0849-142">The device model that is being reported</span></span>|
|<span data-ttu-id="b0849-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b0849-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b0849-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0849-144">DateTimeOffset</span></span>|<span data-ttu-id="b0849-145">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="b0849-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b0849-146">status</span><span class="sxs-lookup"><span data-stu-id="b0849-146">status</span></span>|[<span data-ttu-id="b0849-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b0849-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b0849-148">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="b0849-148">Compliance status of the policy report.</span></span> <span data-ttu-id="b0849-149">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b0849-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b0849-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0849-150">lastReportedDateTime</span></span>|<span data-ttu-id="b0849-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0849-151">DateTimeOffset</span></span>|<span data-ttu-id="b0849-152">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="b0849-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b0849-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0849-153">userPrincipalName</span></span>|<span data-ttu-id="b0849-154">String</span><span class="sxs-lookup"><span data-stu-id="b0849-154">String</span></span>|<span data-ttu-id="b0849-155">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b0849-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b0849-156">响应</span><span class="sxs-lookup"><span data-stu-id="b0849-156">Response</span></span>
<span data-ttu-id="b0849-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0849-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0849-158">示例</span><span class="sxs-lookup"><span data-stu-id="b0849-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0849-159">请求</span><span class="sxs-lookup"><span data-stu-id="b0849-159">Request</span></span>
<span data-ttu-id="b0849-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0849-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0849-161">响应</span><span class="sxs-lookup"><span data-stu-id="b0849-161">Response</span></span>
<span data-ttu-id="b0849-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0849-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



