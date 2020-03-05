---
title: 创建 deviceManagementIntentDeviceSettingStateSummary
description: 创建新的 deviceManagementIntentDeviceSettingStateSummary 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d29d3596c19ddbeb661ee3986787c0337ab2e80e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471062"
---
# <a name="create-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="5c67f-103">创建 deviceManagementIntentDeviceSettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="5c67f-103">Create deviceManagementIntentDeviceSettingStateSummary</span></span>

<span data-ttu-id="5c67f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5c67f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c67f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5c67f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c67f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5c67f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c67f-107">创建新的[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5c67f-107">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c67f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5c67f-108">Prerequisites</span></span>
<span data-ttu-id="5c67f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c67f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c67f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c67f-111">Permission type</span></span>|<span data-ttu-id="5c67f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5c67f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c67f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c67f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c67f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c67f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c67f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c67f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c67f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c67f-116">Not supported.</span></span>|
|<span data-ttu-id="5c67f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c67f-117">Application</span></span>|<span data-ttu-id="5c67f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c67f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c67f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c67f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="5c67f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c67f-120">Request headers</span></span>
|<span data-ttu-id="5c67f-121">标头</span><span class="sxs-lookup"><span data-stu-id="5c67f-121">Header</span></span>|<span data-ttu-id="5c67f-122">值</span><span class="sxs-lookup"><span data-stu-id="5c67f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c67f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c67f-123">Authorization</span></span>|<span data-ttu-id="5c67f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5c67f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c67f-125">接受</span><span class="sxs-lookup"><span data-stu-id="5c67f-125">Accept</span></span>|<span data-ttu-id="5c67f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c67f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c67f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c67f-127">Request body</span></span>
<span data-ttu-id="5c67f-128">在请求正文中，提供 deviceManagementIntentDeviceSettingStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c67f-128">In the request body, supply a JSON representation for the deviceManagementIntentDeviceSettingStateSummary object.</span></span>

<span data-ttu-id="5c67f-129">下表显示创建 deviceManagementIntentDeviceSettingStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5c67f-129">The following table shows the properties that are required when you create the deviceManagementIntentDeviceSettingStateSummary.</span></span>

|<span data-ttu-id="5c67f-130">属性</span><span class="sxs-lookup"><span data-stu-id="5c67f-130">Property</span></span>|<span data-ttu-id="5c67f-131">类型</span><span class="sxs-lookup"><span data-stu-id="5c67f-131">Type</span></span>|<span data-ttu-id="5c67f-132">说明</span><span class="sxs-lookup"><span data-stu-id="5c67f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c67f-133">id</span><span class="sxs-lookup"><span data-stu-id="5c67f-133">id</span></span>|<span data-ttu-id="5c67f-134">String</span><span class="sxs-lookup"><span data-stu-id="5c67f-134">String</span></span>|<span data-ttu-id="5c67f-135">ID</span><span class="sxs-lookup"><span data-stu-id="5c67f-135">The ID</span></span>|
|<span data-ttu-id="5c67f-136">settingName</span><span class="sxs-lookup"><span data-stu-id="5c67f-136">settingName</span></span>|<span data-ttu-id="5c67f-137">String</span><span class="sxs-lookup"><span data-stu-id="5c67f-137">String</span></span>|<span data-ttu-id="5c67f-138">设置的名称</span><span class="sxs-lookup"><span data-stu-id="5c67f-138">Name of a setting</span></span>|
|<span data-ttu-id="5c67f-139">compliantCount</span><span class="sxs-lookup"><span data-stu-id="5c67f-139">compliantCount</span></span>|<span data-ttu-id="5c67f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5c67f-140">Int32</span></span>|<span data-ttu-id="5c67f-141">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="5c67f-141">Number of compliant devices</span></span>|
|<span data-ttu-id="5c67f-142">conflictCount</span><span class="sxs-lookup"><span data-stu-id="5c67f-142">conflictCount</span></span>|<span data-ttu-id="5c67f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5c67f-143">Int32</span></span>|<span data-ttu-id="5c67f-144">发生冲突的设备数</span><span class="sxs-lookup"><span data-stu-id="5c67f-144">Number of devices in conflict</span></span>|
|<span data-ttu-id="5c67f-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="5c67f-145">errorCount</span></span>|<span data-ttu-id="5c67f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5c67f-146">Int32</span></span>|<span data-ttu-id="5c67f-147">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="5c67f-147">Number of error devices</span></span>|
|<span data-ttu-id="5c67f-148">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="5c67f-148">nonCompliantCount</span></span>|<span data-ttu-id="5c67f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5c67f-149">Int32</span></span>|<span data-ttu-id="5c67f-150">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="5c67f-150">Number of non compliant devices</span></span>|
|<span data-ttu-id="5c67f-151">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="5c67f-151">notApplicableCount</span></span>|<span data-ttu-id="5c67f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5c67f-152">Int32</span></span>|<span data-ttu-id="5c67f-153">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="5c67f-153">Number of not applicable devices</span></span>|
|<span data-ttu-id="5c67f-154">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="5c67f-154">remediatedCount</span></span>|<span data-ttu-id="5c67f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="5c67f-155">Int32</span></span>|<span data-ttu-id="5c67f-156">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="5c67f-156">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="5c67f-157">响应</span><span class="sxs-lookup"><span data-stu-id="5c67f-157">Response</span></span>
<span data-ttu-id="5c67f-158">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5c67f-158">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c67f-159">示例</span><span class="sxs-lookup"><span data-stu-id="5c67f-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c67f-160">请求</span><span class="sxs-lookup"><span data-stu-id="5c67f-160">Request</span></span>
<span data-ttu-id="5c67f-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c67f-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5c67f-162">响应</span><span class="sxs-lookup"><span data-stu-id="5c67f-162">Response</span></span>
<span data-ttu-id="5c67f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c67f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





