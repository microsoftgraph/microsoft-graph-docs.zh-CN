---
title: 更新 deviceComplianceDeviceStatus
description: 更新 deviceComplianceDeviceStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f7c8c00e2d03f49c10a5a37d5c97ba5a611885c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292468"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="b131a-103">更新 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b131a-103">Update deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="b131a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b131a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b131a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b131a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b131a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b131a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b131a-107">更新 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b131a-107">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b131a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b131a-108">Prerequisites</span></span>
<span data-ttu-id="b131a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b131a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b131a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b131a-111">Permission type</span></span>|<span data-ttu-id="b131a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b131a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b131a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b131a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b131a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b131a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b131a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b131a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b131a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b131a-116">Not supported.</span></span>|
|<span data-ttu-id="b131a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b131a-117">Application</span></span>|<span data-ttu-id="b131a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b131a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b131a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b131a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b131a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b131a-120">Request headers</span></span>
|<span data-ttu-id="b131a-121">标头</span><span class="sxs-lookup"><span data-stu-id="b131a-121">Header</span></span>|<span data-ttu-id="b131a-122">值</span><span class="sxs-lookup"><span data-stu-id="b131a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b131a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b131a-123">Authorization</span></span>|<span data-ttu-id="b131a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b131a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b131a-125">接受</span><span class="sxs-lookup"><span data-stu-id="b131a-125">Accept</span></span>|<span data-ttu-id="b131a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b131a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b131a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b131a-127">Request body</span></span>
<span data-ttu-id="b131a-128">在请求正文中，提供 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b131a-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="b131a-129">下表显示了创建 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b131a-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="b131a-130">属性</span><span class="sxs-lookup"><span data-stu-id="b131a-130">Property</span></span>|<span data-ttu-id="b131a-131">类型</span><span class="sxs-lookup"><span data-stu-id="b131a-131">Type</span></span>|<span data-ttu-id="b131a-132">说明</span><span class="sxs-lookup"><span data-stu-id="b131a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b131a-133">id</span><span class="sxs-lookup"><span data-stu-id="b131a-133">id</span></span>|<span data-ttu-id="b131a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b131a-134">String</span></span>|<span data-ttu-id="b131a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b131a-135">Key of the entity.</span></span>|
|<span data-ttu-id="b131a-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b131a-136">deviceDisplayName</span></span>|<span data-ttu-id="b131a-137">String</span><span class="sxs-lookup"><span data-stu-id="b131a-137">String</span></span>|<span data-ttu-id="b131a-138">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="b131a-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b131a-139">userName</span><span class="sxs-lookup"><span data-stu-id="b131a-139">userName</span></span>|<span data-ttu-id="b131a-140">String</span><span class="sxs-lookup"><span data-stu-id="b131a-140">String</span></span>|<span data-ttu-id="b131a-141">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="b131a-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="b131a-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b131a-142">deviceModel</span></span>|<span data-ttu-id="b131a-143">String</span><span class="sxs-lookup"><span data-stu-id="b131a-143">String</span></span>|<span data-ttu-id="b131a-144">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="b131a-144">The device model that is being reported</span></span>|
|<span data-ttu-id="b131a-145">平台</span><span class="sxs-lookup"><span data-stu-id="b131a-145">platform</span></span>|<span data-ttu-id="b131a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b131a-146">Int32</span></span>|<span data-ttu-id="b131a-147">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="b131a-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="b131a-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b131a-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b131a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b131a-149">DateTimeOffset</span></span>|<span data-ttu-id="b131a-150">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="b131a-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b131a-151">status</span><span class="sxs-lookup"><span data-stu-id="b131a-151">status</span></span>|[<span data-ttu-id="b131a-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b131a-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b131a-153">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="b131a-153">Compliance status of the policy report.</span></span> <span data-ttu-id="b131a-154">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b131a-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b131a-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b131a-155">lastReportedDateTime</span></span>|<span data-ttu-id="b131a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b131a-156">DateTimeOffset</span></span>|<span data-ttu-id="b131a-157">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="b131a-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b131a-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b131a-158">userPrincipalName</span></span>|<span data-ttu-id="b131a-159">字符串</span><span class="sxs-lookup"><span data-stu-id="b131a-159">String</span></span>|<span data-ttu-id="b131a-160">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b131a-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b131a-161">响应</span><span class="sxs-lookup"><span data-stu-id="b131a-161">Response</span></span>
<span data-ttu-id="b131a-162">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b131a-162">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b131a-163">示例</span><span class="sxs-lookup"><span data-stu-id="b131a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="b131a-164">请求</span><span class="sxs-lookup"><span data-stu-id="b131a-164">Request</span></span>
<span data-ttu-id="b131a-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b131a-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b131a-166">响应</span><span class="sxs-lookup"><span data-stu-id="b131a-166">Response</span></span>
<span data-ttu-id="b131a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b131a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




