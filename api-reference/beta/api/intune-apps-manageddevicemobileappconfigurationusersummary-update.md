---
title: 更新 managedDeviceMobileAppConfigurationUserSummary
description: 更新 managedDeviceMobileAppConfigurationUserSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 484e6f2c2caa406ce95c4a3e4d9d78b9a879cd5f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983034"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="186fe-103">更新 managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="186fe-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="186fe-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="186fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="186fe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="186fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="186fe-106">更新 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="186fe-106">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="186fe-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="186fe-107">Prerequisites</span></span>
<span data-ttu-id="186fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="186fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="186fe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="186fe-110">Permission type</span></span>|<span data-ttu-id="186fe-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="186fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="186fe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="186fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="186fe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="186fe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="186fe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="186fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="186fe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="186fe-115">Not supported.</span></span>|
|<span data-ttu-id="186fe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="186fe-116">Application</span></span>|<span data-ttu-id="186fe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="186fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="186fe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="186fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="186fe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="186fe-119">Request headers</span></span>
|<span data-ttu-id="186fe-120">标头</span><span class="sxs-lookup"><span data-stu-id="186fe-120">Header</span></span>|<span data-ttu-id="186fe-121">值</span><span class="sxs-lookup"><span data-stu-id="186fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="186fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="186fe-122">Authorization</span></span>|<span data-ttu-id="186fe-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="186fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="186fe-124">接受</span><span class="sxs-lookup"><span data-stu-id="186fe-124">Accept</span></span>|<span data-ttu-id="186fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="186fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="186fe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="186fe-126">Request body</span></span>
<span data-ttu-id="186fe-127">在请求正文中，提供 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="186fe-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="186fe-128">下表显示创建 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="186fe-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="186fe-129">属性</span><span class="sxs-lookup"><span data-stu-id="186fe-129">Property</span></span>|<span data-ttu-id="186fe-130">类型</span><span class="sxs-lookup"><span data-stu-id="186fe-130">Type</span></span>|<span data-ttu-id="186fe-131">说明</span><span class="sxs-lookup"><span data-stu-id="186fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="186fe-132">id</span><span class="sxs-lookup"><span data-stu-id="186fe-132">id</span></span>|<span data-ttu-id="186fe-133">String</span><span class="sxs-lookup"><span data-stu-id="186fe-133">String</span></span>|<span data-ttu-id="186fe-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="186fe-134">Key of the entity.</span></span>|
|<span data-ttu-id="186fe-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="186fe-135">pendingCount</span></span>|<span data-ttu-id="186fe-136">Int32</span><span class="sxs-lookup"><span data-stu-id="186fe-136">Int32</span></span>|<span data-ttu-id="186fe-137">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="186fe-137">Number of pending Users</span></span>|
|<span data-ttu-id="186fe-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="186fe-138">notApplicableCount</span></span>|<span data-ttu-id="186fe-139">Int32</span><span class="sxs-lookup"><span data-stu-id="186fe-139">Int32</span></span>|<span data-ttu-id="186fe-140">不适用的用户数</span><span class="sxs-lookup"><span data-stu-id="186fe-140">Number of not applicable users</span></span>|
|<span data-ttu-id="186fe-141">successCount</span><span class="sxs-lookup"><span data-stu-id="186fe-141">successCount</span></span>|<span data-ttu-id="186fe-142">Int32</span><span class="sxs-lookup"><span data-stu-id="186fe-142">Int32</span></span>|<span data-ttu-id="186fe-143">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="186fe-143">Number of succeeded Users</span></span>|
|<span data-ttu-id="186fe-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="186fe-144">errorCount</span></span>|<span data-ttu-id="186fe-145">Int32</span><span class="sxs-lookup"><span data-stu-id="186fe-145">Int32</span></span>|<span data-ttu-id="186fe-146">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="186fe-146">Number of error Users</span></span>|
|<span data-ttu-id="186fe-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="186fe-147">failedCount</span></span>|<span data-ttu-id="186fe-148">Int32</span><span class="sxs-lookup"><span data-stu-id="186fe-148">Int32</span></span>|<span data-ttu-id="186fe-149">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="186fe-149">Number of failed Users</span></span>|
|<span data-ttu-id="186fe-150">conflictCount</span><span class="sxs-lookup"><span data-stu-id="186fe-150">conflictCount</span></span>|<span data-ttu-id="186fe-151">Int32</span><span class="sxs-lookup"><span data-stu-id="186fe-151">Int32</span></span>|<span data-ttu-id="186fe-152">发生冲突的用户数</span><span class="sxs-lookup"><span data-stu-id="186fe-152">Number of users in conflict</span></span>|
|<span data-ttu-id="186fe-153">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="186fe-153">lastUpdateDateTime</span></span>|<span data-ttu-id="186fe-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186fe-154">DateTimeOffset</span></span>|<span data-ttu-id="186fe-155">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="186fe-155">Last update time</span></span>|
|<span data-ttu-id="186fe-156">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="186fe-156">configurationVersion</span></span>|<span data-ttu-id="186fe-157">Int32</span><span class="sxs-lookup"><span data-stu-id="186fe-157">Int32</span></span>|<span data-ttu-id="186fe-158">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="186fe-158">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="186fe-159">响应</span><span class="sxs-lookup"><span data-stu-id="186fe-159">Response</span></span>
<span data-ttu-id="186fe-160">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="186fe-160">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="186fe-161">示例</span><span class="sxs-lookup"><span data-stu-id="186fe-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="186fe-162">请求</span><span class="sxs-lookup"><span data-stu-id="186fe-162">Request</span></span>
<span data-ttu-id="186fe-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="186fe-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 321

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
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

### <a name="response"></a><span data-ttu-id="186fe-164">响应</span><span class="sxs-lookup"><span data-stu-id="186fe-164">Response</span></span>
<span data-ttu-id="186fe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="186fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
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




