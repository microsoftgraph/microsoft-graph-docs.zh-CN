---
title: 创建 deviceComplianceDeviceStatus
description: 创建新的 deviceComplianceDeviceStatus 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77675e82f920a955ac04a8fdab1ab993e01f2fee
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756636"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="f9e7b-103">创建 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f9e7b-103">Create deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="f9e7b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9e7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9e7b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9e7b-106">创建新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-106">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9e7b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9e7b-107">Prerequisites</span></span>
<span data-ttu-id="f9e7b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9e7b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9e7b-110">Permission type</span></span>|<span data-ttu-id="f9e7b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9e7b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9e7b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9e7b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9e7b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9e7b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9e7b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9e7b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9e7b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-115">Not supported.</span></span>|
|<span data-ttu-id="f9e7b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9e7b-116">Application</span></span>|<span data-ttu-id="f9e7b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9e7b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9e7b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9e7b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f9e7b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9e7b-119">Request headers</span></span>
|<span data-ttu-id="f9e7b-120">标头</span><span class="sxs-lookup"><span data-stu-id="f9e7b-120">Header</span></span>|<span data-ttu-id="f9e7b-121">值</span><span class="sxs-lookup"><span data-stu-id="f9e7b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9e7b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9e7b-122">Authorization</span></span>|<span data-ttu-id="f9e7b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9e7b-124">接受</span><span class="sxs-lookup"><span data-stu-id="f9e7b-124">Accept</span></span>|<span data-ttu-id="f9e7b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9e7b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9e7b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9e7b-126">Request body</span></span>
<span data-ttu-id="f9e7b-127">在请求正文中，提供 deviceComplianceDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-127">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="f9e7b-128">下表显示创建 deviceComplianceDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-128">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="f9e7b-129">属性</span><span class="sxs-lookup"><span data-stu-id="f9e7b-129">Property</span></span>|<span data-ttu-id="f9e7b-130">类型</span><span class="sxs-lookup"><span data-stu-id="f9e7b-130">Type</span></span>|<span data-ttu-id="f9e7b-131">说明</span><span class="sxs-lookup"><span data-stu-id="f9e7b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9e7b-132">id</span><span class="sxs-lookup"><span data-stu-id="f9e7b-132">id</span></span>|<span data-ttu-id="f9e7b-133">String</span><span class="sxs-lookup"><span data-stu-id="f9e7b-133">String</span></span>|<span data-ttu-id="f9e7b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-134">Key of the entity.</span></span>|
|<span data-ttu-id="f9e7b-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9e7b-135">deviceDisplayName</span></span>|<span data-ttu-id="f9e7b-136">String</span><span class="sxs-lookup"><span data-stu-id="f9e7b-136">String</span></span>|<span data-ttu-id="f9e7b-137">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f9e7b-138">userName</span><span class="sxs-lookup"><span data-stu-id="f9e7b-138">userName</span></span>|<span data-ttu-id="f9e7b-139">String</span><span class="sxs-lookup"><span data-stu-id="f9e7b-139">String</span></span>|<span data-ttu-id="f9e7b-140">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="f9e7b-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="f9e7b-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f9e7b-141">deviceModel</span></span>|<span data-ttu-id="f9e7b-142">String</span><span class="sxs-lookup"><span data-stu-id="f9e7b-142">String</span></span>|<span data-ttu-id="f9e7b-143">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="f9e7b-143">The device model that is being reported</span></span>|
|<span data-ttu-id="f9e7b-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f9e7b-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f9e7b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9e7b-145">DateTimeOffset</span></span>|<span data-ttu-id="f9e7b-146">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="f9e7b-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f9e7b-147">status</span><span class="sxs-lookup"><span data-stu-id="f9e7b-147">status</span></span>|[<span data-ttu-id="f9e7b-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f9e7b-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f9e7b-149">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-149">Compliance status of the policy report.</span></span> <span data-ttu-id="f9e7b-150">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f9e7b-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9e7b-151">lastReportedDateTime</span></span>|<span data-ttu-id="f9e7b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9e7b-152">DateTimeOffset</span></span>|<span data-ttu-id="f9e7b-153">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f9e7b-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9e7b-154">userPrincipalName</span></span>|<span data-ttu-id="f9e7b-155">String</span><span class="sxs-lookup"><span data-stu-id="f9e7b-155">String</span></span>|<span data-ttu-id="f9e7b-156">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f9e7b-157">响应</span><span class="sxs-lookup"><span data-stu-id="f9e7b-157">Response</span></span>
<span data-ttu-id="f9e7b-158">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和更新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-158">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9e7b-159">示例</span><span class="sxs-lookup"><span data-stu-id="f9e7b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9e7b-160">请求</span><span class="sxs-lookup"><span data-stu-id="f9e7b-160">Request</span></span>
<span data-ttu-id="f9e7b-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="f9e7b-162">响应</span><span class="sxs-lookup"><span data-stu-id="f9e7b-162">Response</span></span>
<span data-ttu-id="f9e7b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9e7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




