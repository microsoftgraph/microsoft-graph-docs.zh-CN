---
title: 更新 deviceManagementIntentDeviceSettingStateSummary
description: 更新 deviceManagementIntentDeviceSettingStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4fb26c4e4a60cde2aade117155402f7181232c0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690992"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="b793a-103">更新 deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="b793a-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="b793a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b793a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b793a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b793a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b793a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b793a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b793a-107">更新 [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b793a-107">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b793a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b793a-108">Prerequisites</span></span>
<span data-ttu-id="b793a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b793a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b793a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b793a-111">Permission type</span></span>|<span data-ttu-id="b793a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b793a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b793a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b793a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b793a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b793a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b793a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b793a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b793a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b793a-116">Not supported.</span></span>|
|<span data-ttu-id="b793a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b793a-117">Application</span></span>|<span data-ttu-id="b793a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b793a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b793a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b793a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="b793a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b793a-120">Request headers</span></span>
|<span data-ttu-id="b793a-121">标头</span><span class="sxs-lookup"><span data-stu-id="b793a-121">Header</span></span>|<span data-ttu-id="b793a-122">值</span><span class="sxs-lookup"><span data-stu-id="b793a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b793a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b793a-123">Authorization</span></span>|<span data-ttu-id="b793a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b793a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b793a-125">接受</span><span class="sxs-lookup"><span data-stu-id="b793a-125">Accept</span></span>|<span data-ttu-id="b793a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b793a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b793a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b793a-127">Request body</span></span>
<span data-ttu-id="b793a-128">在请求正文中，提供 [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b793a-128">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="b793a-129">下表显示创建 [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b793a-129">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="b793a-130">属性</span><span class="sxs-lookup"><span data-stu-id="b793a-130">Property</span></span>|<span data-ttu-id="b793a-131">类型</span><span class="sxs-lookup"><span data-stu-id="b793a-131">Type</span></span>|<span data-ttu-id="b793a-132">说明</span><span class="sxs-lookup"><span data-stu-id="b793a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b793a-133">id</span><span class="sxs-lookup"><span data-stu-id="b793a-133">id</span></span>|<span data-ttu-id="b793a-134">String</span><span class="sxs-lookup"><span data-stu-id="b793a-134">String</span></span>|<span data-ttu-id="b793a-135">ID</span><span class="sxs-lookup"><span data-stu-id="b793a-135">The ID</span></span>|
|<span data-ttu-id="b793a-136">settingName</span><span class="sxs-lookup"><span data-stu-id="b793a-136">settingName</span></span>|<span data-ttu-id="b793a-137">String</span><span class="sxs-lookup"><span data-stu-id="b793a-137">String</span></span>|<span data-ttu-id="b793a-138">设置的名称</span><span class="sxs-lookup"><span data-stu-id="b793a-138">Name of a setting</span></span>|
|<span data-ttu-id="b793a-139">compliantCount</span><span class="sxs-lookup"><span data-stu-id="b793a-139">compliantCount</span></span>|<span data-ttu-id="b793a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b793a-140">Int32</span></span>|<span data-ttu-id="b793a-141">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="b793a-141">Number of compliant devices</span></span>|
|<span data-ttu-id="b793a-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b793a-142">conflictCount</span></span>|<span data-ttu-id="b793a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b793a-143">Int32</span></span>|<span data-ttu-id="b793a-144">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="b793a-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="b793a-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="b793a-145">errorCount</span></span>|<span data-ttu-id="b793a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b793a-146">Int32</span></span>|<span data-ttu-id="b793a-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="b793a-147">Number of error devices</span></span>|
|<span data-ttu-id="b793a-148">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="b793a-148">nonCompliantCount</span></span>|<span data-ttu-id="b793a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b793a-149">Int32</span></span>|<span data-ttu-id="b793a-150">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="b793a-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="b793a-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b793a-151">notApplicableCount</span></span>|<span data-ttu-id="b793a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b793a-152">Int32</span></span>|<span data-ttu-id="b793a-153">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="b793a-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="b793a-154">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="b793a-154">remediatedCount</span></span>|<span data-ttu-id="b793a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="b793a-155">Int32</span></span>|<span data-ttu-id="b793a-156">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="b793a-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="b793a-157">响应</span><span class="sxs-lookup"><span data-stu-id="b793a-157">Response</span></span>
<span data-ttu-id="b793a-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b793a-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b793a-159">示例</span><span class="sxs-lookup"><span data-stu-id="b793a-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="b793a-160">请求</span><span class="sxs-lookup"><span data-stu-id="b793a-160">Request</span></span>
<span data-ttu-id="b793a-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b793a-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
Content-type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```

### <a name="response"></a><span data-ttu-id="b793a-162">响应</span><span class="sxs-lookup"><span data-stu-id="b793a-162">Response</span></span>
<span data-ttu-id="b793a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b793a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "d3d3a75f-a75f-d3d3-5fa7-d3d35fa7d3d3",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```





