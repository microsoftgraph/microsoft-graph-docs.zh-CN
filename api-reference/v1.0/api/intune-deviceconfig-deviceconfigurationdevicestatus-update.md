---
title: 更新 deviceConfigurationDeviceStatus
description: 更新 deviceConfigurationDeviceStatus 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 34fefa2da07c62c31247e290f962e0e521caa0a6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753907"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="4d875-103">更新 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="4d875-103">Update deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="4d875-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d875-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d875-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d875-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d875-106">更新 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4d875-106">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d875-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d875-107">Prerequisites</span></span>
<span data-ttu-id="4d875-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d875-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d875-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d875-110">Permission type</span></span>|<span data-ttu-id="4d875-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d875-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d875-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d875-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d875-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d875-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d875-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d875-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d875-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d875-115">Not supported.</span></span>|
|<span data-ttu-id="4d875-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d875-116">Application</span></span>|<span data-ttu-id="4d875-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d875-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d875-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d875-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="4d875-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d875-119">Request headers</span></span>
|<span data-ttu-id="4d875-120">标头</span><span class="sxs-lookup"><span data-stu-id="4d875-120">Header</span></span>|<span data-ttu-id="4d875-121">值</span><span class="sxs-lookup"><span data-stu-id="4d875-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d875-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d875-122">Authorization</span></span>|<span data-ttu-id="4d875-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d875-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d875-124">接受</span><span class="sxs-lookup"><span data-stu-id="4d875-124">Accept</span></span>|<span data-ttu-id="4d875-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d875-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d875-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d875-126">Request body</span></span>
<span data-ttu-id="4d875-127">在请求正文中，提供 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d875-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="4d875-128">下表显示创建 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4d875-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="4d875-129">属性</span><span class="sxs-lookup"><span data-stu-id="4d875-129">Property</span></span>|<span data-ttu-id="4d875-130">类型</span><span class="sxs-lookup"><span data-stu-id="4d875-130">Type</span></span>|<span data-ttu-id="4d875-131">说明</span><span class="sxs-lookup"><span data-stu-id="4d875-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d875-132">id</span><span class="sxs-lookup"><span data-stu-id="4d875-132">id</span></span>|<span data-ttu-id="4d875-133">String</span><span class="sxs-lookup"><span data-stu-id="4d875-133">String</span></span>|<span data-ttu-id="4d875-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4d875-134">Key of the entity.</span></span>|
|<span data-ttu-id="4d875-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4d875-135">deviceDisplayName</span></span>|<span data-ttu-id="4d875-136">String</span><span class="sxs-lookup"><span data-stu-id="4d875-136">String</span></span>|<span data-ttu-id="4d875-137">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="4d875-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4d875-138">userName</span><span class="sxs-lookup"><span data-stu-id="4d875-138">userName</span></span>|<span data-ttu-id="4d875-139">String</span><span class="sxs-lookup"><span data-stu-id="4d875-139">String</span></span>|<span data-ttu-id="4d875-140">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="4d875-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="4d875-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="4d875-141">deviceModel</span></span>|<span data-ttu-id="4d875-142">String</span><span class="sxs-lookup"><span data-stu-id="4d875-142">String</span></span>|<span data-ttu-id="4d875-143">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="4d875-143">The device model that is being reported</span></span>|
|<span data-ttu-id="4d875-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4d875-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4d875-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d875-145">DateTimeOffset</span></span>|<span data-ttu-id="4d875-146">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="4d875-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="4d875-147">status</span><span class="sxs-lookup"><span data-stu-id="4d875-147">status</span></span>|[<span data-ttu-id="4d875-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4d875-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4d875-149">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="4d875-149">Compliance status of the policy report.</span></span> <span data-ttu-id="4d875-150">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="4d875-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4d875-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d875-151">lastReportedDateTime</span></span>|<span data-ttu-id="4d875-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d875-152">DateTimeOffset</span></span>|<span data-ttu-id="4d875-153">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="4d875-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4d875-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4d875-154">userPrincipalName</span></span>|<span data-ttu-id="4d875-155">String</span><span class="sxs-lookup"><span data-stu-id="4d875-155">String</span></span>|<span data-ttu-id="4d875-156">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="4d875-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4d875-157">响应</span><span class="sxs-lookup"><span data-stu-id="4d875-157">Response</span></span>
<span data-ttu-id="4d875-158">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d875-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d875-159">示例</span><span class="sxs-lookup"><span data-stu-id="4d875-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d875-160">请求</span><span class="sxs-lookup"><span data-stu-id="4d875-160">Request</span></span>
<span data-ttu-id="4d875-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d875-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="4d875-162">响应</span><span class="sxs-lookup"><span data-stu-id="4d875-162">Response</span></span>
<span data-ttu-id="4d875-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d875-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




