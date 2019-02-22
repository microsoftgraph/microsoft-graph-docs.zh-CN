---
title: 更新 managedDeviceMobileAppConfigurationDeviceSummary
description: 更新 managedDeviceMobileAppConfigurationDeviceSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b5093a64185a05aafb9aa378f9f84b3490894a0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174317"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="68d15-103">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="68d15-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="68d15-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68d15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68d15-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68d15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68d15-106">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="68d15-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68d15-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="68d15-107">Prerequisites</span></span>
<span data-ttu-id="68d15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="68d15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="68d15-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="68d15-110">Permission type</span></span>|<span data-ttu-id="68d15-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="68d15-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68d15-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68d15-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68d15-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68d15-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="68d15-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68d15-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68d15-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="68d15-115">Not supported.</span></span>|
|<span data-ttu-id="68d15-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="68d15-116">Application</span></span>|<span data-ttu-id="68d15-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="68d15-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68d15-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68d15-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="68d15-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="68d15-119">Request headers</span></span>
|<span data-ttu-id="68d15-120">标头</span><span class="sxs-lookup"><span data-stu-id="68d15-120">Header</span></span>|<span data-ttu-id="68d15-121">值</span><span class="sxs-lookup"><span data-stu-id="68d15-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68d15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="68d15-122">Authorization</span></span>|<span data-ttu-id="68d15-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="68d15-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68d15-124">Accept</span><span class="sxs-lookup"><span data-stu-id="68d15-124">Accept</span></span>|<span data-ttu-id="68d15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="68d15-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68d15-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="68d15-126">Request body</span></span>
<span data-ttu-id="68d15-127">在请求正文中，提供 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68d15-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="68d15-128">下表显示创建 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="68d15-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="68d15-129">属性</span><span class="sxs-lookup"><span data-stu-id="68d15-129">Property</span></span>|<span data-ttu-id="68d15-130">类型</span><span class="sxs-lookup"><span data-stu-id="68d15-130">Type</span></span>|<span data-ttu-id="68d15-131">说明</span><span class="sxs-lookup"><span data-stu-id="68d15-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68d15-132">id</span><span class="sxs-lookup"><span data-stu-id="68d15-132">id</span></span>|<span data-ttu-id="68d15-133">String</span><span class="sxs-lookup"><span data-stu-id="68d15-133">String</span></span>|<span data-ttu-id="68d15-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="68d15-134">Key of the entity.</span></span>|
|<span data-ttu-id="68d15-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="68d15-135">pendingCount</span></span>|<span data-ttu-id="68d15-136">Int32</span><span class="sxs-lookup"><span data-stu-id="68d15-136">Int32</span></span>|<span data-ttu-id="68d15-137">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="68d15-137">Number of pending devices</span></span>|
|<span data-ttu-id="68d15-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="68d15-138">notApplicableCount</span></span>|<span data-ttu-id="68d15-139">Int32</span><span class="sxs-lookup"><span data-stu-id="68d15-139">Int32</span></span>|<span data-ttu-id="68d15-140">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="68d15-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="68d15-141">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="68d15-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="68d15-142">Int32</span><span class="sxs-lookup"><span data-stu-id="68d15-142">Int32</span></span>|<span data-ttu-id="68d15-143">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="68d15-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="68d15-144">successCount</span><span class="sxs-lookup"><span data-stu-id="68d15-144">successCount</span></span>|<span data-ttu-id="68d15-145">Int32</span><span class="sxs-lookup"><span data-stu-id="68d15-145">Int32</span></span>|<span data-ttu-id="68d15-146">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="68d15-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="68d15-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="68d15-147">errorCount</span></span>|<span data-ttu-id="68d15-148">Int32</span><span class="sxs-lookup"><span data-stu-id="68d15-148">Int32</span></span>|<span data-ttu-id="68d15-149">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="68d15-149">Number of error devices</span></span>|
|<span data-ttu-id="68d15-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="68d15-150">failedCount</span></span>|<span data-ttu-id="68d15-151">Int32</span><span class="sxs-lookup"><span data-stu-id="68d15-151">Int32</span></span>|<span data-ttu-id="68d15-152">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="68d15-152">Number of failed devices</span></span>|
|<span data-ttu-id="68d15-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="68d15-153">conflictCount</span></span>|<span data-ttu-id="68d15-154">Int32</span><span class="sxs-lookup"><span data-stu-id="68d15-154">Int32</span></span>|<span data-ttu-id="68d15-155">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="68d15-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="68d15-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="68d15-156">lastUpdateDateTime</span></span>|<span data-ttu-id="68d15-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68d15-157">DateTimeOffset</span></span>|<span data-ttu-id="68d15-158">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="68d15-158">Last update time</span></span>|
|<span data-ttu-id="68d15-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="68d15-159">configurationVersion</span></span>|<span data-ttu-id="68d15-160">Int32</span><span class="sxs-lookup"><span data-stu-id="68d15-160">Int32</span></span>|<span data-ttu-id="68d15-161">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="68d15-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="68d15-162">响应</span><span class="sxs-lookup"><span data-stu-id="68d15-162">Response</span></span>
<span data-ttu-id="68d15-163">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68d15-163">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68d15-164">示例</span><span class="sxs-lookup"><span data-stu-id="68d15-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="68d15-165">请求</span><span class="sxs-lookup"><span data-stu-id="68d15-165">Request</span></span>
<span data-ttu-id="68d15-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="68d15-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="68d15-167">响应</span><span class="sxs-lookup"><span data-stu-id="68d15-167">Response</span></span>
<span data-ttu-id="68d15-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="68d15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




