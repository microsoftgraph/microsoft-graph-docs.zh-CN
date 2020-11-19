---
title: 更新 deviceComplianceUserOverview
description: 更新 deviceComplianceUserOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26ef3709d37cf6c83b065ad572aa3db383df791f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213810"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="d945c-103">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="d945c-103">Update deviceComplianceUserOverview</span></span>

<span data-ttu-id="d945c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d945c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d945c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d945c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d945c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d945c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d945c-107">更新 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d945c-107">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d945c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d945c-108">Prerequisites</span></span>
<span data-ttu-id="d945c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d945c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d945c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d945c-111">Permission type</span></span>|<span data-ttu-id="d945c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d945c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d945c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d945c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d945c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d945c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d945c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d945c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d945c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d945c-116">Not supported.</span></span>|
|<span data-ttu-id="d945c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d945c-117">Application</span></span>|<span data-ttu-id="d945c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d945c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d945c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d945c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="d945c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d945c-120">Request headers</span></span>
|<span data-ttu-id="d945c-121">标头</span><span class="sxs-lookup"><span data-stu-id="d945c-121">Header</span></span>|<span data-ttu-id="d945c-122">值</span><span class="sxs-lookup"><span data-stu-id="d945c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d945c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d945c-123">Authorization</span></span>|<span data-ttu-id="d945c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d945c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d945c-125">接受</span><span class="sxs-lookup"><span data-stu-id="d945c-125">Accept</span></span>|<span data-ttu-id="d945c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d945c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d945c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d945c-127">Request body</span></span>
<span data-ttu-id="d945c-128">在请求正文中，提供 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d945c-128">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="d945c-129">下表显示了创建 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d945c-129">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="d945c-130">属性</span><span class="sxs-lookup"><span data-stu-id="d945c-130">Property</span></span>|<span data-ttu-id="d945c-131">类型</span><span class="sxs-lookup"><span data-stu-id="d945c-131">Type</span></span>|<span data-ttu-id="d945c-132">说明</span><span class="sxs-lookup"><span data-stu-id="d945c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d945c-133">id</span><span class="sxs-lookup"><span data-stu-id="d945c-133">id</span></span>|<span data-ttu-id="d945c-134">String</span><span class="sxs-lookup"><span data-stu-id="d945c-134">String</span></span>|<span data-ttu-id="d945c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d945c-135">Key of the entity.</span></span>|
|<span data-ttu-id="d945c-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d945c-136">pendingCount</span></span>|<span data-ttu-id="d945c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d945c-137">Int32</span></span>|<span data-ttu-id="d945c-138">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="d945c-138">Number of pending Users</span></span>|
|<span data-ttu-id="d945c-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d945c-139">notApplicableCount</span></span>|<span data-ttu-id="d945c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d945c-140">Int32</span></span>|<span data-ttu-id="d945c-141">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="d945c-141">Number of not applicable users</span></span>|
|<span data-ttu-id="d945c-142">successCount</span><span class="sxs-lookup"><span data-stu-id="d945c-142">successCount</span></span>|<span data-ttu-id="d945c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d945c-143">Int32</span></span>|<span data-ttu-id="d945c-144">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="d945c-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="d945c-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="d945c-145">errorCount</span></span>|<span data-ttu-id="d945c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d945c-146">Int32</span></span>|<span data-ttu-id="d945c-147">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="d945c-147">Number of error Users</span></span>|
|<span data-ttu-id="d945c-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="d945c-148">failedCount</span></span>|<span data-ttu-id="d945c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d945c-149">Int32</span></span>|<span data-ttu-id="d945c-150">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="d945c-150">Number of failed Users</span></span>|
|<span data-ttu-id="d945c-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d945c-151">conflictCount</span></span>|<span data-ttu-id="d945c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d945c-152">Int32</span></span>|<span data-ttu-id="d945c-153">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="d945c-153">Number of users in conflict</span></span>|
|<span data-ttu-id="d945c-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d945c-154">lastUpdateDateTime</span></span>|<span data-ttu-id="d945c-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d945c-155">DateTimeOffset</span></span>|<span data-ttu-id="d945c-156">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="d945c-156">Last update time</span></span>|
|<span data-ttu-id="d945c-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d945c-157">configurationVersion</span></span>|<span data-ttu-id="d945c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d945c-158">Int32</span></span>|<span data-ttu-id="d945c-159">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="d945c-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="d945c-160">响应</span><span class="sxs-lookup"><span data-stu-id="d945c-160">Response</span></span>
<span data-ttu-id="d945c-161">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d945c-161">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d945c-162">示例</span><span class="sxs-lookup"><span data-stu-id="d945c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="d945c-163">请求</span><span class="sxs-lookup"><span data-stu-id="d945c-163">Request</span></span>
<span data-ttu-id="d945c-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d945c-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d945c-165">响应</span><span class="sxs-lookup"><span data-stu-id="d945c-165">Response</span></span>
<span data-ttu-id="d945c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d945c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




