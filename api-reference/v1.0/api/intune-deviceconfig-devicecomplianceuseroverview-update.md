---
title: 更新 deviceComplianceUserOverview
description: 更新 deviceComplianceUserOverview 对象的属性。
ms.openlocfilehash: 8bd9ad8c413d6414305cf8648eacee00cca32930
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009903"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="8de7a-103">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="8de7a-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="8de7a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8de7a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8de7a-105">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8de7a-105">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8de7a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="8de7a-106">Prerequisites</span></span>
<span data-ttu-id="8de7a-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="8de7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8de7a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8de7a-109">Permission type</span></span>|<span data-ttu-id="8de7a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8de7a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8de7a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8de7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8de7a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8de7a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8de7a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8de7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8de7a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8de7a-114">Not supported.</span></span>|
|<span data-ttu-id="8de7a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8de7a-115">Application</span></span>|<span data-ttu-id="8de7a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8de7a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8de7a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8de7a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="8de7a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8de7a-118">Request headers</span></span>
|<span data-ttu-id="8de7a-119">标头</span><span class="sxs-lookup"><span data-stu-id="8de7a-119">Header</span></span>|<span data-ttu-id="8de7a-120">值</span><span class="sxs-lookup"><span data-stu-id="8de7a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8de7a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8de7a-121">Authorization</span></span>|<span data-ttu-id="8de7a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8de7a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8de7a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8de7a-123">Accept</span></span>|<span data-ttu-id="8de7a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8de7a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8de7a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8de7a-125">Request body</span></span>
<span data-ttu-id="8de7a-126">在请求正文中，提供 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8de7a-126">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="8de7a-127">下表显示了创建 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8de7a-127">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="8de7a-128">属性</span><span class="sxs-lookup"><span data-stu-id="8de7a-128">Property</span></span>|<span data-ttu-id="8de7a-129">类型</span><span class="sxs-lookup"><span data-stu-id="8de7a-129">Type</span></span>|<span data-ttu-id="8de7a-130">说明</span><span class="sxs-lookup"><span data-stu-id="8de7a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8de7a-131">id</span><span class="sxs-lookup"><span data-stu-id="8de7a-131">id</span></span>|<span data-ttu-id="8de7a-132">String</span><span class="sxs-lookup"><span data-stu-id="8de7a-132">String</span></span>|<span data-ttu-id="8de7a-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8de7a-133">Key of the entity.</span></span>|
|<span data-ttu-id="8de7a-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="8de7a-134">pendingCount</span></span>|<span data-ttu-id="8de7a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="8de7a-135">Int32</span></span>|<span data-ttu-id="8de7a-136">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="8de7a-136">Number of pending Users</span></span>|
|<span data-ttu-id="8de7a-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8de7a-137">notApplicableCount</span></span>|<span data-ttu-id="8de7a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="8de7a-138">Int32</span></span>|<span data-ttu-id="8de7a-139">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="8de7a-139">Number of not applicable users</span></span>|
|<span data-ttu-id="8de7a-140">successCount</span><span class="sxs-lookup"><span data-stu-id="8de7a-140">successCount</span></span>|<span data-ttu-id="8de7a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="8de7a-141">Int32</span></span>|<span data-ttu-id="8de7a-142">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="8de7a-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="8de7a-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="8de7a-143">errorCount</span></span>|<span data-ttu-id="8de7a-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8de7a-144">Int32</span></span>|<span data-ttu-id="8de7a-145">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="8de7a-145">Number of error Users</span></span>|
|<span data-ttu-id="8de7a-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="8de7a-146">failedCount</span></span>|<span data-ttu-id="8de7a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8de7a-147">Int32</span></span>|<span data-ttu-id="8de7a-148">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="8de7a-148">Number of failed Users</span></span>|
|<span data-ttu-id="8de7a-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8de7a-149">lastUpdateDateTime</span></span>|<span data-ttu-id="8de7a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8de7a-150">DateTimeOffset</span></span>|<span data-ttu-id="8de7a-151">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="8de7a-151">Last update time</span></span>|
|<span data-ttu-id="8de7a-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="8de7a-152">configurationVersion</span></span>|<span data-ttu-id="8de7a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8de7a-153">Int32</span></span>|<span data-ttu-id="8de7a-154">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="8de7a-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="8de7a-155">响应</span><span class="sxs-lookup"><span data-stu-id="8de7a-155">Response</span></span>
<span data-ttu-id="8de7a-156">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8de7a-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8de7a-157">示例</span><span class="sxs-lookup"><span data-stu-id="8de7a-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="8de7a-158">请求</span><span class="sxs-lookup"><span data-stu-id="8de7a-158">Request</span></span>
<span data-ttu-id="8de7a-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8de7a-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="8de7a-160">响应</span><span class="sxs-lookup"><span data-stu-id="8de7a-160">Response</span></span>
<span data-ttu-id="8de7a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8de7a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



