---
title: 更新 managedDeviceMobileAppConfigurationDeviceSummary
description: 更新 managedDeviceMobileAppConfigurationDeviceSummary 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5672fa78f041967064425520a1df5cb52c6ff15c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412665"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="e503a-103">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="e503a-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="e503a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e503a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e503a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e503a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e503a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e503a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e503a-107">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e503a-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e503a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e503a-108">Prerequisites</span></span>
<span data-ttu-id="e503a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e503a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e503a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e503a-111">Permission type</span></span>|<span data-ttu-id="e503a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e503a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e503a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e503a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e503a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e503a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e503a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e503a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e503a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e503a-116">Not supported.</span></span>|
|<span data-ttu-id="e503a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e503a-117">Application</span></span>|<span data-ttu-id="e503a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e503a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e503a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e503a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="e503a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e503a-120">Request headers</span></span>
|<span data-ttu-id="e503a-121">标头</span><span class="sxs-lookup"><span data-stu-id="e503a-121">Header</span></span>|<span data-ttu-id="e503a-122">值</span><span class="sxs-lookup"><span data-stu-id="e503a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e503a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e503a-123">Authorization</span></span>|<span data-ttu-id="e503a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e503a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e503a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e503a-125">Accept</span></span>|<span data-ttu-id="e503a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e503a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e503a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e503a-127">Request body</span></span>
<span data-ttu-id="e503a-128">在请求正文中，提供 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e503a-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="e503a-129">下表显示创建 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e503a-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="e503a-130">属性</span><span class="sxs-lookup"><span data-stu-id="e503a-130">Property</span></span>|<span data-ttu-id="e503a-131">类型</span><span class="sxs-lookup"><span data-stu-id="e503a-131">Type</span></span>|<span data-ttu-id="e503a-132">说明</span><span class="sxs-lookup"><span data-stu-id="e503a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e503a-133">id</span><span class="sxs-lookup"><span data-stu-id="e503a-133">id</span></span>|<span data-ttu-id="e503a-134">String</span><span class="sxs-lookup"><span data-stu-id="e503a-134">String</span></span>|<span data-ttu-id="e503a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e503a-135">Key of the entity.</span></span>|
|<span data-ttu-id="e503a-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="e503a-136">pendingCount</span></span>|<span data-ttu-id="e503a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e503a-137">Int32</span></span>|<span data-ttu-id="e503a-138">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="e503a-138">Number of pending devices</span></span>|
|<span data-ttu-id="e503a-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="e503a-139">notApplicableCount</span></span>|<span data-ttu-id="e503a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e503a-140">Int32</span></span>|<span data-ttu-id="e503a-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="e503a-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="e503a-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="e503a-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="e503a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e503a-143">Int32</span></span>|<span data-ttu-id="e503a-144">由于不匹配平台和策略不适用设备数</span><span class="sxs-lookup"><span data-stu-id="e503a-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="e503a-145">successCount</span><span class="sxs-lookup"><span data-stu-id="e503a-145">successCount</span></span>|<span data-ttu-id="e503a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e503a-146">Int32</span></span>|<span data-ttu-id="e503a-147">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="e503a-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="e503a-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="e503a-148">errorCount</span></span>|<span data-ttu-id="e503a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e503a-149">Int32</span></span>|<span data-ttu-id="e503a-150">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="e503a-150">Number of error devices</span></span>|
|<span data-ttu-id="e503a-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="e503a-151">failedCount</span></span>|<span data-ttu-id="e503a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e503a-152">Int32</span></span>|<span data-ttu-id="e503a-153">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="e503a-153">Number of failed devices</span></span>|
|<span data-ttu-id="e503a-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="e503a-154">conflictCount</span></span>|<span data-ttu-id="e503a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="e503a-155">Int32</span></span>|<span data-ttu-id="e503a-156">存在冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="e503a-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="e503a-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e503a-157">lastUpdateDateTime</span></span>|<span data-ttu-id="e503a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e503a-158">DateTimeOffset</span></span>|<span data-ttu-id="e503a-159">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="e503a-159">Last update time</span></span>|
|<span data-ttu-id="e503a-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="e503a-160">configurationVersion</span></span>|<span data-ttu-id="e503a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="e503a-161">Int32</span></span>|<span data-ttu-id="e503a-162">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="e503a-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="e503a-163">响应</span><span class="sxs-lookup"><span data-stu-id="e503a-163">Response</span></span>
<span data-ttu-id="e503a-164">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e503a-164">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e503a-165">示例</span><span class="sxs-lookup"><span data-stu-id="e503a-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="e503a-166">请求</span><span class="sxs-lookup"><span data-stu-id="e503a-166">Request</span></span>
<span data-ttu-id="e503a-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e503a-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="e503a-168">响应</span><span class="sxs-lookup"><span data-stu-id="e503a-168">Response</span></span>
<span data-ttu-id="e503a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e503a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




