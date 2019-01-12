---
title: 更新 deviceComplianceUserOverview
description: 更新 deviceComplianceUserOverview 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1a7cfc6bbcb28636e0f5fe8568e1be619f92eb78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946264"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="f763c-103">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="f763c-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="f763c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f763c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f763c-105">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f763c-105">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f763c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f763c-106">Prerequisites</span></span>
<span data-ttu-id="f763c-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f763c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f763c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f763c-109">Permission type</span></span>|<span data-ttu-id="f763c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f763c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f763c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f763c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f763c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f763c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f763c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f763c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f763c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f763c-114">Not supported.</span></span>|
|<span data-ttu-id="f763c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f763c-115">Application</span></span>|<span data-ttu-id="f763c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f763c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f763c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f763c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="f763c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f763c-118">Request headers</span></span>
|<span data-ttu-id="f763c-119">标头</span><span class="sxs-lookup"><span data-stu-id="f763c-119">Header</span></span>|<span data-ttu-id="f763c-120">值</span><span class="sxs-lookup"><span data-stu-id="f763c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f763c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f763c-121">Authorization</span></span>|<span data-ttu-id="f763c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f763c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f763c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f763c-123">Accept</span></span>|<span data-ttu-id="f763c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f763c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f763c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f763c-125">Request body</span></span>
<span data-ttu-id="f763c-126">在请求正文中，提供 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f763c-126">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="f763c-127">下表显示了创建 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f763c-127">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="f763c-128">属性</span><span class="sxs-lookup"><span data-stu-id="f763c-128">Property</span></span>|<span data-ttu-id="f763c-129">类型</span><span class="sxs-lookup"><span data-stu-id="f763c-129">Type</span></span>|<span data-ttu-id="f763c-130">说明</span><span class="sxs-lookup"><span data-stu-id="f763c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f763c-131">id</span><span class="sxs-lookup"><span data-stu-id="f763c-131">id</span></span>|<span data-ttu-id="f763c-132">String</span><span class="sxs-lookup"><span data-stu-id="f763c-132">String</span></span>|<span data-ttu-id="f763c-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f763c-133">Key of the entity.</span></span>|
|<span data-ttu-id="f763c-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f763c-134">pendingCount</span></span>|<span data-ttu-id="f763c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f763c-135">Int32</span></span>|<span data-ttu-id="f763c-136">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="f763c-136">Number of pending Users</span></span>|
|<span data-ttu-id="f763c-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f763c-137">notApplicableCount</span></span>|<span data-ttu-id="f763c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f763c-138">Int32</span></span>|<span data-ttu-id="f763c-139">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="f763c-139">Number of not applicable users</span></span>|
|<span data-ttu-id="f763c-140">successCount</span><span class="sxs-lookup"><span data-stu-id="f763c-140">successCount</span></span>|<span data-ttu-id="f763c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f763c-141">Int32</span></span>|<span data-ttu-id="f763c-142">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="f763c-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="f763c-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="f763c-143">errorCount</span></span>|<span data-ttu-id="f763c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f763c-144">Int32</span></span>|<span data-ttu-id="f763c-145">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="f763c-145">Number of error Users</span></span>|
|<span data-ttu-id="f763c-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="f763c-146">failedCount</span></span>|<span data-ttu-id="f763c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f763c-147">Int32</span></span>|<span data-ttu-id="f763c-148">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="f763c-148">Number of failed Users</span></span>|
|<span data-ttu-id="f763c-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f763c-149">lastUpdateDateTime</span></span>|<span data-ttu-id="f763c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f763c-150">DateTimeOffset</span></span>|<span data-ttu-id="f763c-151">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="f763c-151">Last update time</span></span>|
|<span data-ttu-id="f763c-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f763c-152">configurationVersion</span></span>|<span data-ttu-id="f763c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f763c-153">Int32</span></span>|<span data-ttu-id="f763c-154">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="f763c-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f763c-155">响应</span><span class="sxs-lookup"><span data-stu-id="f763c-155">Response</span></span>
<span data-ttu-id="f763c-156">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f763c-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f763c-157">示例</span><span class="sxs-lookup"><span data-stu-id="f763c-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="f763c-158">请求</span><span class="sxs-lookup"><span data-stu-id="f763c-158">Request</span></span>
<span data-ttu-id="f763c-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f763c-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f763c-160">响应</span><span class="sxs-lookup"><span data-stu-id="f763c-160">Response</span></span>
<span data-ttu-id="f763c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f763c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



