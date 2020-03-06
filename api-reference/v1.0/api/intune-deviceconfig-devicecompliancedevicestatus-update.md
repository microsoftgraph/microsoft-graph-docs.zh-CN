---
title: 更新 deviceComplianceDeviceStatus
description: 更新 deviceComplianceDeviceStatus 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da9f5bf299594a28dc75d6af8a651e33fb257b2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515096"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="796a6-103">更新 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="796a6-103">Update deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="796a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="796a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="796a6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="796a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="796a6-106">更新 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="796a6-106">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="796a6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="796a6-107">Prerequisites</span></span>
<span data-ttu-id="796a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="796a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="796a6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="796a6-110">Permission type</span></span>|<span data-ttu-id="796a6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="796a6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="796a6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="796a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="796a6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="796a6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="796a6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="796a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="796a6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="796a6-115">Not supported.</span></span>|
|<span data-ttu-id="796a6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="796a6-116">Application</span></span>|<span data-ttu-id="796a6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="796a6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="796a6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="796a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="796a6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="796a6-119">Request headers</span></span>
|<span data-ttu-id="796a6-120">标头</span><span class="sxs-lookup"><span data-stu-id="796a6-120">Header</span></span>|<span data-ttu-id="796a6-121">值</span><span class="sxs-lookup"><span data-stu-id="796a6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="796a6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="796a6-122">Authorization</span></span>|<span data-ttu-id="796a6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="796a6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="796a6-124">接受</span><span class="sxs-lookup"><span data-stu-id="796a6-124">Accept</span></span>|<span data-ttu-id="796a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="796a6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="796a6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="796a6-126">Request body</span></span>
<span data-ttu-id="796a6-127">在请求正文中，提供 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="796a6-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="796a6-128">下表显示了创建 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="796a6-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="796a6-129">属性</span><span class="sxs-lookup"><span data-stu-id="796a6-129">Property</span></span>|<span data-ttu-id="796a6-130">类型</span><span class="sxs-lookup"><span data-stu-id="796a6-130">Type</span></span>|<span data-ttu-id="796a6-131">说明</span><span class="sxs-lookup"><span data-stu-id="796a6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="796a6-132">id</span><span class="sxs-lookup"><span data-stu-id="796a6-132">id</span></span>|<span data-ttu-id="796a6-133">String</span><span class="sxs-lookup"><span data-stu-id="796a6-133">String</span></span>|<span data-ttu-id="796a6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="796a6-134">Key of the entity.</span></span>|
|<span data-ttu-id="796a6-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="796a6-135">deviceDisplayName</span></span>|<span data-ttu-id="796a6-136">字符串</span><span class="sxs-lookup"><span data-stu-id="796a6-136">String</span></span>|<span data-ttu-id="796a6-137">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="796a6-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="796a6-138">userName</span><span class="sxs-lookup"><span data-stu-id="796a6-138">userName</span></span>|<span data-ttu-id="796a6-139">字符串</span><span class="sxs-lookup"><span data-stu-id="796a6-139">String</span></span>|<span data-ttu-id="796a6-140">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="796a6-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="796a6-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="796a6-141">deviceModel</span></span>|<span data-ttu-id="796a6-142">String</span><span class="sxs-lookup"><span data-stu-id="796a6-142">String</span></span>|<span data-ttu-id="796a6-143">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="796a6-143">The device model that is being reported</span></span>|
|<span data-ttu-id="796a6-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="796a6-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="796a6-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="796a6-145">DateTimeOffset</span></span>|<span data-ttu-id="796a6-146">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="796a6-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="796a6-147">status</span><span class="sxs-lookup"><span data-stu-id="796a6-147">status</span></span>|[<span data-ttu-id="796a6-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="796a6-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="796a6-149">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="796a6-149">Compliance status of the policy report.</span></span> <span data-ttu-id="796a6-150">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="796a6-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="796a6-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="796a6-151">lastReportedDateTime</span></span>|<span data-ttu-id="796a6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="796a6-152">DateTimeOffset</span></span>|<span data-ttu-id="796a6-153">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="796a6-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="796a6-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="796a6-154">userPrincipalName</span></span>|<span data-ttu-id="796a6-155">字符串</span><span class="sxs-lookup"><span data-stu-id="796a6-155">String</span></span>|<span data-ttu-id="796a6-156">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="796a6-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="796a6-157">响应</span><span class="sxs-lookup"><span data-stu-id="796a6-157">Response</span></span>
<span data-ttu-id="796a6-158">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="796a6-158">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="796a6-159">示例</span><span class="sxs-lookup"><span data-stu-id="796a6-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="796a6-160">请求</span><span class="sxs-lookup"><span data-stu-id="796a6-160">Request</span></span>
<span data-ttu-id="796a6-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="796a6-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="796a6-162">响应</span><span class="sxs-lookup"><span data-stu-id="796a6-162">Response</span></span>
<span data-ttu-id="796a6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="796a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




