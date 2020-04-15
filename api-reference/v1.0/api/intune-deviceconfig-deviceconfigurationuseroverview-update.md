---
title: 更新 deviceConfigurationUserOverview
description: 更新 deviceConfigurationUserOverview 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b23fc487717af39bbcd84fb04ed290e7d98c3b55
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450638"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="4ab8c-103">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="4ab8c-103">Update deviceConfigurationUserOverview</span></span>

<span data-ttu-id="4ab8c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ab8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ab8c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ab8c-106">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-106">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ab8c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ab8c-107">Prerequisites</span></span>
<span data-ttu-id="4ab8c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ab8c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ab8c-110">Permission type</span></span>|<span data-ttu-id="4ab8c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ab8c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ab8c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ab8c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ab8c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ab8c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ab8c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ab8c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ab8c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-115">Not supported.</span></span>|
|<span data-ttu-id="4ab8c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ab8c-116">Application</span></span>|<span data-ttu-id="4ab8c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ab8c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ab8c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="4ab8c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ab8c-119">Request headers</span></span>
|<span data-ttu-id="4ab8c-120">标头</span><span class="sxs-lookup"><span data-stu-id="4ab8c-120">Header</span></span>|<span data-ttu-id="4ab8c-121">值</span><span class="sxs-lookup"><span data-stu-id="4ab8c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ab8c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ab8c-122">Authorization</span></span>|<span data-ttu-id="4ab8c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ab8c-124">接受</span><span class="sxs-lookup"><span data-stu-id="4ab8c-124">Accept</span></span>|<span data-ttu-id="4ab8c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ab8c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ab8c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ab8c-126">Request body</span></span>
<span data-ttu-id="4ab8c-127">在请求正文中，提供 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-127">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="4ab8c-128">下表显示创建 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-128">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="4ab8c-129">属性</span><span class="sxs-lookup"><span data-stu-id="4ab8c-129">Property</span></span>|<span data-ttu-id="4ab8c-130">类型</span><span class="sxs-lookup"><span data-stu-id="4ab8c-130">Type</span></span>|<span data-ttu-id="4ab8c-131">说明</span><span class="sxs-lookup"><span data-stu-id="4ab8c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ab8c-132">id</span><span class="sxs-lookup"><span data-stu-id="4ab8c-132">id</span></span>|<span data-ttu-id="4ab8c-133">String</span><span class="sxs-lookup"><span data-stu-id="4ab8c-133">String</span></span>|<span data-ttu-id="4ab8c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-134">Key of the entity.</span></span>|
|<span data-ttu-id="4ab8c-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4ab8c-135">pendingCount</span></span>|<span data-ttu-id="4ab8c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab8c-136">Int32</span></span>|<span data-ttu-id="4ab8c-137">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="4ab8c-137">Number of pending Users</span></span>|
|<span data-ttu-id="4ab8c-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4ab8c-138">notApplicableCount</span></span>|<span data-ttu-id="4ab8c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab8c-139">Int32</span></span>|<span data-ttu-id="4ab8c-140">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="4ab8c-140">Number of not applicable users</span></span>|
|<span data-ttu-id="4ab8c-141">successCount</span><span class="sxs-lookup"><span data-stu-id="4ab8c-141">successCount</span></span>|<span data-ttu-id="4ab8c-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab8c-142">Int32</span></span>|<span data-ttu-id="4ab8c-143">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="4ab8c-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="4ab8c-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="4ab8c-144">errorCount</span></span>|<span data-ttu-id="4ab8c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab8c-145">Int32</span></span>|<span data-ttu-id="4ab8c-146">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="4ab8c-146">Number of error Users</span></span>|
|<span data-ttu-id="4ab8c-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="4ab8c-147">failedCount</span></span>|<span data-ttu-id="4ab8c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab8c-148">Int32</span></span>|<span data-ttu-id="4ab8c-149">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="4ab8c-149">Number of failed Users</span></span>|
|<span data-ttu-id="4ab8c-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab8c-150">lastUpdateDateTime</span></span>|<span data-ttu-id="4ab8c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab8c-151">DateTimeOffset</span></span>|<span data-ttu-id="4ab8c-152">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="4ab8c-152">Last update time</span></span>|
|<span data-ttu-id="4ab8c-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4ab8c-153">configurationVersion</span></span>|<span data-ttu-id="4ab8c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="4ab8c-154">Int32</span></span>|<span data-ttu-id="4ab8c-155">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="4ab8c-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="4ab8c-156">响应</span><span class="sxs-lookup"><span data-stu-id="4ab8c-156">Response</span></span>
<span data-ttu-id="4ab8c-157">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ab8c-158">示例</span><span class="sxs-lookup"><span data-stu-id="4ab8c-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ab8c-159">请求</span><span class="sxs-lookup"><span data-stu-id="4ab8c-159">Request</span></span>
<span data-ttu-id="4ab8c-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 282

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="4ab8c-161">响应</span><span class="sxs-lookup"><span data-stu-id="4ab8c-161">Response</span></span>
<span data-ttu-id="4ab8c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ab8c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```






