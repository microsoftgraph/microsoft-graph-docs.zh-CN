---
title: 更新 deviceConfigurationDeviceStatus
description: 更新 deviceConfigurationDeviceStatus 对象的属性。
author: tfitzmac
ms.openlocfilehash: 26d66b7821454a7d8b77245b736dbbf62c44590f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315559"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="2322e-103">更新 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2322e-103">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="2322e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2322e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2322e-105">更新 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2322e-105">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2322e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2322e-106">Prerequisites</span></span>
<span data-ttu-id="2322e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2322e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2322e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2322e-109">Permission type</span></span>|<span data-ttu-id="2322e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2322e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2322e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2322e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2322e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2322e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2322e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2322e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2322e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2322e-114">Not supported.</span></span>|
|<span data-ttu-id="2322e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2322e-115">Application</span></span>|<span data-ttu-id="2322e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2322e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2322e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2322e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2322e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2322e-118">Request headers</span></span>
|<span data-ttu-id="2322e-119">标头</span><span class="sxs-lookup"><span data-stu-id="2322e-119">Header</span></span>|<span data-ttu-id="2322e-120">值</span><span class="sxs-lookup"><span data-stu-id="2322e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2322e-121">授权</span><span class="sxs-lookup"><span data-stu-id="2322e-121">Authorization</span></span>|<span data-ttu-id="2322e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2322e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2322e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2322e-123">Accept</span></span>|<span data-ttu-id="2322e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2322e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2322e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2322e-125">Request body</span></span>
<span data-ttu-id="2322e-126">在请求正文中，提供 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2322e-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="2322e-127">下表显示创建 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2322e-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="2322e-128">属性</span><span class="sxs-lookup"><span data-stu-id="2322e-128">Property</span></span>|<span data-ttu-id="2322e-129">类型</span><span class="sxs-lookup"><span data-stu-id="2322e-129">Type</span></span>|<span data-ttu-id="2322e-130">说明</span><span class="sxs-lookup"><span data-stu-id="2322e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2322e-131">id</span><span class="sxs-lookup"><span data-stu-id="2322e-131">id</span></span>|<span data-ttu-id="2322e-132">String</span><span class="sxs-lookup"><span data-stu-id="2322e-132">String</span></span>|<span data-ttu-id="2322e-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2322e-133">Key of the entity.</span></span>|
|<span data-ttu-id="2322e-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2322e-134">deviceDisplayName</span></span>|<span data-ttu-id="2322e-135">String</span><span class="sxs-lookup"><span data-stu-id="2322e-135">String</span></span>|<span data-ttu-id="2322e-136">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="2322e-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2322e-137">userName</span><span class="sxs-lookup"><span data-stu-id="2322e-137">userName</span></span>|<span data-ttu-id="2322e-138">String</span><span class="sxs-lookup"><span data-stu-id="2322e-138">String</span></span>|<span data-ttu-id="2322e-139">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="2322e-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="2322e-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2322e-140">deviceModel</span></span>|<span data-ttu-id="2322e-141">String</span><span class="sxs-lookup"><span data-stu-id="2322e-141">String</span></span>|<span data-ttu-id="2322e-142">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="2322e-142">The device model that is being reported</span></span>|
|<span data-ttu-id="2322e-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2322e-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2322e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2322e-144">DateTimeOffset</span></span>|<span data-ttu-id="2322e-145">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="2322e-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2322e-146">status</span><span class="sxs-lookup"><span data-stu-id="2322e-146">status</span></span>|[<span data-ttu-id="2322e-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2322e-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2322e-148">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="2322e-148">Compliance status of the policy report.</span></span> <span data-ttu-id="2322e-149">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="2322e-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2322e-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2322e-150">lastReportedDateTime</span></span>|<span data-ttu-id="2322e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2322e-151">DateTimeOffset</span></span>|<span data-ttu-id="2322e-152">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="2322e-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2322e-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2322e-153">userPrincipalName</span></span>|<span data-ttu-id="2322e-154">String</span><span class="sxs-lookup"><span data-stu-id="2322e-154">String</span></span>|<span data-ttu-id="2322e-155">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="2322e-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2322e-156">响应</span><span class="sxs-lookup"><span data-stu-id="2322e-156">Response</span></span>
<span data-ttu-id="2322e-157">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2322e-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2322e-158">示例</span><span class="sxs-lookup"><span data-stu-id="2322e-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="2322e-159">请求</span><span class="sxs-lookup"><span data-stu-id="2322e-159">Request</span></span>
<span data-ttu-id="2322e-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2322e-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2322e-161">响应</span><span class="sxs-lookup"><span data-stu-id="2322e-161">Response</span></span>
<span data-ttu-id="2322e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2322e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



