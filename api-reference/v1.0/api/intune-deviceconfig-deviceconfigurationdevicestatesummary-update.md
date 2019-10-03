---
title: 更新 deviceConfigurationDeviceStateSummary
description: 更新 deviceConfigurationDeviceStateSummary 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7161455a6f0b341a0d88008f5e8b7e167e1e1f24
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368685"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="52196-103">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="52196-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="52196-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="52196-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52196-105">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="52196-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52196-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="52196-106">Prerequisites</span></span>
<span data-ttu-id="52196-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52196-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="52196-109">Permission type</span></span>|<span data-ttu-id="52196-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="52196-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52196-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52196-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52196-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52196-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52196-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52196-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52196-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="52196-114">Not supported.</span></span>|
|<span data-ttu-id="52196-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="52196-115">Application</span></span>|<span data-ttu-id="52196-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="52196-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52196-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52196-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="52196-118">请求头</span><span class="sxs-lookup"><span data-stu-id="52196-118">Request headers</span></span>
|<span data-ttu-id="52196-119">标头</span><span class="sxs-lookup"><span data-stu-id="52196-119">Header</span></span>|<span data-ttu-id="52196-120">值</span><span class="sxs-lookup"><span data-stu-id="52196-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52196-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="52196-121">Authorization</span></span>|<span data-ttu-id="52196-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="52196-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52196-123">接受</span><span class="sxs-lookup"><span data-stu-id="52196-123">Accept</span></span>|<span data-ttu-id="52196-124">application/json</span><span class="sxs-lookup"><span data-stu-id="52196-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52196-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="52196-125">Request body</span></span>
<span data-ttu-id="52196-126">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52196-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="52196-127">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="52196-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="52196-128">属性</span><span class="sxs-lookup"><span data-stu-id="52196-128">Property</span></span>|<span data-ttu-id="52196-129">类型</span><span class="sxs-lookup"><span data-stu-id="52196-129">Type</span></span>|<span data-ttu-id="52196-130">说明</span><span class="sxs-lookup"><span data-stu-id="52196-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52196-131">id</span><span class="sxs-lookup"><span data-stu-id="52196-131">id</span></span>|<span data-ttu-id="52196-132">String</span><span class="sxs-lookup"><span data-stu-id="52196-132">String</span></span>|<span data-ttu-id="52196-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="52196-133">Key of the entity.</span></span>|
|<span data-ttu-id="52196-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="52196-134">unknownDeviceCount</span></span>|<span data-ttu-id="52196-135">Int32</span><span class="sxs-lookup"><span data-stu-id="52196-135">Int32</span></span>|<span data-ttu-id="52196-136">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="52196-136">Number of unknown devices</span></span>|
|<span data-ttu-id="52196-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="52196-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="52196-138">Int32</span><span class="sxs-lookup"><span data-stu-id="52196-138">Int32</span></span>|<span data-ttu-id="52196-139">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="52196-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="52196-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="52196-140">compliantDeviceCount</span></span>|<span data-ttu-id="52196-141">Int32</span><span class="sxs-lookup"><span data-stu-id="52196-141">Int32</span></span>|<span data-ttu-id="52196-142">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="52196-142">Number of compliant devices</span></span>|
|<span data-ttu-id="52196-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="52196-143">remediatedDeviceCount</span></span>|<span data-ttu-id="52196-144">Int32</span><span class="sxs-lookup"><span data-stu-id="52196-144">Int32</span></span>|<span data-ttu-id="52196-145">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="52196-145">Number of remediated devices</span></span>|
|<span data-ttu-id="52196-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="52196-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="52196-147">Int32</span><span class="sxs-lookup"><span data-stu-id="52196-147">Int32</span></span>|<span data-ttu-id="52196-148">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="52196-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="52196-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="52196-149">errorDeviceCount</span></span>|<span data-ttu-id="52196-150">Int32</span><span class="sxs-lookup"><span data-stu-id="52196-150">Int32</span></span>|<span data-ttu-id="52196-151">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="52196-151">Number of error devices</span></span>|
|<span data-ttu-id="52196-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="52196-152">conflictDeviceCount</span></span>|<span data-ttu-id="52196-153">Int32</span><span class="sxs-lookup"><span data-stu-id="52196-153">Int32</span></span>|<span data-ttu-id="52196-154">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="52196-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="52196-155">响应</span><span class="sxs-lookup"><span data-stu-id="52196-155">Response</span></span>
<span data-ttu-id="52196-156">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52196-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52196-157">示例</span><span class="sxs-lookup"><span data-stu-id="52196-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="52196-158">请求</span><span class="sxs-lookup"><span data-stu-id="52196-158">Request</span></span>
<span data-ttu-id="52196-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="52196-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="52196-160">响应</span><span class="sxs-lookup"><span data-stu-id="52196-160">Response</span></span>
<span data-ttu-id="52196-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="52196-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




