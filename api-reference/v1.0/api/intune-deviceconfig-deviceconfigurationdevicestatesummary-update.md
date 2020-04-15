---
title: 更新 deviceConfigurationDeviceStateSummary
description: 更新 deviceConfigurationDeviceStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a0229b605a9aa7bbee3b2555c74823edf9ced43c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460690"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="43af8-103">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="43af8-103">Update deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="43af8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43af8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43af8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43af8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43af8-106">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="43af8-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43af8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="43af8-107">Prerequisites</span></span>
<span data-ttu-id="43af8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43af8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43af8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="43af8-110">Permission type</span></span>|<span data-ttu-id="43af8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="43af8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43af8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43af8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43af8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43af8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43af8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43af8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43af8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="43af8-115">Not supported.</span></span>|
|<span data-ttu-id="43af8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="43af8-116">Application</span></span>|<span data-ttu-id="43af8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="43af8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43af8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43af8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="43af8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="43af8-119">Request headers</span></span>
|<span data-ttu-id="43af8-120">标头</span><span class="sxs-lookup"><span data-stu-id="43af8-120">Header</span></span>|<span data-ttu-id="43af8-121">值</span><span class="sxs-lookup"><span data-stu-id="43af8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43af8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43af8-122">Authorization</span></span>|<span data-ttu-id="43af8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43af8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43af8-124">接受</span><span class="sxs-lookup"><span data-stu-id="43af8-124">Accept</span></span>|<span data-ttu-id="43af8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43af8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43af8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="43af8-126">Request body</span></span>
<span data-ttu-id="43af8-127">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43af8-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="43af8-128">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="43af8-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="43af8-129">属性</span><span class="sxs-lookup"><span data-stu-id="43af8-129">Property</span></span>|<span data-ttu-id="43af8-130">类型</span><span class="sxs-lookup"><span data-stu-id="43af8-130">Type</span></span>|<span data-ttu-id="43af8-131">说明</span><span class="sxs-lookup"><span data-stu-id="43af8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43af8-132">id</span><span class="sxs-lookup"><span data-stu-id="43af8-132">id</span></span>|<span data-ttu-id="43af8-133">String</span><span class="sxs-lookup"><span data-stu-id="43af8-133">String</span></span>|<span data-ttu-id="43af8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="43af8-134">Key of the entity.</span></span>|
|<span data-ttu-id="43af8-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43af8-135">unknownDeviceCount</span></span>|<span data-ttu-id="43af8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="43af8-136">Int32</span></span>|<span data-ttu-id="43af8-137">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="43af8-137">Number of unknown devices</span></span>|
|<span data-ttu-id="43af8-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43af8-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="43af8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="43af8-139">Int32</span></span>|<span data-ttu-id="43af8-140">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="43af8-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="43af8-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43af8-141">compliantDeviceCount</span></span>|<span data-ttu-id="43af8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="43af8-142">Int32</span></span>|<span data-ttu-id="43af8-143">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="43af8-143">Number of compliant devices</span></span>|
|<span data-ttu-id="43af8-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43af8-144">remediatedDeviceCount</span></span>|<span data-ttu-id="43af8-145">Int32</span><span class="sxs-lookup"><span data-stu-id="43af8-145">Int32</span></span>|<span data-ttu-id="43af8-146">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="43af8-146">Number of remediated devices</span></span>|
|<span data-ttu-id="43af8-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43af8-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="43af8-148">Int32</span><span class="sxs-lookup"><span data-stu-id="43af8-148">Int32</span></span>|<span data-ttu-id="43af8-149">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="43af8-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="43af8-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43af8-150">errorDeviceCount</span></span>|<span data-ttu-id="43af8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="43af8-151">Int32</span></span>|<span data-ttu-id="43af8-152">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="43af8-152">Number of error devices</span></span>|
|<span data-ttu-id="43af8-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="43af8-153">conflictDeviceCount</span></span>|<span data-ttu-id="43af8-154">Int32</span><span class="sxs-lookup"><span data-stu-id="43af8-154">Int32</span></span>|<span data-ttu-id="43af8-155">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="43af8-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="43af8-156">响应</span><span class="sxs-lookup"><span data-stu-id="43af8-156">Response</span></span>
<span data-ttu-id="43af8-157">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43af8-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43af8-158">示例</span><span class="sxs-lookup"><span data-stu-id="43af8-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="43af8-159">请求</span><span class="sxs-lookup"><span data-stu-id="43af8-159">Request</span></span>
<span data-ttu-id="43af8-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43af8-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43af8-161">响应</span><span class="sxs-lookup"><span data-stu-id="43af8-161">Response</span></span>
<span data-ttu-id="43af8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43af8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






