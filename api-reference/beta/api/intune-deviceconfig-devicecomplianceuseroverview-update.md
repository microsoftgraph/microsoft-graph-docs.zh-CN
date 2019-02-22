---
title: 更新 deviceComplianceUserOverview
description: 更新 deviceComplianceUserOverview 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c82332f83e79ca9d5ccfceb1967b4d8df76bd7fd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146275"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="4d25e-103">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="4d25e-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="4d25e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d25e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d25e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d25e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d25e-106">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4d25e-106">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d25e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4d25e-107">Prerequisites</span></span>
<span data-ttu-id="4d25e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4d25e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4d25e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d25e-110">Permission type</span></span>|<span data-ttu-id="4d25e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4d25e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d25e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d25e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4d25e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d25e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d25e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d25e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d25e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d25e-115">Not supported.</span></span>|
|<span data-ttu-id="4d25e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d25e-116">Application</span></span>|<span data-ttu-id="4d25e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d25e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d25e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d25e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="4d25e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d25e-119">Request headers</span></span>
|<span data-ttu-id="4d25e-120">标头</span><span class="sxs-lookup"><span data-stu-id="4d25e-120">Header</span></span>|<span data-ttu-id="4d25e-121">值</span><span class="sxs-lookup"><span data-stu-id="4d25e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d25e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d25e-122">Authorization</span></span>|<span data-ttu-id="4d25e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4d25e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d25e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4d25e-124">Accept</span></span>|<span data-ttu-id="4d25e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d25e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d25e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d25e-126">Request body</span></span>
<span data-ttu-id="4d25e-127">在请求正文中，提供 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d25e-127">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="4d25e-128">下表显示了创建 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4d25e-128">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="4d25e-129">属性</span><span class="sxs-lookup"><span data-stu-id="4d25e-129">Property</span></span>|<span data-ttu-id="4d25e-130">类型</span><span class="sxs-lookup"><span data-stu-id="4d25e-130">Type</span></span>|<span data-ttu-id="4d25e-131">说明</span><span class="sxs-lookup"><span data-stu-id="4d25e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d25e-132">id</span><span class="sxs-lookup"><span data-stu-id="4d25e-132">id</span></span>|<span data-ttu-id="4d25e-133">String</span><span class="sxs-lookup"><span data-stu-id="4d25e-133">String</span></span>|<span data-ttu-id="4d25e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4d25e-134">Key of the entity.</span></span>|
|<span data-ttu-id="4d25e-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4d25e-135">pendingCount</span></span>|<span data-ttu-id="4d25e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4d25e-136">Int32</span></span>|<span data-ttu-id="4d25e-137">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="4d25e-137">Number of pending Users</span></span>|
|<span data-ttu-id="4d25e-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4d25e-138">notApplicableCount</span></span>|<span data-ttu-id="4d25e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4d25e-139">Int32</span></span>|<span data-ttu-id="4d25e-140">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="4d25e-140">Number of not applicable users</span></span>|
|<span data-ttu-id="4d25e-141">successCount</span><span class="sxs-lookup"><span data-stu-id="4d25e-141">successCount</span></span>|<span data-ttu-id="4d25e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4d25e-142">Int32</span></span>|<span data-ttu-id="4d25e-143">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="4d25e-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="4d25e-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="4d25e-144">errorCount</span></span>|<span data-ttu-id="4d25e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4d25e-145">Int32</span></span>|<span data-ttu-id="4d25e-146">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="4d25e-146">Number of error Users</span></span>|
|<span data-ttu-id="4d25e-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="4d25e-147">failedCount</span></span>|<span data-ttu-id="4d25e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4d25e-148">Int32</span></span>|<span data-ttu-id="4d25e-149">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="4d25e-149">Number of failed Users</span></span>|
|<span data-ttu-id="4d25e-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="4d25e-150">conflictCount</span></span>|<span data-ttu-id="4d25e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="4d25e-151">Int32</span></span>|<span data-ttu-id="4d25e-152">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="4d25e-152">Number of users in conflict</span></span>|
|<span data-ttu-id="4d25e-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4d25e-153">lastUpdateDateTime</span></span>|<span data-ttu-id="4d25e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d25e-154">DateTimeOffset</span></span>|<span data-ttu-id="4d25e-155">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="4d25e-155">Last update time</span></span>|
|<span data-ttu-id="4d25e-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4d25e-156">configurationVersion</span></span>|<span data-ttu-id="4d25e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="4d25e-157">Int32</span></span>|<span data-ttu-id="4d25e-158">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="4d25e-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="4d25e-159">响应</span><span class="sxs-lookup"><span data-stu-id="4d25e-159">Response</span></span>
<span data-ttu-id="4d25e-160">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d25e-160">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d25e-161">示例</span><span class="sxs-lookup"><span data-stu-id="4d25e-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d25e-162">请求</span><span class="sxs-lookup"><span data-stu-id="4d25e-162">Request</span></span>
<span data-ttu-id="4d25e-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4d25e-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="4d25e-164">响应</span><span class="sxs-lookup"><span data-stu-id="4d25e-164">Response</span></span>
<span data-ttu-id="4d25e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d25e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 352

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




