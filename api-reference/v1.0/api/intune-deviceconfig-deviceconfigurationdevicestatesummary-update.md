---
title: 更新 deviceConfigurationDeviceStateSummary
description: 更新 deviceConfigurationDeviceStateSummary 对象的属性。
ms.openlocfilehash: a65ce289ad7c5c95b9a5ba344493c46d3dd14822
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010322"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="b4d18-103">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b4d18-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="b4d18-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b4d18-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4d18-105">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b4d18-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4d18-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4d18-106">Prerequisites</span></span>
<span data-ttu-id="b4d18-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b4d18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4d18-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4d18-109">Permission type</span></span>|<span data-ttu-id="b4d18-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b4d18-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4d18-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4d18-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4d18-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4d18-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4d18-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4d18-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4d18-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4d18-114">Not supported.</span></span>|
|<span data-ttu-id="b4d18-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4d18-115">Application</span></span>|<span data-ttu-id="b4d18-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4d18-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4d18-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4d18-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="b4d18-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4d18-118">Request headers</span></span>
|<span data-ttu-id="b4d18-119">标头</span><span class="sxs-lookup"><span data-stu-id="b4d18-119">Header</span></span>|<span data-ttu-id="b4d18-120">值</span><span class="sxs-lookup"><span data-stu-id="b4d18-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4d18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4d18-121">Authorization</span></span>|<span data-ttu-id="b4d18-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b4d18-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4d18-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b4d18-123">Accept</span></span>|<span data-ttu-id="b4d18-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b4d18-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4d18-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4d18-125">Request body</span></span>
<span data-ttu-id="b4d18-126">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4d18-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="b4d18-127">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b4d18-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="b4d18-128">属性</span><span class="sxs-lookup"><span data-stu-id="b4d18-128">Property</span></span>|<span data-ttu-id="b4d18-129">类型</span><span class="sxs-lookup"><span data-stu-id="b4d18-129">Type</span></span>|<span data-ttu-id="b4d18-130">说明</span><span class="sxs-lookup"><span data-stu-id="b4d18-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d18-131">id</span><span class="sxs-lookup"><span data-stu-id="b4d18-131">id</span></span>|<span data-ttu-id="b4d18-132">String</span><span class="sxs-lookup"><span data-stu-id="b4d18-132">String</span></span>|<span data-ttu-id="b4d18-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b4d18-133">Key of the entity.</span></span>|
|<span data-ttu-id="b4d18-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4d18-134">unknownDeviceCount</span></span>|<span data-ttu-id="b4d18-135">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d18-135">Int32</span></span>|<span data-ttu-id="b4d18-136">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="b4d18-136">Number of unknown devices</span></span>|
|<span data-ttu-id="b4d18-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4d18-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="b4d18-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d18-138">Int32</span></span>|<span data-ttu-id="b4d18-139">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="b4d18-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="b4d18-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4d18-140">compliantDeviceCount</span></span>|<span data-ttu-id="b4d18-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d18-141">Int32</span></span>|<span data-ttu-id="b4d18-142">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="b4d18-142">Number of compliant devices</span></span>|
|<span data-ttu-id="b4d18-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4d18-143">remediatedDeviceCount</span></span>|<span data-ttu-id="b4d18-144">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d18-144">Int32</span></span>|<span data-ttu-id="b4d18-145">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="b4d18-145">Number of remediated devices</span></span>|
|<span data-ttu-id="b4d18-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4d18-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="b4d18-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d18-147">Int32</span></span>|<span data-ttu-id="b4d18-148">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="b4d18-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="b4d18-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4d18-149">errorDeviceCount</span></span>|<span data-ttu-id="b4d18-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d18-150">Int32</span></span>|<span data-ttu-id="b4d18-151">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="b4d18-151">Number of error devices</span></span>|
|<span data-ttu-id="b4d18-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="b4d18-152">conflictDeviceCount</span></span>|<span data-ttu-id="b4d18-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b4d18-153">Int32</span></span>|<span data-ttu-id="b4d18-154">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="b4d18-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="b4d18-155">响应</span><span class="sxs-lookup"><span data-stu-id="b4d18-155">Response</span></span>
<span data-ttu-id="b4d18-156">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4d18-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4d18-157">示例</span><span class="sxs-lookup"><span data-stu-id="b4d18-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4d18-158">请求</span><span class="sxs-lookup"><span data-stu-id="b4d18-158">Request</span></span>
<span data-ttu-id="b4d18-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4d18-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4d18-160">响应</span><span class="sxs-lookup"><span data-stu-id="b4d18-160">Response</span></span>
<span data-ttu-id="b4d18-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4d18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



