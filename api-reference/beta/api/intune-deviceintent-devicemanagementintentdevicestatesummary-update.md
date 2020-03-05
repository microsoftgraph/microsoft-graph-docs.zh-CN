---
title: 更新 deviceManagementIntentDeviceStateSummary
description: 更新 deviceManagementIntentDeviceStateSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f52742c990d86cde024bdc115670cf0e5c2c3bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470866"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="2f9b4-103">更新 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="2f9b4-103">Update deviceManagementIntentDeviceStateSummary</span></span>

<span data-ttu-id="2f9b4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2f9b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f9b4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f9b4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f9b4-107">更新[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-107">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f9b4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2f9b4-108">Prerequisites</span></span>
<span data-ttu-id="2f9b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f9b4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f9b4-111">Permission type</span></span>|<span data-ttu-id="2f9b4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2f9b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f9b4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f9b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f9b4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f9b4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f9b4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f9b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f9b4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-116">Not supported.</span></span>|
|<span data-ttu-id="2f9b4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f9b4-117">Application</span></span>|<span data-ttu-id="2f9b4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f9b4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f9b4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f9b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="2f9b4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f9b4-120">Request headers</span></span>
|<span data-ttu-id="2f9b4-121">标头</span><span class="sxs-lookup"><span data-stu-id="2f9b4-121">Header</span></span>|<span data-ttu-id="2f9b4-122">值</span><span class="sxs-lookup"><span data-stu-id="2f9b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f9b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f9b4-123">Authorization</span></span>|<span data-ttu-id="2f9b4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f9b4-125">接受</span><span class="sxs-lookup"><span data-stu-id="2f9b4-125">Accept</span></span>|<span data-ttu-id="2f9b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f9b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f9b4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f9b4-127">Request body</span></span>
<span data-ttu-id="2f9b4-128">在请求正文中，提供[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="2f9b4-129">下表显示创建[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="2f9b4-130">属性</span><span class="sxs-lookup"><span data-stu-id="2f9b4-130">Property</span></span>|<span data-ttu-id="2f9b4-131">类型</span><span class="sxs-lookup"><span data-stu-id="2f9b4-131">Type</span></span>|<span data-ttu-id="2f9b4-132">说明</span><span class="sxs-lookup"><span data-stu-id="2f9b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f9b4-133">id</span><span class="sxs-lookup"><span data-stu-id="2f9b4-133">id</span></span>|<span data-ttu-id="2f9b4-134">String</span><span class="sxs-lookup"><span data-stu-id="2f9b4-134">String</span></span>|<span data-ttu-id="2f9b4-135">ID</span><span class="sxs-lookup"><span data-stu-id="2f9b4-135">The ID</span></span>|
|<span data-ttu-id="2f9b4-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="2f9b4-136">conflictCount</span></span>|<span data-ttu-id="2f9b4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2f9b4-137">Int32</span></span>|<span data-ttu-id="2f9b4-138">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="2f9b4-138">Number of devices in conflict</span></span>|
|<span data-ttu-id="2f9b4-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="2f9b4-139">errorCount</span></span>|<span data-ttu-id="2f9b4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2f9b4-140">Int32</span></span>|<span data-ttu-id="2f9b4-141">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="2f9b4-141">Number of error devices</span></span>|
|<span data-ttu-id="2f9b4-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="2f9b4-142">failedCount</span></span>|<span data-ttu-id="2f9b4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2f9b4-143">Int32</span></span>|<span data-ttu-id="2f9b4-144">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="2f9b4-144">Number of failed devices</span></span>|
|<span data-ttu-id="2f9b4-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="2f9b4-145">notApplicableCount</span></span>|<span data-ttu-id="2f9b4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2f9b4-146">Int32</span></span>|<span data-ttu-id="2f9b4-147">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="2f9b4-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="2f9b4-148">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="2f9b4-148">notApplicablePlatformCount</span></span>|<span data-ttu-id="2f9b4-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2f9b4-149">Int32</span></span>|<span data-ttu-id="2f9b4-150">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="2f9b4-150">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="2f9b4-151">successCount</span><span class="sxs-lookup"><span data-stu-id="2f9b4-151">successCount</span></span>|<span data-ttu-id="2f9b4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2f9b4-152">Int32</span></span>|<span data-ttu-id="2f9b4-153">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="2f9b4-153">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="2f9b4-154">响应</span><span class="sxs-lookup"><span data-stu-id="2f9b4-154">Response</span></span>
<span data-ttu-id="2f9b4-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f9b4-156">示例</span><span class="sxs-lookup"><span data-stu-id="2f9b4-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f9b4-157">请求</span><span class="sxs-lookup"><span data-stu-id="2f9b4-157">Request</span></span>
<span data-ttu-id="2f9b4-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
Content-type: application/json
Content-length: 237

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```

### <a name="response"></a><span data-ttu-id="2f9b4-159">响应</span><span class="sxs-lookup"><span data-stu-id="2f9b4-159">Response</span></span>
<span data-ttu-id="2f9b4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f9b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "12230bf9-0bf9-1223-f90b-2312f90b2312",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```





