---
title: 更新 deviceConfigurationUserOverview
description: 更新 deviceConfigurationUserOverview 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5badee7a5a5257b06e30e9a943bd37eb7d9db107
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568164"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="f8f12-103">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="f8f12-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="f8f12-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8f12-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8f12-105">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f8f12-105">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8f12-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8f12-106">Prerequisites</span></span>
<span data-ttu-id="f8f12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8f12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8f12-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8f12-109">Permission type</span></span>|<span data-ttu-id="f8f12-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8f12-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8f12-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8f12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f8f12-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8f12-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8f12-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8f12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8f12-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8f12-114">Not supported.</span></span>|
|<span data-ttu-id="f8f12-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8f12-115">Application</span></span>|<span data-ttu-id="f8f12-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8f12-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8f12-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8f12-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="f8f12-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8f12-118">Request headers</span></span>
|<span data-ttu-id="f8f12-119">标头</span><span class="sxs-lookup"><span data-stu-id="f8f12-119">Header</span></span>|<span data-ttu-id="f8f12-120">值</span><span class="sxs-lookup"><span data-stu-id="f8f12-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8f12-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8f12-121">Authorization</span></span>|<span data-ttu-id="f8f12-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f8f12-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8f12-123">接受</span><span class="sxs-lookup"><span data-stu-id="f8f12-123">Accept</span></span>|<span data-ttu-id="f8f12-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f8f12-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8f12-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8f12-125">Request body</span></span>
<span data-ttu-id="f8f12-126">在请求正文中，提供 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8f12-126">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="f8f12-127">下表显示创建 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f8f12-127">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="f8f12-128">属性</span><span class="sxs-lookup"><span data-stu-id="f8f12-128">Property</span></span>|<span data-ttu-id="f8f12-129">类型</span><span class="sxs-lookup"><span data-stu-id="f8f12-129">Type</span></span>|<span data-ttu-id="f8f12-130">说明</span><span class="sxs-lookup"><span data-stu-id="f8f12-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8f12-131">id</span><span class="sxs-lookup"><span data-stu-id="f8f12-131">id</span></span>|<span data-ttu-id="f8f12-132">String</span><span class="sxs-lookup"><span data-stu-id="f8f12-132">String</span></span>|<span data-ttu-id="f8f12-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f8f12-133">Key of the entity.</span></span>|
|<span data-ttu-id="f8f12-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="f8f12-134">pendingCount</span></span>|<span data-ttu-id="f8f12-135">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f12-135">Int32</span></span>|<span data-ttu-id="f8f12-136">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="f8f12-136">Number of pending Users</span></span>|
|<span data-ttu-id="f8f12-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="f8f12-137">notApplicableCount</span></span>|<span data-ttu-id="f8f12-138">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f12-138">Int32</span></span>|<span data-ttu-id="f8f12-139">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="f8f12-139">Number of not applicable users</span></span>|
|<span data-ttu-id="f8f12-140">successCount</span><span class="sxs-lookup"><span data-stu-id="f8f12-140">successCount</span></span>|<span data-ttu-id="f8f12-141">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f12-141">Int32</span></span>|<span data-ttu-id="f8f12-142">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="f8f12-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="f8f12-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="f8f12-143">errorCount</span></span>|<span data-ttu-id="f8f12-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f12-144">Int32</span></span>|<span data-ttu-id="f8f12-145">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="f8f12-145">Number of error Users</span></span>|
|<span data-ttu-id="f8f12-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="f8f12-146">failedCount</span></span>|<span data-ttu-id="f8f12-147">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f12-147">Int32</span></span>|<span data-ttu-id="f8f12-148">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="f8f12-148">Number of failed Users</span></span>|
|<span data-ttu-id="f8f12-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f8f12-149">lastUpdateDateTime</span></span>|<span data-ttu-id="f8f12-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8f12-150">DateTimeOffset</span></span>|<span data-ttu-id="f8f12-151">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="f8f12-151">Last update time</span></span>|
|<span data-ttu-id="f8f12-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="f8f12-152">configurationVersion</span></span>|<span data-ttu-id="f8f12-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f8f12-153">Int32</span></span>|<span data-ttu-id="f8f12-154">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="f8f12-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="f8f12-155">响应</span><span class="sxs-lookup"><span data-stu-id="f8f12-155">Response</span></span>
<span data-ttu-id="f8f12-156">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8f12-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8f12-157">示例</span><span class="sxs-lookup"><span data-stu-id="f8f12-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8f12-158">请求</span><span class="sxs-lookup"><span data-stu-id="f8f12-158">Request</span></span>
<span data-ttu-id="f8f12-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8f12-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8f12-160">响应</span><span class="sxs-lookup"><span data-stu-id="f8f12-160">Response</span></span>
<span data-ttu-id="f8f12-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8f12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



