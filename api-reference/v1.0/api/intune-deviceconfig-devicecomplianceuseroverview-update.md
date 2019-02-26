---
title: 更新 deviceComplianceUserOverview
description: 更新 deviceComplianceUserOverview 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c822ecc1c3fa61cb034a935d1a6ff363bba1520
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252768"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="d21db-103">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="d21db-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="d21db-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d21db-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d21db-105">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d21db-105">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d21db-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d21db-106">Prerequisites</span></span>
<span data-ttu-id="d21db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d21db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d21db-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d21db-109">Permission type</span></span>|<span data-ttu-id="d21db-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d21db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d21db-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d21db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d21db-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d21db-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d21db-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d21db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d21db-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d21db-114">Not supported.</span></span>|
|<span data-ttu-id="d21db-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d21db-115">Application</span></span>|<span data-ttu-id="d21db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d21db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d21db-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d21db-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="d21db-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d21db-118">Request headers</span></span>
|<span data-ttu-id="d21db-119">标头</span><span class="sxs-lookup"><span data-stu-id="d21db-119">Header</span></span>|<span data-ttu-id="d21db-120">值</span><span class="sxs-lookup"><span data-stu-id="d21db-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d21db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d21db-121">Authorization</span></span>|<span data-ttu-id="d21db-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d21db-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d21db-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d21db-123">Accept</span></span>|<span data-ttu-id="d21db-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d21db-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d21db-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d21db-125">Request body</span></span>
<span data-ttu-id="d21db-126">在请求正文中，提供 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d21db-126">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="d21db-127">下表显示了创建 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d21db-127">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="d21db-128">属性</span><span class="sxs-lookup"><span data-stu-id="d21db-128">Property</span></span>|<span data-ttu-id="d21db-129">类型</span><span class="sxs-lookup"><span data-stu-id="d21db-129">Type</span></span>|<span data-ttu-id="d21db-130">说明</span><span class="sxs-lookup"><span data-stu-id="d21db-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d21db-131">id</span><span class="sxs-lookup"><span data-stu-id="d21db-131">id</span></span>|<span data-ttu-id="d21db-132">String</span><span class="sxs-lookup"><span data-stu-id="d21db-132">String</span></span>|<span data-ttu-id="d21db-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d21db-133">Key of the entity.</span></span>|
|<span data-ttu-id="d21db-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d21db-134">pendingCount</span></span>|<span data-ttu-id="d21db-135">Int32</span><span class="sxs-lookup"><span data-stu-id="d21db-135">Int32</span></span>|<span data-ttu-id="d21db-136">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="d21db-136">Number of pending Users</span></span>|
|<span data-ttu-id="d21db-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d21db-137">notApplicableCount</span></span>|<span data-ttu-id="d21db-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d21db-138">Int32</span></span>|<span data-ttu-id="d21db-139">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="d21db-139">Number of not applicable users</span></span>|
|<span data-ttu-id="d21db-140">successCount</span><span class="sxs-lookup"><span data-stu-id="d21db-140">successCount</span></span>|<span data-ttu-id="d21db-141">Int32</span><span class="sxs-lookup"><span data-stu-id="d21db-141">Int32</span></span>|<span data-ttu-id="d21db-142">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="d21db-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="d21db-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="d21db-143">errorCount</span></span>|<span data-ttu-id="d21db-144">Int32</span><span class="sxs-lookup"><span data-stu-id="d21db-144">Int32</span></span>|<span data-ttu-id="d21db-145">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="d21db-145">Number of error Users</span></span>|
|<span data-ttu-id="d21db-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="d21db-146">failedCount</span></span>|<span data-ttu-id="d21db-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d21db-147">Int32</span></span>|<span data-ttu-id="d21db-148">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="d21db-148">Number of failed Users</span></span>|
|<span data-ttu-id="d21db-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d21db-149">lastUpdateDateTime</span></span>|<span data-ttu-id="d21db-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d21db-150">DateTimeOffset</span></span>|<span data-ttu-id="d21db-151">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="d21db-151">Last update time</span></span>|
|<span data-ttu-id="d21db-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d21db-152">configurationVersion</span></span>|<span data-ttu-id="d21db-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d21db-153">Int32</span></span>|<span data-ttu-id="d21db-154">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="d21db-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="d21db-155">响应</span><span class="sxs-lookup"><span data-stu-id="d21db-155">Response</span></span>
<span data-ttu-id="d21db-156">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d21db-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d21db-157">示例</span><span class="sxs-lookup"><span data-stu-id="d21db-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="d21db-158">请求</span><span class="sxs-lookup"><span data-stu-id="d21db-158">Request</span></span>
<span data-ttu-id="d21db-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d21db-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d21db-160">响应</span><span class="sxs-lookup"><span data-stu-id="d21db-160">Response</span></span>
<span data-ttu-id="d21db-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d21db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



