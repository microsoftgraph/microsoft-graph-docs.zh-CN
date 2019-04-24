---
title: 更新 deviceManagementIntentDeviceStateSummary
description: 更新 deviceManagementIntentDeviceStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d790aaf3e0218d7313c6999ace76a443925ecec2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32508293"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="8c90a-103">更新 deviceManagementIntentDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="8c90a-103">Update deviceManagementIntentDeviceStateSummary</span></span>

> <span data-ttu-id="8c90a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c90a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c90a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c90a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c90a-106">更新[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8c90a-106">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c90a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c90a-107">Prerequisites</span></span>
<span data-ttu-id="8c90a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8c90a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c90a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c90a-110">Permission type</span></span>|<span data-ttu-id="8c90a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c90a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c90a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c90a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c90a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c90a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8c90a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c90a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c90a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c90a-115">Not supported.</span></span>|
|<span data-ttu-id="8c90a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c90a-116">Application</span></span>|<span data-ttu-id="8c90a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c90a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c90a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c90a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="8c90a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c90a-119">Request headers</span></span>
|<span data-ttu-id="8c90a-120">标头</span><span class="sxs-lookup"><span data-stu-id="8c90a-120">Header</span></span>|<span data-ttu-id="8c90a-121">值</span><span class="sxs-lookup"><span data-stu-id="8c90a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c90a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c90a-122">Authorization</span></span>|<span data-ttu-id="8c90a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c90a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c90a-124">接受</span><span class="sxs-lookup"><span data-stu-id="8c90a-124">Accept</span></span>|<span data-ttu-id="8c90a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c90a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c90a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c90a-126">Request body</span></span>
<span data-ttu-id="8c90a-127">在请求正文中, 提供[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c90a-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="8c90a-128">下表显示创建[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8c90a-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="8c90a-129">属性</span><span class="sxs-lookup"><span data-stu-id="8c90a-129">Property</span></span>|<span data-ttu-id="8c90a-130">类型</span><span class="sxs-lookup"><span data-stu-id="8c90a-130">Type</span></span>|<span data-ttu-id="8c90a-131">说明</span><span class="sxs-lookup"><span data-stu-id="8c90a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c90a-132">id</span><span class="sxs-lookup"><span data-stu-id="8c90a-132">id</span></span>|<span data-ttu-id="8c90a-133">String</span><span class="sxs-lookup"><span data-stu-id="8c90a-133">String</span></span>|<span data-ttu-id="8c90a-134">ID</span><span class="sxs-lookup"><span data-stu-id="8c90a-134">The ID</span></span>|
|<span data-ttu-id="8c90a-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="8c90a-135">conflictCount</span></span>|<span data-ttu-id="8c90a-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8c90a-136">Int32</span></span>|<span data-ttu-id="8c90a-137">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="8c90a-137">Number of devices in conflict</span></span>|
|<span data-ttu-id="8c90a-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="8c90a-138">errorCount</span></span>|<span data-ttu-id="8c90a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8c90a-139">Int32</span></span>|<span data-ttu-id="8c90a-140">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="8c90a-140">Number of error devices</span></span>|
|<span data-ttu-id="8c90a-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="8c90a-141">failedCount</span></span>|<span data-ttu-id="8c90a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8c90a-142">Int32</span></span>|<span data-ttu-id="8c90a-143">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="8c90a-143">Number of failed devices</span></span>|
|<span data-ttu-id="8c90a-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="8c90a-144">notApplicableCount</span></span>|<span data-ttu-id="8c90a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="8c90a-145">Int32</span></span>|<span data-ttu-id="8c90a-146">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="8c90a-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="8c90a-147">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="8c90a-147">notApplicablePlatformCount</span></span>|<span data-ttu-id="8c90a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8c90a-148">Int32</span></span>|<span data-ttu-id="8c90a-149">由于平台和策略不匹配而导致不适用的设备数量</span><span class="sxs-lookup"><span data-stu-id="8c90a-149">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="8c90a-150">successCount</span><span class="sxs-lookup"><span data-stu-id="8c90a-150">successCount</span></span>|<span data-ttu-id="8c90a-151">Int32</span><span class="sxs-lookup"><span data-stu-id="8c90a-151">Int32</span></span>|<span data-ttu-id="8c90a-152">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="8c90a-152">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="8c90a-153">响应</span><span class="sxs-lookup"><span data-stu-id="8c90a-153">Response</span></span>
<span data-ttu-id="8c90a-154">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8c90a-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c90a-155">示例</span><span class="sxs-lookup"><span data-stu-id="8c90a-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c90a-156">请求</span><span class="sxs-lookup"><span data-stu-id="8c90a-156">Request</span></span>
<span data-ttu-id="8c90a-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c90a-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8c90a-158">响应</span><span class="sxs-lookup"><span data-stu-id="8c90a-158">Response</span></span>
<span data-ttu-id="8c90a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c90a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





