---
title: 创建 deviceConfigurationDeviceStatus
description: 创建新的 deviceConfigurationDeviceStatus 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3093d0b2aa3318fc408eb34d6fb80515c805bd1e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752705"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="5b14c-103">创建 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="5b14c-103">Create deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="5b14c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b14c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b14c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b14c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b14c-106">创建新的 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b14c-106">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b14c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="5b14c-107">Prerequisites</span></span>
<span data-ttu-id="5b14c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b14c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b14c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b14c-110">Permission type</span></span>|<span data-ttu-id="5b14c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b14c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b14c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b14c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5b14c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b14c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b14c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b14c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b14c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b14c-115">Not supported.</span></span>|
|<span data-ttu-id="5b14c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b14c-116">Application</span></span>|<span data-ttu-id="5b14c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b14c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b14c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b14c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5b14c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b14c-119">Request headers</span></span>
|<span data-ttu-id="5b14c-120">标头</span><span class="sxs-lookup"><span data-stu-id="5b14c-120">Header</span></span>|<span data-ttu-id="5b14c-121">值</span><span class="sxs-lookup"><span data-stu-id="5b14c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b14c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b14c-122">Authorization</span></span>|<span data-ttu-id="5b14c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5b14c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b14c-124">接受</span><span class="sxs-lookup"><span data-stu-id="5b14c-124">Accept</span></span>|<span data-ttu-id="5b14c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5b14c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b14c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b14c-126">Request body</span></span>
<span data-ttu-id="5b14c-127">在请求正文中，提供 deviceConfigurationDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b14c-127">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="5b14c-128">下表显示创建 deviceConfigurationDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5b14c-128">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="5b14c-129">属性</span><span class="sxs-lookup"><span data-stu-id="5b14c-129">Property</span></span>|<span data-ttu-id="5b14c-130">类型</span><span class="sxs-lookup"><span data-stu-id="5b14c-130">Type</span></span>|<span data-ttu-id="5b14c-131">说明</span><span class="sxs-lookup"><span data-stu-id="5b14c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b14c-132">id</span><span class="sxs-lookup"><span data-stu-id="5b14c-132">id</span></span>|<span data-ttu-id="5b14c-133">String</span><span class="sxs-lookup"><span data-stu-id="5b14c-133">String</span></span>|<span data-ttu-id="5b14c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5b14c-134">Key of the entity.</span></span>|
|<span data-ttu-id="5b14c-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5b14c-135">deviceDisplayName</span></span>|<span data-ttu-id="5b14c-136">String</span><span class="sxs-lookup"><span data-stu-id="5b14c-136">String</span></span>|<span data-ttu-id="5b14c-137">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="5b14c-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="5b14c-138">userName</span><span class="sxs-lookup"><span data-stu-id="5b14c-138">userName</span></span>|<span data-ttu-id="5b14c-139">String</span><span class="sxs-lookup"><span data-stu-id="5b14c-139">String</span></span>|<span data-ttu-id="5b14c-140">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="5b14c-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="5b14c-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="5b14c-141">deviceModel</span></span>|<span data-ttu-id="5b14c-142">String</span><span class="sxs-lookup"><span data-stu-id="5b14c-142">String</span></span>|<span data-ttu-id="5b14c-143">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="5b14c-143">The device model that is being reported</span></span>|
|<span data-ttu-id="5b14c-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5b14c-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="5b14c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b14c-145">DateTimeOffset</span></span>|<span data-ttu-id="5b14c-146">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="5b14c-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="5b14c-147">status</span><span class="sxs-lookup"><span data-stu-id="5b14c-147">status</span></span>|[<span data-ttu-id="5b14c-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5b14c-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5b14c-149">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="5b14c-149">Compliance status of the policy report.</span></span> <span data-ttu-id="5b14c-150">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="5b14c-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5b14c-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b14c-151">lastReportedDateTime</span></span>|<span data-ttu-id="5b14c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b14c-152">DateTimeOffset</span></span>|<span data-ttu-id="5b14c-153">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="5b14c-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="5b14c-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5b14c-154">userPrincipalName</span></span>|<span data-ttu-id="5b14c-155">String</span><span class="sxs-lookup"><span data-stu-id="5b14c-155">String</span></span>|<span data-ttu-id="5b14c-156">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="5b14c-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="5b14c-157">响应</span><span class="sxs-lookup"><span data-stu-id="5b14c-157">Response</span></span>
<span data-ttu-id="5b14c-158">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b14c-158">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b14c-159">示例</span><span class="sxs-lookup"><span data-stu-id="5b14c-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b14c-160">请求</span><span class="sxs-lookup"><span data-stu-id="5b14c-160">Request</span></span>
<span data-ttu-id="5b14c-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b14c-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="5b14c-162">响应</span><span class="sxs-lookup"><span data-stu-id="5b14c-162">Response</span></span>
<span data-ttu-id="5b14c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b14c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




