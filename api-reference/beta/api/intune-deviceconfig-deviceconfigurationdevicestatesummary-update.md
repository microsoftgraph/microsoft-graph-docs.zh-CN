---
title: 更新 deviceConfigurationDeviceStateSummary
description: 更新 deviceConfigurationDeviceStateSummary 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6afdd4559e21453dc615f4adfd736b98977746d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42449164"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="f2bc4-103">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="f2bc4-103">Update deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="f2bc4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f2bc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2bc4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2bc4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2bc4-107">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2bc4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2bc4-108">Prerequisites</span></span>
<span data-ttu-id="f2bc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2bc4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2bc4-111">Permission type</span></span>|<span data-ttu-id="f2bc4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2bc4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2bc4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2bc4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2bc4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2bc4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2bc4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2bc4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2bc4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-116">Not supported.</span></span>|
|<span data-ttu-id="f2bc4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2bc4-117">Application</span></span>|<span data-ttu-id="f2bc4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2bc4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2bc4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2bc4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="f2bc4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2bc4-120">Request headers</span></span>
|<span data-ttu-id="f2bc4-121">标头</span><span class="sxs-lookup"><span data-stu-id="f2bc4-121">Header</span></span>|<span data-ttu-id="f2bc4-122">值</span><span class="sxs-lookup"><span data-stu-id="f2bc4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2bc4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2bc4-123">Authorization</span></span>|<span data-ttu-id="f2bc4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2bc4-125">接受</span><span class="sxs-lookup"><span data-stu-id="f2bc4-125">Accept</span></span>|<span data-ttu-id="f2bc4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2bc4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2bc4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2bc4-127">Request body</span></span>
<span data-ttu-id="f2bc4-128">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="f2bc4-129">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="f2bc4-130">属性</span><span class="sxs-lookup"><span data-stu-id="f2bc4-130">Property</span></span>|<span data-ttu-id="f2bc4-131">类型</span><span class="sxs-lookup"><span data-stu-id="f2bc4-131">Type</span></span>|<span data-ttu-id="f2bc4-132">说明</span><span class="sxs-lookup"><span data-stu-id="f2bc4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2bc4-133">id</span><span class="sxs-lookup"><span data-stu-id="f2bc4-133">id</span></span>|<span data-ttu-id="f2bc4-134">String</span><span class="sxs-lookup"><span data-stu-id="f2bc4-134">String</span></span>|<span data-ttu-id="f2bc4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-135">Key of the entity.</span></span>|
|<span data-ttu-id="f2bc4-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2bc4-136">unknownDeviceCount</span></span>|<span data-ttu-id="f2bc4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f2bc4-137">Int32</span></span>|<span data-ttu-id="f2bc4-138">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="f2bc4-138">Number of unknown devices</span></span>|
|<span data-ttu-id="f2bc4-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2bc4-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="f2bc4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f2bc4-140">Int32</span></span>|<span data-ttu-id="f2bc4-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="f2bc4-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="f2bc4-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2bc4-142">compliantDeviceCount</span></span>|<span data-ttu-id="f2bc4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f2bc4-143">Int32</span></span>|<span data-ttu-id="f2bc4-144">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f2bc4-144">Number of compliant devices</span></span>|
|<span data-ttu-id="f2bc4-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2bc4-145">remediatedDeviceCount</span></span>|<span data-ttu-id="f2bc4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f2bc4-146">Int32</span></span>|<span data-ttu-id="f2bc4-147">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="f2bc4-147">Number of remediated devices</span></span>|
|<span data-ttu-id="f2bc4-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2bc4-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="f2bc4-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f2bc4-149">Int32</span></span>|<span data-ttu-id="f2bc4-150">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="f2bc4-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="f2bc4-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2bc4-151">errorDeviceCount</span></span>|<span data-ttu-id="f2bc4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f2bc4-152">Int32</span></span>|<span data-ttu-id="f2bc4-153">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="f2bc4-153">Number of error devices</span></span>|
|<span data-ttu-id="f2bc4-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2bc4-154">conflictDeviceCount</span></span>|<span data-ttu-id="f2bc4-155">Int32</span><span class="sxs-lookup"><span data-stu-id="f2bc4-155">Int32</span></span>|<span data-ttu-id="f2bc4-156">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="f2bc4-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="f2bc4-157">响应</span><span class="sxs-lookup"><span data-stu-id="f2bc4-157">Response</span></span>
<span data-ttu-id="f2bc4-158">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2bc4-159">示例</span><span class="sxs-lookup"><span data-stu-id="f2bc4-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2bc4-160">请求</span><span class="sxs-lookup"><span data-stu-id="f2bc4-160">Request</span></span>
<span data-ttu-id="f2bc4-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
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

### <a name="response"></a><span data-ttu-id="f2bc4-162">响应</span><span class="sxs-lookup"><span data-stu-id="f2bc4-162">Response</span></span>
<span data-ttu-id="f2bc4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2bc4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





