---
title: 创建 deviceManagementIntentDeviceSettingStateSummary
description: 创建新的 deviceManagementIntentDeviceSettingStateSummary 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4bfe4c44bdd0ec2a68e58c3a881dbe00ae1b7f5e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787601"
---
# <a name="create-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="fb772-103">创建 deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="fb772-103">Create deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="fb772-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb772-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb772-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb772-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb772-106">创建新的[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fb772-106">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb772-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fb772-107">Prerequisites</span></span>
<span data-ttu-id="fb772-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb772-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb772-110">Permission type</span></span>|<span data-ttu-id="fb772-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb772-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb772-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb772-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb772-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb772-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb772-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb772-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb772-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb772-115">Not supported.</span></span>|
|<span data-ttu-id="fb772-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb772-116">Application</span></span>|<span data-ttu-id="fb772-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb772-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb772-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb772-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="fb772-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb772-119">Request headers</span></span>
|<span data-ttu-id="fb772-120">标头</span><span class="sxs-lookup"><span data-stu-id="fb772-120">Header</span></span>|<span data-ttu-id="fb772-121">值</span><span class="sxs-lookup"><span data-stu-id="fb772-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb772-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb772-122">Authorization</span></span>|<span data-ttu-id="fb772-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fb772-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb772-124">接受</span><span class="sxs-lookup"><span data-stu-id="fb772-124">Accept</span></span>|<span data-ttu-id="fb772-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fb772-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb772-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb772-126">Request body</span></span>
<span data-ttu-id="fb772-127">在请求正文中, 提供 deviceManagementIntentDeviceSettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb772-127">In the request body, supply a JSON representation for the deviceManagementIntentDeviceSettingStateSummary object.</span></span>

<span data-ttu-id="fb772-128">下表显示创建 deviceManagementIntentDeviceSettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb772-128">The following table shows the properties that are required when you create the deviceManagementIntentDeviceSettingStateSummary.</span></span>

|<span data-ttu-id="fb772-129">属性</span><span class="sxs-lookup"><span data-stu-id="fb772-129">Property</span></span>|<span data-ttu-id="fb772-130">类型</span><span class="sxs-lookup"><span data-stu-id="fb772-130">Type</span></span>|<span data-ttu-id="fb772-131">说明</span><span class="sxs-lookup"><span data-stu-id="fb772-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb772-132">id</span><span class="sxs-lookup"><span data-stu-id="fb772-132">id</span></span>|<span data-ttu-id="fb772-133">String</span><span class="sxs-lookup"><span data-stu-id="fb772-133">String</span></span>|<span data-ttu-id="fb772-134">ID</span><span class="sxs-lookup"><span data-stu-id="fb772-134">The ID</span></span>|
|<span data-ttu-id="fb772-135">settingName</span><span class="sxs-lookup"><span data-stu-id="fb772-135">settingName</span></span>|<span data-ttu-id="fb772-136">String</span><span class="sxs-lookup"><span data-stu-id="fb772-136">String</span></span>|<span data-ttu-id="fb772-137">设置的名称</span><span class="sxs-lookup"><span data-stu-id="fb772-137">Name of a setting</span></span>|
|<span data-ttu-id="fb772-138">compliantCount</span><span class="sxs-lookup"><span data-stu-id="fb772-138">compliantCount</span></span>|<span data-ttu-id="fb772-139">Int32</span><span class="sxs-lookup"><span data-stu-id="fb772-139">Int32</span></span>|<span data-ttu-id="fb772-140">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="fb772-140">Number of compliant devices</span></span>|
|<span data-ttu-id="fb772-141">conflictCount</span><span class="sxs-lookup"><span data-stu-id="fb772-141">conflictCount</span></span>|<span data-ttu-id="fb772-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fb772-142">Int32</span></span>|<span data-ttu-id="fb772-143">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="fb772-143">Number of devices in conflict</span></span>|
|<span data-ttu-id="fb772-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="fb772-144">errorCount</span></span>|<span data-ttu-id="fb772-145">Int32</span><span class="sxs-lookup"><span data-stu-id="fb772-145">Int32</span></span>|<span data-ttu-id="fb772-146">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="fb772-146">Number of error devices</span></span>|
|<span data-ttu-id="fb772-147">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="fb772-147">nonCompliantCount</span></span>|<span data-ttu-id="fb772-148">Int32</span><span class="sxs-lookup"><span data-stu-id="fb772-148">Int32</span></span>|<span data-ttu-id="fb772-149">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="fb772-149">Number of non compliant devices</span></span>|
|<span data-ttu-id="fb772-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="fb772-150">notApplicableCount</span></span>|<span data-ttu-id="fb772-151">Int32</span><span class="sxs-lookup"><span data-stu-id="fb772-151">Int32</span></span>|<span data-ttu-id="fb772-152">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="fb772-152">Number of not applicable devices</span></span>|
|<span data-ttu-id="fb772-153">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="fb772-153">remediatedCount</span></span>|<span data-ttu-id="fb772-154">Int32</span><span class="sxs-lookup"><span data-stu-id="fb772-154">Int32</span></span>|<span data-ttu-id="fb772-155">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="fb772-155">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="fb772-156">响应</span><span class="sxs-lookup"><span data-stu-id="fb772-156">Response</span></span>
<span data-ttu-id="fb772-157">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fb772-157">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb772-158">示例</span><span class="sxs-lookup"><span data-stu-id="fb772-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb772-159">请求</span><span class="sxs-lookup"><span data-stu-id="fb772-159">Request</span></span>
<span data-ttu-id="fb772-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fb772-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="fb772-161">响应</span><span class="sxs-lookup"><span data-stu-id="fb772-161">Response</span></span>
<span data-ttu-id="fb772-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fb772-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





