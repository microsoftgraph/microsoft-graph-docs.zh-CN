---
title: 更新 deviceComplianceUserStatus
description: 更新 deviceComplianceUserStatus 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 179e220d66c37e21c7d79b51e0c3d7cc9bbd7a66
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37174898"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="598c2-103">更新 deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="598c2-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="598c2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="598c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="598c2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="598c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="598c2-106">更新 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="598c2-106">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="598c2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="598c2-107">Prerequisites</span></span>
<span data-ttu-id="598c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="598c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="598c2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="598c2-110">Permission type</span></span>|<span data-ttu-id="598c2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="598c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="598c2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="598c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="598c2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="598c2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="598c2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="598c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="598c2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="598c2-115">Not supported.</span></span>|
|<span data-ttu-id="598c2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="598c2-116">Application</span></span>|<span data-ttu-id="598c2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="598c2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="598c2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="598c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="598c2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="598c2-119">Request headers</span></span>
|<span data-ttu-id="598c2-120">标头</span><span class="sxs-lookup"><span data-stu-id="598c2-120">Header</span></span>|<span data-ttu-id="598c2-121">值</span><span class="sxs-lookup"><span data-stu-id="598c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="598c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="598c2-122">Authorization</span></span>|<span data-ttu-id="598c2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="598c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="598c2-124">接受</span><span class="sxs-lookup"><span data-stu-id="598c2-124">Accept</span></span>|<span data-ttu-id="598c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="598c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="598c2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="598c2-126">Request body</span></span>
<span data-ttu-id="598c2-127">在请求正文中，提供 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="598c2-127">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="598c2-128">下表显示了创建 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="598c2-128">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="598c2-129">属性</span><span class="sxs-lookup"><span data-stu-id="598c2-129">Property</span></span>|<span data-ttu-id="598c2-130">类型</span><span class="sxs-lookup"><span data-stu-id="598c2-130">Type</span></span>|<span data-ttu-id="598c2-131">说明</span><span class="sxs-lookup"><span data-stu-id="598c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="598c2-132">id</span><span class="sxs-lookup"><span data-stu-id="598c2-132">id</span></span>|<span data-ttu-id="598c2-133">String</span><span class="sxs-lookup"><span data-stu-id="598c2-133">String</span></span>|<span data-ttu-id="598c2-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="598c2-134">Key of the entity.</span></span>|
|<span data-ttu-id="598c2-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="598c2-135">userDisplayName</span></span>|<span data-ttu-id="598c2-136">String</span><span class="sxs-lookup"><span data-stu-id="598c2-136">String</span></span>|<span data-ttu-id="598c2-137">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="598c2-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="598c2-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="598c2-138">devicesCount</span></span>|<span data-ttu-id="598c2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="598c2-139">Int32</span></span>|<span data-ttu-id="598c2-140">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="598c2-140">Devices count for that user.</span></span>|
|<span data-ttu-id="598c2-141">status</span><span class="sxs-lookup"><span data-stu-id="598c2-141">status</span></span>|[<span data-ttu-id="598c2-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="598c2-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="598c2-143">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="598c2-143">Compliance status of the policy report.</span></span> <span data-ttu-id="598c2-144">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="598c2-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="598c2-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="598c2-145">lastReportedDateTime</span></span>|<span data-ttu-id="598c2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="598c2-146">DateTimeOffset</span></span>|<span data-ttu-id="598c2-147">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="598c2-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="598c2-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="598c2-148">userPrincipalName</span></span>|<span data-ttu-id="598c2-149">字符串</span><span class="sxs-lookup"><span data-stu-id="598c2-149">String</span></span>|<span data-ttu-id="598c2-150">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="598c2-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="598c2-151">响应</span><span class="sxs-lookup"><span data-stu-id="598c2-151">Response</span></span>
<span data-ttu-id="598c2-152">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="598c2-152">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="598c2-153">示例</span><span class="sxs-lookup"><span data-stu-id="598c2-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="598c2-154">请求</span><span class="sxs-lookup"><span data-stu-id="598c2-154">Request</span></span>
<span data-ttu-id="598c2-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="598c2-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
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

### <a name="response"></a><span data-ttu-id="598c2-156">响应</span><span class="sxs-lookup"><span data-stu-id="598c2-156">Response</span></span>
<span data-ttu-id="598c2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="598c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




