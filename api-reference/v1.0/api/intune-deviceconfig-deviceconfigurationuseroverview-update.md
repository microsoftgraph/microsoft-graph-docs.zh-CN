---
title: 更新 deviceConfigurationUserOverview
description: 更新 deviceConfigurationUserOverview 对象的属性。
author: tfitzmac
ms.openlocfilehash: 8b8feeec14bf8e9e3eafca8770461da611d05ae1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322755"
---
# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="4ea50-103">更新 deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="4ea50-103">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="4ea50-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4ea50-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ea50-105">更新 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4ea50-105">Update the properties of a [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4ea50-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ea50-106">Prerequisites</span></span>
<span data-ttu-id="4ea50-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="4ea50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea50-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ea50-109">Permission type</span></span>|<span data-ttu-id="4ea50-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ea50-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ea50-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ea50-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4ea50-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea50-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ea50-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ea50-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ea50-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ea50-114">Not supported.</span></span>|
|<span data-ttu-id="4ea50-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ea50-115">Application</span></span>|<span data-ttu-id="4ea50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ea50-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ea50-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ea50-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="4ea50-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ea50-118">Request headers</span></span>
|<span data-ttu-id="4ea50-119">标头</span><span class="sxs-lookup"><span data-stu-id="4ea50-119">Header</span></span>|<span data-ttu-id="4ea50-120">值</span><span class="sxs-lookup"><span data-stu-id="4ea50-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ea50-121">授权</span><span class="sxs-lookup"><span data-stu-id="4ea50-121">Authorization</span></span>|<span data-ttu-id="4ea50-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ea50-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ea50-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4ea50-123">Accept</span></span>|<span data-ttu-id="4ea50-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4ea50-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ea50-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ea50-125">Request body</span></span>
<span data-ttu-id="4ea50-126">在请求正文中，提供 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ea50-126">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="4ea50-127">下表显示创建 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ea50-127">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="4ea50-128">属性</span><span class="sxs-lookup"><span data-stu-id="4ea50-128">Property</span></span>|<span data-ttu-id="4ea50-129">类型</span><span class="sxs-lookup"><span data-stu-id="4ea50-129">Type</span></span>|<span data-ttu-id="4ea50-130">说明</span><span class="sxs-lookup"><span data-stu-id="4ea50-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ea50-131">id</span><span class="sxs-lookup"><span data-stu-id="4ea50-131">id</span></span>|<span data-ttu-id="4ea50-132">String</span><span class="sxs-lookup"><span data-stu-id="4ea50-132">String</span></span>|<span data-ttu-id="4ea50-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4ea50-133">Key of the entity.</span></span>|
|<span data-ttu-id="4ea50-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="4ea50-134">pendingCount</span></span>|<span data-ttu-id="4ea50-135">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea50-135">Int32</span></span>|<span data-ttu-id="4ea50-136">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="4ea50-136">Number of pending Users</span></span>|
|<span data-ttu-id="4ea50-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="4ea50-137">notApplicableCount</span></span>|<span data-ttu-id="4ea50-138">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea50-138">Int32</span></span>|<span data-ttu-id="4ea50-139">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="4ea50-139">Number of not applicable users</span></span>|
|<span data-ttu-id="4ea50-140">successCount</span><span class="sxs-lookup"><span data-stu-id="4ea50-140">successCount</span></span>|<span data-ttu-id="4ea50-141">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea50-141">Int32</span></span>|<span data-ttu-id="4ea50-142">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="4ea50-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="4ea50-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="4ea50-143">errorCount</span></span>|<span data-ttu-id="4ea50-144">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea50-144">Int32</span></span>|<span data-ttu-id="4ea50-145">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="4ea50-145">Number of error Users</span></span>|
|<span data-ttu-id="4ea50-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="4ea50-146">failedCount</span></span>|<span data-ttu-id="4ea50-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea50-147">Int32</span></span>|<span data-ttu-id="4ea50-148">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="4ea50-148">Number of failed Users</span></span>|
|<span data-ttu-id="4ea50-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4ea50-149">lastUpdateDateTime</span></span>|<span data-ttu-id="4ea50-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ea50-150">DateTimeOffset</span></span>|<span data-ttu-id="4ea50-151">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="4ea50-151">Last update time</span></span>|
|<span data-ttu-id="4ea50-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="4ea50-152">configurationVersion</span></span>|<span data-ttu-id="4ea50-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4ea50-153">Int32</span></span>|<span data-ttu-id="4ea50-154">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="4ea50-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="4ea50-155">响应</span><span class="sxs-lookup"><span data-stu-id="4ea50-155">Response</span></span>
<span data-ttu-id="4ea50-156">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ea50-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ea50-157">示例</span><span class="sxs-lookup"><span data-stu-id="4ea50-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ea50-158">请求</span><span class="sxs-lookup"><span data-stu-id="4ea50-158">Request</span></span>
<span data-ttu-id="4ea50-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ea50-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4ea50-160">响应</span><span class="sxs-lookup"><span data-stu-id="4ea50-160">Response</span></span>
<span data-ttu-id="4ea50-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ea50-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



