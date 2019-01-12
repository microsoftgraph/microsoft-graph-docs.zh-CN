---
title: 更新 deviceComplianceUserStatus
description: 更新 deviceComplianceUserStatus 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a3e3aced0068ceca0f364819db419eb8801a3916
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966767"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="2e80f-103">更新 deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="2e80f-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="2e80f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2e80f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e80f-105">更新 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2e80f-105">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e80f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2e80f-106">Prerequisites</span></span>
<span data-ttu-id="2e80f-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2e80f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e80f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e80f-109">Permission type</span></span>|<span data-ttu-id="2e80f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2e80f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e80f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e80f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e80f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e80f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2e80f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e80f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e80f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e80f-114">Not supported.</span></span>|
|<span data-ttu-id="2e80f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e80f-115">Application</span></span>|<span data-ttu-id="2e80f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e80f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e80f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e80f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2e80f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e80f-118">Request headers</span></span>
|<span data-ttu-id="2e80f-119">标头</span><span class="sxs-lookup"><span data-stu-id="2e80f-119">Header</span></span>|<span data-ttu-id="2e80f-120">值</span><span class="sxs-lookup"><span data-stu-id="2e80f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e80f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e80f-121">Authorization</span></span>|<span data-ttu-id="2e80f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2e80f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e80f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2e80f-123">Accept</span></span>|<span data-ttu-id="2e80f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2e80f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e80f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e80f-125">Request body</span></span>
<span data-ttu-id="2e80f-126">在请求正文中，提供 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e80f-126">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="2e80f-127">下表显示了创建 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2e80f-127">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="2e80f-128">属性</span><span class="sxs-lookup"><span data-stu-id="2e80f-128">Property</span></span>|<span data-ttu-id="2e80f-129">类型</span><span class="sxs-lookup"><span data-stu-id="2e80f-129">Type</span></span>|<span data-ttu-id="2e80f-130">说明</span><span class="sxs-lookup"><span data-stu-id="2e80f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e80f-131">id</span><span class="sxs-lookup"><span data-stu-id="2e80f-131">id</span></span>|<span data-ttu-id="2e80f-132">String</span><span class="sxs-lookup"><span data-stu-id="2e80f-132">String</span></span>|<span data-ttu-id="2e80f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2e80f-133">Key of the entity.</span></span>|
|<span data-ttu-id="2e80f-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2e80f-134">userDisplayName</span></span>|<span data-ttu-id="2e80f-135">String</span><span class="sxs-lookup"><span data-stu-id="2e80f-135">String</span></span>|<span data-ttu-id="2e80f-136">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="2e80f-136">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2e80f-137">devicesCount</span><span class="sxs-lookup"><span data-stu-id="2e80f-137">devicesCount</span></span>|<span data-ttu-id="2e80f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="2e80f-138">Int32</span></span>|<span data-ttu-id="2e80f-139">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="2e80f-139">Devices count for that user.</span></span>|
|<span data-ttu-id="2e80f-140">status</span><span class="sxs-lookup"><span data-stu-id="2e80f-140">status</span></span>|[<span data-ttu-id="2e80f-141">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2e80f-141">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2e80f-142">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="2e80f-142">Compliance status of the policy report.</span></span> <span data-ttu-id="2e80f-143">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="2e80f-143">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2e80f-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e80f-144">lastReportedDateTime</span></span>|<span data-ttu-id="2e80f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e80f-145">DateTimeOffset</span></span>|<span data-ttu-id="2e80f-146">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="2e80f-146">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2e80f-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2e80f-147">userPrincipalName</span></span>|<span data-ttu-id="2e80f-148">String</span><span class="sxs-lookup"><span data-stu-id="2e80f-148">String</span></span>|<span data-ttu-id="2e80f-149">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="2e80f-149">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2e80f-150">响应</span><span class="sxs-lookup"><span data-stu-id="2e80f-150">Response</span></span>
<span data-ttu-id="2e80f-151">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2e80f-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e80f-152">示例</span><span class="sxs-lookup"><span data-stu-id="2e80f-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e80f-153">请求</span><span class="sxs-lookup"><span data-stu-id="2e80f-153">Request</span></span>
<span data-ttu-id="2e80f-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e80f-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
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

### <a name="response"></a><span data-ttu-id="2e80f-155">响应</span><span class="sxs-lookup"><span data-stu-id="2e80f-155">Response</span></span>
<span data-ttu-id="2e80f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e80f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



