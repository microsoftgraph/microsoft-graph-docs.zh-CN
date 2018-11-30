---
title: 创建 deviceComplianceUserStatus
description: 创建新的 deviceComplianceUserStatus 对象。
ms.openlocfilehash: ab4b20f463ec6d8e30b02ebc8eceb33b9637ed51
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009406"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="811ce-103">创建 deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="811ce-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="811ce-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="811ce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="811ce-105">创建新的 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="811ce-105">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="811ce-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="811ce-106">Prerequisites</span></span>
<span data-ttu-id="811ce-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="811ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="811ce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="811ce-109">Permission type</span></span>|<span data-ttu-id="811ce-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="811ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="811ce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="811ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="811ce-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="811ce-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="811ce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="811ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="811ce-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="811ce-114">Not supported.</span></span>|
|<span data-ttu-id="811ce-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="811ce-115">Application</span></span>|<span data-ttu-id="811ce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="811ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="811ce-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="811ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="811ce-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="811ce-118">Request headers</span></span>
|<span data-ttu-id="811ce-119">标头</span><span class="sxs-lookup"><span data-stu-id="811ce-119">Header</span></span>|<span data-ttu-id="811ce-120">值</span><span class="sxs-lookup"><span data-stu-id="811ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="811ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="811ce-121">Authorization</span></span>|<span data-ttu-id="811ce-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="811ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="811ce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="811ce-123">Accept</span></span>|<span data-ttu-id="811ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="811ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="811ce-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="811ce-125">Request body</span></span>
<span data-ttu-id="811ce-126">在请求正文中，提供 deviceComplianceUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="811ce-126">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="811ce-127">下表显示了创建 deviceComplianceUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="811ce-127">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="811ce-128">属性</span><span class="sxs-lookup"><span data-stu-id="811ce-128">Property</span></span>|<span data-ttu-id="811ce-129">类型</span><span class="sxs-lookup"><span data-stu-id="811ce-129">Type</span></span>|<span data-ttu-id="811ce-130">说明</span><span class="sxs-lookup"><span data-stu-id="811ce-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="811ce-131">id</span><span class="sxs-lookup"><span data-stu-id="811ce-131">id</span></span>|<span data-ttu-id="811ce-132">String</span><span class="sxs-lookup"><span data-stu-id="811ce-132">String</span></span>|<span data-ttu-id="811ce-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="811ce-133">Key of the entity.</span></span>|
|<span data-ttu-id="811ce-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="811ce-134">userDisplayName</span></span>|<span data-ttu-id="811ce-135">String</span><span class="sxs-lookup"><span data-stu-id="811ce-135">String</span></span>|<span data-ttu-id="811ce-136">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="811ce-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="811ce-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="811ce-137">devicesCount</span></span>|<span data-ttu-id="811ce-138">Int32</span><span class="sxs-lookup"><span data-stu-id="811ce-138">Int32</span></span>|<span data-ttu-id="811ce-139">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="811ce-139">Devices count for that user.</span></span>|
|<span data-ttu-id="811ce-140">状态</span><span class="sxs-lookup"><span data-stu-id="811ce-140">status</span></span>|[<span data-ttu-id="811ce-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="811ce-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="811ce-142">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="811ce-142">Compliance status of the policy report.</span></span> <span data-ttu-id="811ce-143">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="811ce-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="811ce-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="811ce-144">lastReportedDateTime</span></span>|<span data-ttu-id="811ce-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="811ce-145">DateTimeOffset</span></span>|<span data-ttu-id="811ce-146">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="811ce-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="811ce-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="811ce-147">userPrincipalName</span></span>|<span data-ttu-id="811ce-148">String</span><span class="sxs-lookup"><span data-stu-id="811ce-148">String</span></span>|<span data-ttu-id="811ce-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="811ce-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="811ce-150">响应</span><span class="sxs-lookup"><span data-stu-id="811ce-150">Response</span></span>
<span data-ttu-id="811ce-151">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="811ce-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="811ce-152">示例</span><span class="sxs-lookup"><span data-stu-id="811ce-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="811ce-153">请求</span><span class="sxs-lookup"><span data-stu-id="811ce-153">Request</span></span>
<span data-ttu-id="811ce-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="811ce-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="811ce-155">响应</span><span class="sxs-lookup"><span data-stu-id="811ce-155">Response</span></span>
<span data-ttu-id="811ce-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="811ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



