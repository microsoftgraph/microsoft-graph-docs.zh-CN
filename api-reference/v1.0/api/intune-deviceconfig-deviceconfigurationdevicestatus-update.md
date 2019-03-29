---
title: 更新 deviceConfigurationDeviceStatus
description: 更新 deviceConfigurationDeviceStatus 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eea019b4e22c78accb81ba8d1381074608055d03
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962300"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="8455f-103">更新 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="8455f-103">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="8455f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8455f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8455f-105">更新 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8455f-105">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8455f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="8455f-106">Prerequisites</span></span>
<span data-ttu-id="8455f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8455f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8455f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8455f-109">Permission type</span></span>|<span data-ttu-id="8455f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8455f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8455f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8455f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8455f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8455f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8455f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8455f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8455f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8455f-114">Not supported.</span></span>|
|<span data-ttu-id="8455f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8455f-115">Application</span></span>|<span data-ttu-id="8455f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8455f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8455f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8455f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="8455f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8455f-118">Request headers</span></span>
|<span data-ttu-id="8455f-119">标头</span><span class="sxs-lookup"><span data-stu-id="8455f-119">Header</span></span>|<span data-ttu-id="8455f-120">值</span><span class="sxs-lookup"><span data-stu-id="8455f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8455f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8455f-121">Authorization</span></span>|<span data-ttu-id="8455f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8455f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8455f-123">接受</span><span class="sxs-lookup"><span data-stu-id="8455f-123">Accept</span></span>|<span data-ttu-id="8455f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8455f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8455f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8455f-125">Request body</span></span>
<span data-ttu-id="8455f-126">在请求正文中，提供 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8455f-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="8455f-127">下表显示创建 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8455f-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="8455f-128">属性</span><span class="sxs-lookup"><span data-stu-id="8455f-128">Property</span></span>|<span data-ttu-id="8455f-129">类型</span><span class="sxs-lookup"><span data-stu-id="8455f-129">Type</span></span>|<span data-ttu-id="8455f-130">说明</span><span class="sxs-lookup"><span data-stu-id="8455f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8455f-131">id</span><span class="sxs-lookup"><span data-stu-id="8455f-131">id</span></span>|<span data-ttu-id="8455f-132">String</span><span class="sxs-lookup"><span data-stu-id="8455f-132">String</span></span>|<span data-ttu-id="8455f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8455f-133">Key of the entity.</span></span>|
|<span data-ttu-id="8455f-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8455f-134">deviceDisplayName</span></span>|<span data-ttu-id="8455f-135">String</span><span class="sxs-lookup"><span data-stu-id="8455f-135">String</span></span>|<span data-ttu-id="8455f-136">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="8455f-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="8455f-137">userName</span><span class="sxs-lookup"><span data-stu-id="8455f-137">userName</span></span>|<span data-ttu-id="8455f-138">String</span><span class="sxs-lookup"><span data-stu-id="8455f-138">String</span></span>|<span data-ttu-id="8455f-139">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="8455f-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="8455f-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8455f-140">deviceModel</span></span>|<span data-ttu-id="8455f-141">String</span><span class="sxs-lookup"><span data-stu-id="8455f-141">String</span></span>|<span data-ttu-id="8455f-142">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="8455f-142">The device model that is being reported</span></span>|
|<span data-ttu-id="8455f-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8455f-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="8455f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8455f-144">DateTimeOffset</span></span>|<span data-ttu-id="8455f-145">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="8455f-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="8455f-146">status</span><span class="sxs-lookup"><span data-stu-id="8455f-146">status</span></span>|[<span data-ttu-id="8455f-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8455f-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8455f-148">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="8455f-148">Compliance status of the policy report.</span></span> <span data-ttu-id="8455f-149">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="8455f-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8455f-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="8455f-150">lastReportedDateTime</span></span>|<span data-ttu-id="8455f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8455f-151">DateTimeOffset</span></span>|<span data-ttu-id="8455f-152">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="8455f-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="8455f-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8455f-153">userPrincipalName</span></span>|<span data-ttu-id="8455f-154">String</span><span class="sxs-lookup"><span data-stu-id="8455f-154">String</span></span>|<span data-ttu-id="8455f-155">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="8455f-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="8455f-156">响应</span><span class="sxs-lookup"><span data-stu-id="8455f-156">Response</span></span>
<span data-ttu-id="8455f-157">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8455f-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8455f-158">示例</span><span class="sxs-lookup"><span data-stu-id="8455f-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="8455f-159">请求</span><span class="sxs-lookup"><span data-stu-id="8455f-159">Request</span></span>
<span data-ttu-id="8455f-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8455f-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8455f-161">响应</span><span class="sxs-lookup"><span data-stu-id="8455f-161">Response</span></span>
<span data-ttu-id="8455f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8455f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



