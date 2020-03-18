---
title: 更新 deviceManagementIntentDeviceStateSummary
description: 更新 deviceManagementIntentDeviceStateSummary 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: de70cd0e2ac314dad0baaf271b57525be59b73af
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42815224"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="da9ee-103">更新 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="da9ee-103">Update deviceManagementIntentDeviceStateSummary</span></span>

> <span data-ttu-id="da9ee-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da9ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da9ee-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da9ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da9ee-106">更新[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="da9ee-106">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da9ee-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="da9ee-107">Prerequisites</span></span>
<span data-ttu-id="da9ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da9ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da9ee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="da9ee-110">Permission type</span></span>|<span data-ttu-id="da9ee-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da9ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da9ee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da9ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da9ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da9ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da9ee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da9ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da9ee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da9ee-115">Not supported.</span></span>|
|<span data-ttu-id="da9ee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="da9ee-116">Application</span></span>|<span data-ttu-id="da9ee-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da9ee-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da9ee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da9ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="da9ee-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="da9ee-119">Request headers</span></span>
|<span data-ttu-id="da9ee-120">标头</span><span class="sxs-lookup"><span data-stu-id="da9ee-120">Header</span></span>|<span data-ttu-id="da9ee-121">值</span><span class="sxs-lookup"><span data-stu-id="da9ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da9ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da9ee-122">Authorization</span></span>|<span data-ttu-id="da9ee-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da9ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da9ee-124">接受</span><span class="sxs-lookup"><span data-stu-id="da9ee-124">Accept</span></span>|<span data-ttu-id="da9ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da9ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da9ee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="da9ee-126">Request body</span></span>
<span data-ttu-id="da9ee-127">在请求正文中，提供[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da9ee-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="da9ee-128">下表显示创建[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da9ee-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="da9ee-129">属性</span><span class="sxs-lookup"><span data-stu-id="da9ee-129">Property</span></span>|<span data-ttu-id="da9ee-130">类型</span><span class="sxs-lookup"><span data-stu-id="da9ee-130">Type</span></span>|<span data-ttu-id="da9ee-131">说明</span><span class="sxs-lookup"><span data-stu-id="da9ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da9ee-132">id</span><span class="sxs-lookup"><span data-stu-id="da9ee-132">id</span></span>|<span data-ttu-id="da9ee-133">String</span><span class="sxs-lookup"><span data-stu-id="da9ee-133">String</span></span>|<span data-ttu-id="da9ee-134">ID</span><span class="sxs-lookup"><span data-stu-id="da9ee-134">The ID</span></span>|
|<span data-ttu-id="da9ee-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="da9ee-135">conflictCount</span></span>|<span data-ttu-id="da9ee-136">Int32</span><span class="sxs-lookup"><span data-stu-id="da9ee-136">Int32</span></span>|<span data-ttu-id="da9ee-137">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="da9ee-137">Number of devices in conflict</span></span>|
|<span data-ttu-id="da9ee-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="da9ee-138">errorCount</span></span>|<span data-ttu-id="da9ee-139">Int32</span><span class="sxs-lookup"><span data-stu-id="da9ee-139">Int32</span></span>|<span data-ttu-id="da9ee-140">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="da9ee-140">Number of error devices</span></span>|
|<span data-ttu-id="da9ee-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="da9ee-141">failedCount</span></span>|<span data-ttu-id="da9ee-142">Int32</span><span class="sxs-lookup"><span data-stu-id="da9ee-142">Int32</span></span>|<span data-ttu-id="da9ee-143">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="da9ee-143">Number of failed devices</span></span>|
|<span data-ttu-id="da9ee-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="da9ee-144">notApplicableCount</span></span>|<span data-ttu-id="da9ee-145">Int32</span><span class="sxs-lookup"><span data-stu-id="da9ee-145">Int32</span></span>|<span data-ttu-id="da9ee-146">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="da9ee-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="da9ee-147">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="da9ee-147">notApplicablePlatformCount</span></span>|<span data-ttu-id="da9ee-148">Int32</span><span class="sxs-lookup"><span data-stu-id="da9ee-148">Int32</span></span>|<span data-ttu-id="da9ee-149">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="da9ee-149">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="da9ee-150">successCount</span><span class="sxs-lookup"><span data-stu-id="da9ee-150">successCount</span></span>|<span data-ttu-id="da9ee-151">Int32</span><span class="sxs-lookup"><span data-stu-id="da9ee-151">Int32</span></span>|<span data-ttu-id="da9ee-152">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="da9ee-152">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="da9ee-153">响应</span><span class="sxs-lookup"><span data-stu-id="da9ee-153">Response</span></span>
<span data-ttu-id="da9ee-154">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da9ee-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da9ee-155">示例</span><span class="sxs-lookup"><span data-stu-id="da9ee-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="da9ee-156">请求</span><span class="sxs-lookup"><span data-stu-id="da9ee-156">Request</span></span>
<span data-ttu-id="da9ee-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da9ee-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="da9ee-158">响应</span><span class="sxs-lookup"><span data-stu-id="da9ee-158">Response</span></span>
<span data-ttu-id="da9ee-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da9ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




