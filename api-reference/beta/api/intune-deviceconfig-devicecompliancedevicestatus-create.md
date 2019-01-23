---
title: 创建 deviceComplianceDeviceStatus
description: 创建新的 deviceComplianceDeviceStatus 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0b9e7a7049c656c42f2ad843bedafcc6f9975619
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417572"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="05084-103">创建 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="05084-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="05084-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="05084-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="05084-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="05084-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05084-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05084-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05084-107">创建新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05084-107">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05084-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="05084-108">Prerequisites</span></span>
<span data-ttu-id="05084-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="05084-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="05084-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="05084-111">Permission type</span></span>|<span data-ttu-id="05084-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05084-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05084-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05084-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05084-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05084-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05084-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05084-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05084-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="05084-116">Not supported.</span></span>|
|<span data-ttu-id="05084-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="05084-117">Application</span></span>|<span data-ttu-id="05084-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="05084-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05084-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05084-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="05084-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05084-120">Request headers</span></span>
|<span data-ttu-id="05084-121">标头</span><span class="sxs-lookup"><span data-stu-id="05084-121">Header</span></span>|<span data-ttu-id="05084-122">值</span><span class="sxs-lookup"><span data-stu-id="05084-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05084-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05084-123">Authorization</span></span>|<span data-ttu-id="05084-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05084-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05084-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05084-125">Accept</span></span>|<span data-ttu-id="05084-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05084-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05084-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05084-127">Request body</span></span>
<span data-ttu-id="05084-128">在请求正文中，提供 deviceComplianceDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05084-128">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="05084-129">下表显示创建 deviceComplianceDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="05084-129">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="05084-130">属性</span><span class="sxs-lookup"><span data-stu-id="05084-130">Property</span></span>|<span data-ttu-id="05084-131">类型</span><span class="sxs-lookup"><span data-stu-id="05084-131">Type</span></span>|<span data-ttu-id="05084-132">说明</span><span class="sxs-lookup"><span data-stu-id="05084-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05084-133">id</span><span class="sxs-lookup"><span data-stu-id="05084-133">id</span></span>|<span data-ttu-id="05084-134">String</span><span class="sxs-lookup"><span data-stu-id="05084-134">String</span></span>|<span data-ttu-id="05084-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="05084-135">Key of the entity.</span></span>|
|<span data-ttu-id="05084-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="05084-136">deviceDisplayName</span></span>|<span data-ttu-id="05084-137">String</span><span class="sxs-lookup"><span data-stu-id="05084-137">String</span></span>|<span data-ttu-id="05084-138">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="05084-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="05084-139">userName</span><span class="sxs-lookup"><span data-stu-id="05084-139">userName</span></span>|<span data-ttu-id="05084-140">String</span><span class="sxs-lookup"><span data-stu-id="05084-140">String</span></span>|<span data-ttu-id="05084-141">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="05084-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="05084-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="05084-142">deviceModel</span></span>|<span data-ttu-id="05084-143">String</span><span class="sxs-lookup"><span data-stu-id="05084-143">String</span></span>|<span data-ttu-id="05084-144">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="05084-144">The device model that is being reported</span></span>|
|<span data-ttu-id="05084-145">platform</span><span class="sxs-lookup"><span data-stu-id="05084-145">platform</span></span>|<span data-ttu-id="05084-146">Int32</span><span class="sxs-lookup"><span data-stu-id="05084-146">Int32</span></span>|<span data-ttu-id="05084-147">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="05084-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="05084-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="05084-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="05084-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05084-149">DateTimeOffset</span></span>|<span data-ttu-id="05084-150">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="05084-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="05084-151">status</span><span class="sxs-lookup"><span data-stu-id="05084-151">status</span></span>|[<span data-ttu-id="05084-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="05084-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="05084-153">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="05084-153">Compliance status of the policy report.</span></span> <span data-ttu-id="05084-154">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="05084-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="05084-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="05084-155">lastReportedDateTime</span></span>|<span data-ttu-id="05084-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05084-156">DateTimeOffset</span></span>|<span data-ttu-id="05084-157">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="05084-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="05084-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05084-158">userPrincipalName</span></span>|<span data-ttu-id="05084-159">String</span><span class="sxs-lookup"><span data-stu-id="05084-159">String</span></span>|<span data-ttu-id="05084-160">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="05084-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="05084-161">响应</span><span class="sxs-lookup"><span data-stu-id="05084-161">Response</span></span>
<span data-ttu-id="05084-162">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和更新的 [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05084-162">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05084-163">示例</span><span class="sxs-lookup"><span data-stu-id="05084-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="05084-164">请求</span><span class="sxs-lookup"><span data-stu-id="05084-164">Request</span></span>
<span data-ttu-id="05084-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05084-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05084-166">响应</span><span class="sxs-lookup"><span data-stu-id="05084-166">Response</span></span>
<span data-ttu-id="05084-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05084-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




