---
title: 创建 deviceConfigurationDeviceStatus
description: 创建新的 deviceConfigurationDeviceStatus 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 847363fa484de3ea1c210d5e6bd0918721db45b1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984266"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="b926a-103">创建 deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b926a-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="b926a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b926a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b926a-105">创建新的 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b926a-105">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b926a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b926a-106">Prerequisites</span></span>
<span data-ttu-id="b926a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b926a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b926a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b926a-109">Permission type</span></span>|<span data-ttu-id="b926a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b926a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b926a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b926a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b926a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b926a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b926a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b926a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b926a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b926a-114">Not supported.</span></span>|
|<span data-ttu-id="b926a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b926a-115">Application</span></span>|<span data-ttu-id="b926a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b926a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b926a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b926a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b926a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b926a-118">Request headers</span></span>
|<span data-ttu-id="b926a-119">标头</span><span class="sxs-lookup"><span data-stu-id="b926a-119">Header</span></span>|<span data-ttu-id="b926a-120">值</span><span class="sxs-lookup"><span data-stu-id="b926a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b926a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b926a-121">Authorization</span></span>|<span data-ttu-id="b926a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b926a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b926a-123">接受</span><span class="sxs-lookup"><span data-stu-id="b926a-123">Accept</span></span>|<span data-ttu-id="b926a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b926a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b926a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b926a-125">Request body</span></span>
<span data-ttu-id="b926a-126">在请求正文中，提供 deviceConfigurationDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b926a-126">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="b926a-127">下表显示创建 deviceConfigurationDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b926a-127">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="b926a-128">属性</span><span class="sxs-lookup"><span data-stu-id="b926a-128">Property</span></span>|<span data-ttu-id="b926a-129">类型</span><span class="sxs-lookup"><span data-stu-id="b926a-129">Type</span></span>|<span data-ttu-id="b926a-130">说明</span><span class="sxs-lookup"><span data-stu-id="b926a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b926a-131">id</span><span class="sxs-lookup"><span data-stu-id="b926a-131">id</span></span>|<span data-ttu-id="b926a-132">String</span><span class="sxs-lookup"><span data-stu-id="b926a-132">String</span></span>|<span data-ttu-id="b926a-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b926a-133">Key of the entity.</span></span>|
|<span data-ttu-id="b926a-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b926a-134">deviceDisplayName</span></span>|<span data-ttu-id="b926a-135">String</span><span class="sxs-lookup"><span data-stu-id="b926a-135">String</span></span>|<span data-ttu-id="b926a-136">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="b926a-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b926a-137">userName</span><span class="sxs-lookup"><span data-stu-id="b926a-137">userName</span></span>|<span data-ttu-id="b926a-138">String</span><span class="sxs-lookup"><span data-stu-id="b926a-138">String</span></span>|<span data-ttu-id="b926a-139">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="b926a-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="b926a-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b926a-140">deviceModel</span></span>|<span data-ttu-id="b926a-141">String</span><span class="sxs-lookup"><span data-stu-id="b926a-141">String</span></span>|<span data-ttu-id="b926a-142">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="b926a-142">The device model that is being reported</span></span>|
|<span data-ttu-id="b926a-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b926a-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b926a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b926a-144">DateTimeOffset</span></span>|<span data-ttu-id="b926a-145">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="b926a-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b926a-146">status</span><span class="sxs-lookup"><span data-stu-id="b926a-146">status</span></span>|[<span data-ttu-id="b926a-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b926a-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b926a-148">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="b926a-148">Compliance status of the policy report.</span></span> <span data-ttu-id="b926a-149">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b926a-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b926a-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b926a-150">lastReportedDateTime</span></span>|<span data-ttu-id="b926a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b926a-151">DateTimeOffset</span></span>|<span data-ttu-id="b926a-152">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="b926a-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b926a-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b926a-153">userPrincipalName</span></span>|<span data-ttu-id="b926a-154">String</span><span class="sxs-lookup"><span data-stu-id="b926a-154">String</span></span>|<span data-ttu-id="b926a-155">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b926a-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b926a-156">响应</span><span class="sxs-lookup"><span data-stu-id="b926a-156">Response</span></span>
<span data-ttu-id="b926a-157">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b926a-157">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b926a-158">示例</span><span class="sxs-lookup"><span data-stu-id="b926a-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b926a-159">请求</span><span class="sxs-lookup"><span data-stu-id="b926a-159">Request</span></span>
<span data-ttu-id="b926a-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b926a-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b926a-161">响应</span><span class="sxs-lookup"><span data-stu-id="b926a-161">Response</span></span>
<span data-ttu-id="b926a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b926a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



