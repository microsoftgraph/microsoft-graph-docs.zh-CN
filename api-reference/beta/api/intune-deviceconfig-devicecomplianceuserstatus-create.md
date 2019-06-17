---
title: 创建 deviceComplianceUserStatus
description: 创建新的 deviceComplianceUserStatus 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f51a534f620252b8fd8536d828ea8a82e79b89db
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968082"
---
# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="50441-103">创建 deviceComplianceUserStatus</span><span class="sxs-lookup"><span data-stu-id="50441-103">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="50441-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50441-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50441-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50441-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50441-106">创建新的 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50441-106">Create a new [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50441-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="50441-107">Prerequisites</span></span>
<span data-ttu-id="50441-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50441-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50441-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="50441-110">Permission type</span></span>|<span data-ttu-id="50441-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="50441-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50441-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50441-112">Delegated (work or school account)</span></span>|<span data-ttu-id="50441-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50441-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50441-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50441-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50441-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="50441-115">Not supported.</span></span>|
|<span data-ttu-id="50441-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="50441-116">Application</span></span>|<span data-ttu-id="50441-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="50441-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50441-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50441-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="50441-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="50441-119">Request headers</span></span>
|<span data-ttu-id="50441-120">标头</span><span class="sxs-lookup"><span data-stu-id="50441-120">Header</span></span>|<span data-ttu-id="50441-121">值</span><span class="sxs-lookup"><span data-stu-id="50441-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50441-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="50441-122">Authorization</span></span>|<span data-ttu-id="50441-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50441-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50441-124">接受</span><span class="sxs-lookup"><span data-stu-id="50441-124">Accept</span></span>|<span data-ttu-id="50441-125">application/json</span><span class="sxs-lookup"><span data-stu-id="50441-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50441-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="50441-126">Request body</span></span>
<span data-ttu-id="50441-127">在请求正文中，提供 deviceComplianceUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50441-127">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="50441-128">下表显示了创建 deviceComplianceUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="50441-128">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="50441-129">属性</span><span class="sxs-lookup"><span data-stu-id="50441-129">Property</span></span>|<span data-ttu-id="50441-130">类型</span><span class="sxs-lookup"><span data-stu-id="50441-130">Type</span></span>|<span data-ttu-id="50441-131">说明</span><span class="sxs-lookup"><span data-stu-id="50441-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50441-132">id</span><span class="sxs-lookup"><span data-stu-id="50441-132">id</span></span>|<span data-ttu-id="50441-133">String</span><span class="sxs-lookup"><span data-stu-id="50441-133">String</span></span>|<span data-ttu-id="50441-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="50441-134">Key of the entity.</span></span>|
|<span data-ttu-id="50441-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="50441-135">userDisplayName</span></span>|<span data-ttu-id="50441-136">String</span><span class="sxs-lookup"><span data-stu-id="50441-136">String</span></span>|<span data-ttu-id="50441-137">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="50441-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="50441-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="50441-138">devicesCount</span></span>|<span data-ttu-id="50441-139">Int32</span><span class="sxs-lookup"><span data-stu-id="50441-139">Int32</span></span>|<span data-ttu-id="50441-140">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="50441-140">Devices count for that user.</span></span>|
|<span data-ttu-id="50441-141">status</span><span class="sxs-lookup"><span data-stu-id="50441-141">status</span></span>|[<span data-ttu-id="50441-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="50441-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="50441-143">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="50441-143">Compliance status of the policy report.</span></span> <span data-ttu-id="50441-144">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="50441-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="50441-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="50441-145">lastReportedDateTime</span></span>|<span data-ttu-id="50441-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50441-146">DateTimeOffset</span></span>|<span data-ttu-id="50441-147">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="50441-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="50441-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="50441-148">userPrincipalName</span></span>|<span data-ttu-id="50441-149">字符串</span><span class="sxs-lookup"><span data-stu-id="50441-149">String</span></span>|<span data-ttu-id="50441-150">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="50441-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="50441-151">响应</span><span class="sxs-lookup"><span data-stu-id="50441-151">Response</span></span>
<span data-ttu-id="50441-152">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50441-152">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50441-153">示例</span><span class="sxs-lookup"><span data-stu-id="50441-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="50441-154">请求</span><span class="sxs-lookup"><span data-stu-id="50441-154">Request</span></span>
<span data-ttu-id="50441-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50441-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50441-156">响应</span><span class="sxs-lookup"><span data-stu-id="50441-156">Response</span></span>
<span data-ttu-id="50441-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50441-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





