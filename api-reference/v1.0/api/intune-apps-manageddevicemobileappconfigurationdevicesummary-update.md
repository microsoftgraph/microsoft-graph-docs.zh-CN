---
title: 更新 managedDeviceMobileAppConfigurationDeviceSummary
description: 更新 managedDeviceMobileAppConfigurationDeviceSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 595a1b0352421b4470324011cafb7e594dad60ce
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759838"
---
# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="d10bb-103">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="d10bb-103">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

<span data-ttu-id="d10bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d10bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d10bb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d10bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d10bb-106">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d10bb-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d10bb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d10bb-107">Prerequisites</span></span>
<span data-ttu-id="d10bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d10bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d10bb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d10bb-110">Permission type</span></span>|<span data-ttu-id="d10bb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d10bb-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d10bb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d10bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d10bb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d10bb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d10bb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d10bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d10bb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d10bb-115">Not supported.</span></span>|
|<span data-ttu-id="d10bb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d10bb-116">Application</span></span>|<span data-ttu-id="d10bb-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d10bb-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d10bb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d10bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="d10bb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d10bb-119">Request headers</span></span>
|<span data-ttu-id="d10bb-120">标头</span><span class="sxs-lookup"><span data-stu-id="d10bb-120">Header</span></span>|<span data-ttu-id="d10bb-121">值</span><span class="sxs-lookup"><span data-stu-id="d10bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d10bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d10bb-122">Authorization</span></span>|<span data-ttu-id="d10bb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d10bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d10bb-124">接受</span><span class="sxs-lookup"><span data-stu-id="d10bb-124">Accept</span></span>|<span data-ttu-id="d10bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d10bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d10bb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d10bb-126">Request body</span></span>
<span data-ttu-id="d10bb-127">在请求正文中，提供 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d10bb-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="d10bb-128">下表显示创建 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d10bb-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="d10bb-129">属性</span><span class="sxs-lookup"><span data-stu-id="d10bb-129">Property</span></span>|<span data-ttu-id="d10bb-130">类型</span><span class="sxs-lookup"><span data-stu-id="d10bb-130">Type</span></span>|<span data-ttu-id="d10bb-131">说明</span><span class="sxs-lookup"><span data-stu-id="d10bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d10bb-132">id</span><span class="sxs-lookup"><span data-stu-id="d10bb-132">id</span></span>|<span data-ttu-id="d10bb-133">String</span><span class="sxs-lookup"><span data-stu-id="d10bb-133">String</span></span>|<span data-ttu-id="d10bb-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d10bb-134">Key of the entity.</span></span>|
|<span data-ttu-id="d10bb-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="d10bb-135">pendingCount</span></span>|<span data-ttu-id="d10bb-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d10bb-136">Int32</span></span>|<span data-ttu-id="d10bb-137">挂起设备的数量</span><span class="sxs-lookup"><span data-stu-id="d10bb-137">Number of pending devices</span></span>|
|<span data-ttu-id="d10bb-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d10bb-138">notApplicableCount</span></span>|<span data-ttu-id="d10bb-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d10bb-139">Int32</span></span>|<span data-ttu-id="d10bb-140">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="d10bb-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="d10bb-141">successCount</span><span class="sxs-lookup"><span data-stu-id="d10bb-141">successCount</span></span>|<span data-ttu-id="d10bb-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d10bb-142">Int32</span></span>|<span data-ttu-id="d10bb-143">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="d10bb-143">Number of succeeded devices</span></span>|
|<span data-ttu-id="d10bb-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="d10bb-144">errorCount</span></span>|<span data-ttu-id="d10bb-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d10bb-145">Int32</span></span>|<span data-ttu-id="d10bb-146">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="d10bb-146">Number of error devices</span></span>|
|<span data-ttu-id="d10bb-147">failedCount</span><span class="sxs-lookup"><span data-stu-id="d10bb-147">failedCount</span></span>|<span data-ttu-id="d10bb-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d10bb-148">Int32</span></span>|<span data-ttu-id="d10bb-149">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="d10bb-149">Number of failed devices</span></span>|
|<span data-ttu-id="d10bb-150">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="d10bb-150">lastUpdateDateTime</span></span>|<span data-ttu-id="d10bb-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d10bb-151">DateTimeOffset</span></span>|<span data-ttu-id="d10bb-152">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="d10bb-152">Last update time</span></span>|
|<span data-ttu-id="d10bb-153">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="d10bb-153">configurationVersion</span></span>|<span data-ttu-id="d10bb-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d10bb-154">Int32</span></span>|<span data-ttu-id="d10bb-155">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="d10bb-155">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="d10bb-156">响应</span><span class="sxs-lookup"><span data-stu-id="d10bb-156">Response</span></span>
<span data-ttu-id="d10bb-157">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d10bb-157">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d10bb-158">示例</span><span class="sxs-lookup"><span data-stu-id="d10bb-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="d10bb-159">请求</span><span class="sxs-lookup"><span data-stu-id="d10bb-159">Request</span></span>
<span data-ttu-id="d10bb-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d10bb-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 299

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="d10bb-161">响应</span><span class="sxs-lookup"><span data-stu-id="d10bb-161">Response</span></span>
<span data-ttu-id="d10bb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d10bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




