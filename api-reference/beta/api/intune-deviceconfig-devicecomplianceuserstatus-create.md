---
title: 创建 deviceComplianceUserStatus
description: 创建新的 deviceComplianceUserStatus 对象。
ms.openlocfilehash: 03b2b221ba41c2b8812c6cb0d4e6ec9ab711b583
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048272"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="aed30-103">创建 deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="aed30-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="aed30-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aed30-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aed30-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aed30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aed30-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aed30-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aed30-107">创建新的 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aed30-107">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aed30-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="aed30-108">Prerequisites</span></span>
<span data-ttu-id="aed30-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="aed30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aed30-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aed30-111">Permission type</span></span>|<span data-ttu-id="aed30-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aed30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aed30-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aed30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aed30-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aed30-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aed30-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aed30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aed30-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed30-116">Not supported.</span></span>|
|<span data-ttu-id="aed30-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aed30-117">Application</span></span>|<span data-ttu-id="aed30-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aed30-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aed30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="aed30-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="aed30-120">Request headers</span></span>
|<span data-ttu-id="aed30-121">标头</span><span class="sxs-lookup"><span data-stu-id="aed30-121">Header</span></span>|<span data-ttu-id="aed30-122">值</span><span class="sxs-lookup"><span data-stu-id="aed30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aed30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aed30-123">Authorization</span></span>|<span data-ttu-id="aed30-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aed30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aed30-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aed30-125">Accept</span></span>|<span data-ttu-id="aed30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aed30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aed30-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="aed30-127">Request body</span></span>
<span data-ttu-id="aed30-128">在请求正文中，提供 deviceComplianceUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aed30-128">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="aed30-129">下表显示了创建 deviceComplianceUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aed30-129">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="aed30-130">属性</span><span class="sxs-lookup"><span data-stu-id="aed30-130">Property</span></span>|<span data-ttu-id="aed30-131">类型</span><span class="sxs-lookup"><span data-stu-id="aed30-131">Type</span></span>|<span data-ttu-id="aed30-132">说明</span><span class="sxs-lookup"><span data-stu-id="aed30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aed30-133">id</span><span class="sxs-lookup"><span data-stu-id="aed30-133">id</span></span>|<span data-ttu-id="aed30-134">String</span><span class="sxs-lookup"><span data-stu-id="aed30-134">String</span></span>|<span data-ttu-id="aed30-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aed30-135">Key of the entity.</span></span>|
|<span data-ttu-id="aed30-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="aed30-136">userDisplayName</span></span>|<span data-ttu-id="aed30-137">String</span><span class="sxs-lookup"><span data-stu-id="aed30-137">String</span></span>|<span data-ttu-id="aed30-138">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="aed30-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="aed30-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="aed30-139">devicesCount</span></span>|<span data-ttu-id="aed30-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aed30-140">Int32</span></span>|<span data-ttu-id="aed30-141">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="aed30-141">Devices count for that user.</span></span>|
|<span data-ttu-id="aed30-142">状态</span><span class="sxs-lookup"><span data-stu-id="aed30-142">status</span></span>|[<span data-ttu-id="aed30-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="aed30-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="aed30-144">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="aed30-144">Compliance status of the policy report.</span></span> <span data-ttu-id="aed30-145">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="aed30-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="aed30-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="aed30-146">lastReportedDateTime</span></span>|<span data-ttu-id="aed30-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aed30-147">DateTimeOffset</span></span>|<span data-ttu-id="aed30-148">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="aed30-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="aed30-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="aed30-149">userPrincipalName</span></span>|<span data-ttu-id="aed30-150">String</span><span class="sxs-lookup"><span data-stu-id="aed30-150">String</span></span>|<span data-ttu-id="aed30-151">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="aed30-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="aed30-152">响应</span><span class="sxs-lookup"><span data-stu-id="aed30-152">Response</span></span>
<span data-ttu-id="aed30-153">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aed30-153">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aed30-154">示例</span><span class="sxs-lookup"><span data-stu-id="aed30-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="aed30-155">请求</span><span class="sxs-lookup"><span data-stu-id="aed30-155">Request</span></span>
<span data-ttu-id="aed30-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aed30-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="aed30-157">响应</span><span class="sxs-lookup"><span data-stu-id="aed30-157">Response</span></span>
<span data-ttu-id="aed30-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aed30-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





