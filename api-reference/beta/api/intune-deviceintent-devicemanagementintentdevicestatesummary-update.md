---
title: 更新 deviceManagementIntentDeviceStateSummary
description: 更新 deviceManagementIntentDeviceStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0556f44326e76563374d3e84497f1f9ed3dbf1c2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130964"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="50c0e-103">更新 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="50c0e-103">Update deviceManagementIntentDeviceStateSummary</span></span>

<span data-ttu-id="50c0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50c0e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50c0e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50c0e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50c0e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50c0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50c0e-107">更新 [deviceManagementIntentDeviceStateSummary 对象](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="50c0e-107">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50c0e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="50c0e-108">Prerequisites</span></span>
<span data-ttu-id="50c0e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50c0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50c0e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="50c0e-111">Permission type</span></span>|<span data-ttu-id="50c0e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50c0e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50c0e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50c0e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50c0e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50c0e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50c0e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50c0e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50c0e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="50c0e-116">Not supported.</span></span>|
|<span data-ttu-id="50c0e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="50c0e-117">Application</span></span>|<span data-ttu-id="50c0e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50c0e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50c0e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50c0e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="50c0e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="50c0e-120">Request headers</span></span>
|<span data-ttu-id="50c0e-121">标头</span><span class="sxs-lookup"><span data-stu-id="50c0e-121">Header</span></span>|<span data-ttu-id="50c0e-122">值</span><span class="sxs-lookup"><span data-stu-id="50c0e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50c0e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50c0e-123">Authorization</span></span>|<span data-ttu-id="50c0e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50c0e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50c0e-125">接受</span><span class="sxs-lookup"><span data-stu-id="50c0e-125">Accept</span></span>|<span data-ttu-id="50c0e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50c0e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50c0e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="50c0e-127">Request body</span></span>
<span data-ttu-id="50c0e-128">在请求正文中，提供 [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50c0e-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="50c0e-129">下表显示创建 [deviceManagementIntentDeviceStateSummary 时所需的属性](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)。</span><span class="sxs-lookup"><span data-stu-id="50c0e-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="50c0e-130">属性</span><span class="sxs-lookup"><span data-stu-id="50c0e-130">Property</span></span>|<span data-ttu-id="50c0e-131">类型</span><span class="sxs-lookup"><span data-stu-id="50c0e-131">Type</span></span>|<span data-ttu-id="50c0e-132">说明</span><span class="sxs-lookup"><span data-stu-id="50c0e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50c0e-133">id</span><span class="sxs-lookup"><span data-stu-id="50c0e-133">id</span></span>|<span data-ttu-id="50c0e-134">String</span><span class="sxs-lookup"><span data-stu-id="50c0e-134">String</span></span>|<span data-ttu-id="50c0e-135">The ID</span><span class="sxs-lookup"><span data-stu-id="50c0e-135">The ID</span></span>|
|<span data-ttu-id="50c0e-136">conflictCount</span><span class="sxs-lookup"><span data-stu-id="50c0e-136">conflictCount</span></span>|<span data-ttu-id="50c0e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="50c0e-137">Int32</span></span>|<span data-ttu-id="50c0e-138">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="50c0e-138">Number of devices in conflict</span></span>|
|<span data-ttu-id="50c0e-139">errorCount</span><span class="sxs-lookup"><span data-stu-id="50c0e-139">errorCount</span></span>|<span data-ttu-id="50c0e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="50c0e-140">Int32</span></span>|<span data-ttu-id="50c0e-141">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="50c0e-141">Number of error devices</span></span>|
|<span data-ttu-id="50c0e-142">failedCount</span><span class="sxs-lookup"><span data-stu-id="50c0e-142">failedCount</span></span>|<span data-ttu-id="50c0e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="50c0e-143">Int32</span></span>|<span data-ttu-id="50c0e-144">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="50c0e-144">Number of failed devices</span></span>|
|<span data-ttu-id="50c0e-145">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="50c0e-145">notApplicableCount</span></span>|<span data-ttu-id="50c0e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="50c0e-146">Int32</span></span>|<span data-ttu-id="50c0e-147">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="50c0e-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="50c0e-148">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="50c0e-148">notApplicablePlatformCount</span></span>|<span data-ttu-id="50c0e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="50c0e-149">Int32</span></span>|<span data-ttu-id="50c0e-150">由于平台和策略不匹配而不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="50c0e-150">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="50c0e-151">successCount</span><span class="sxs-lookup"><span data-stu-id="50c0e-151">successCount</span></span>|<span data-ttu-id="50c0e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="50c0e-152">Int32</span></span>|<span data-ttu-id="50c0e-153">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="50c0e-153">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="50c0e-154">响应</span><span class="sxs-lookup"><span data-stu-id="50c0e-154">Response</span></span>
<span data-ttu-id="50c0e-155">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50c0e-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50c0e-156">示例</span><span class="sxs-lookup"><span data-stu-id="50c0e-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="50c0e-157">请求</span><span class="sxs-lookup"><span data-stu-id="50c0e-157">Request</span></span>
<span data-ttu-id="50c0e-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50c0e-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50c0e-159">响应</span><span class="sxs-lookup"><span data-stu-id="50c0e-159">Response</span></span>
<span data-ttu-id="50c0e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50c0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




