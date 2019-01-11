---
title: 更新 deviceComplianceUserStatus
description: 更新 deviceComplianceUserStatus 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 40d58158ca3a0e17f7f92b15a35f1b730d2511c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852799"
---
# <a name="update-devicecomplianceuserstatus"></a><span data-ttu-id="fb0f2-103">更新 deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="fb0f2-103">Update deviceComplianceUserStatus</span></span>

> <span data-ttu-id="fb0f2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb0f2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb0f2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb0f2-107">更新 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-107">Update the properties of a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fb0f2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb0f2-108">Prerequisites</span></span>
<span data-ttu-id="fb0f2-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fb0f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb0f2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb0f2-111">Permission type</span></span>|<span data-ttu-id="fb0f2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb0f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb0f2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb0f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb0f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb0f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb0f2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb0f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb0f2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-116">Not supported.</span></span>|
|<span data-ttu-id="fb0f2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb0f2-117">Application</span></span>|<span data-ttu-id="fb0f2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb0f2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb0f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="fb0f2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb0f2-120">Request headers</span></span>
|<span data-ttu-id="fb0f2-121">标头</span><span class="sxs-lookup"><span data-stu-id="fb0f2-121">Header</span></span>|<span data-ttu-id="fb0f2-122">值</span><span class="sxs-lookup"><span data-stu-id="fb0f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb0f2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb0f2-123">Authorization</span></span>|<span data-ttu-id="fb0f2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb0f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb0f2-125">Accept</span></span>|<span data-ttu-id="fb0f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb0f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb0f2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb0f2-127">Request body</span></span>
<span data-ttu-id="fb0f2-128">在请求正文中，提供 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-128">In the request body, supply a JSON representation for the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

<span data-ttu-id="fb0f2-129">下表显示了创建 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-129">The following table shows the properties that are required when you create the [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md).</span></span>

|<span data-ttu-id="fb0f2-130">属性</span><span class="sxs-lookup"><span data-stu-id="fb0f2-130">Property</span></span>|<span data-ttu-id="fb0f2-131">类型</span><span class="sxs-lookup"><span data-stu-id="fb0f2-131">Type</span></span>|<span data-ttu-id="fb0f2-132">说明</span><span class="sxs-lookup"><span data-stu-id="fb0f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb0f2-133">id</span><span class="sxs-lookup"><span data-stu-id="fb0f2-133">id</span></span>|<span data-ttu-id="fb0f2-134">String</span><span class="sxs-lookup"><span data-stu-id="fb0f2-134">String</span></span>|<span data-ttu-id="fb0f2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-135">Key of the entity.</span></span>|
|<span data-ttu-id="fb0f2-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fb0f2-136">userDisplayName</span></span>|<span data-ttu-id="fb0f2-137">String</span><span class="sxs-lookup"><span data-stu-id="fb0f2-137">String</span></span>|<span data-ttu-id="fb0f2-138">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="fb0f2-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="fb0f2-139">devicesCount</span></span>|<span data-ttu-id="fb0f2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="fb0f2-140">Int32</span></span>|<span data-ttu-id="fb0f2-141">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-141">Devices count for that user.</span></span>|
|<span data-ttu-id="fb0f2-142">status</span><span class="sxs-lookup"><span data-stu-id="fb0f2-142">status</span></span>|[<span data-ttu-id="fb0f2-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fb0f2-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="fb0f2-144">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-144">Compliance status of the policy report.</span></span> <span data-ttu-id="fb0f2-145">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fb0f2-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb0f2-146">lastReportedDateTime</span></span>|<span data-ttu-id="fb0f2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb0f2-147">DateTimeOffset</span></span>|<span data-ttu-id="fb0f2-148">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="fb0f2-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fb0f2-149">userPrincipalName</span></span>|<span data-ttu-id="fb0f2-150">String</span><span class="sxs-lookup"><span data-stu-id="fb0f2-150">String</span></span>|<span data-ttu-id="fb0f2-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="fb0f2-152">响应</span><span class="sxs-lookup"><span data-stu-id="fb0f2-152">Response</span></span>
<span data-ttu-id="fb0f2-153">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-153">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb0f2-154">示例</span><span class="sxs-lookup"><span data-stu-id="fb0f2-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="fb0f2-155">请求</span><span class="sxs-lookup"><span data-stu-id="fb0f2-155">Request</span></span>
<span data-ttu-id="fb0f2-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses/{deviceComplianceUserStatusId}
Content-type: application/json
Content-length: 222

{
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="fb0f2-157">响应</span><span class="sxs-lookup"><span data-stu-id="fb0f2-157">Response</span></span>
<span data-ttu-id="fb0f2-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb0f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





