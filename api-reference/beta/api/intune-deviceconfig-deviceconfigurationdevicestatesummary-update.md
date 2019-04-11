---
title: 更新 deviceConfigurationDeviceStateSummary
description: 更新 deviceConfigurationDeviceStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f7077e76e6bfc0c0652291a491eab4e1aee0d97
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806816"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="df0cd-103">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="df0cd-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="df0cd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df0cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df0cd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df0cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df0cd-106">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="df0cd-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df0cd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="df0cd-107">Prerequisites</span></span>
<span data-ttu-id="df0cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df0cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df0cd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="df0cd-110">Permission type</span></span>|<span data-ttu-id="df0cd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df0cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df0cd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df0cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df0cd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df0cd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df0cd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df0cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df0cd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="df0cd-115">Not supported.</span></span>|
|<span data-ttu-id="df0cd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="df0cd-116">Application</span></span>|<span data-ttu-id="df0cd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="df0cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df0cd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df0cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="df0cd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="df0cd-119">Request headers</span></span>
|<span data-ttu-id="df0cd-120">标头</span><span class="sxs-lookup"><span data-stu-id="df0cd-120">Header</span></span>|<span data-ttu-id="df0cd-121">值</span><span class="sxs-lookup"><span data-stu-id="df0cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df0cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df0cd-122">Authorization</span></span>|<span data-ttu-id="df0cd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df0cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df0cd-124">接受</span><span class="sxs-lookup"><span data-stu-id="df0cd-124">Accept</span></span>|<span data-ttu-id="df0cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df0cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df0cd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="df0cd-126">Request body</span></span>
<span data-ttu-id="df0cd-127">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df0cd-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="df0cd-128">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df0cd-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="df0cd-129">属性</span><span class="sxs-lookup"><span data-stu-id="df0cd-129">Property</span></span>|<span data-ttu-id="df0cd-130">类型</span><span class="sxs-lookup"><span data-stu-id="df0cd-130">Type</span></span>|<span data-ttu-id="df0cd-131">说明</span><span class="sxs-lookup"><span data-stu-id="df0cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df0cd-132">id</span><span class="sxs-lookup"><span data-stu-id="df0cd-132">id</span></span>|<span data-ttu-id="df0cd-133">String</span><span class="sxs-lookup"><span data-stu-id="df0cd-133">String</span></span>|<span data-ttu-id="df0cd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="df0cd-134">Key of the entity.</span></span>|
|<span data-ttu-id="df0cd-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df0cd-135">unknownDeviceCount</span></span>|<span data-ttu-id="df0cd-136">Int32</span><span class="sxs-lookup"><span data-stu-id="df0cd-136">Int32</span></span>|<span data-ttu-id="df0cd-137">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="df0cd-137">Number of unknown devices</span></span>|
|<span data-ttu-id="df0cd-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df0cd-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="df0cd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="df0cd-139">Int32</span></span>|<span data-ttu-id="df0cd-140">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="df0cd-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="df0cd-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df0cd-141">compliantDeviceCount</span></span>|<span data-ttu-id="df0cd-142">Int32</span><span class="sxs-lookup"><span data-stu-id="df0cd-142">Int32</span></span>|<span data-ttu-id="df0cd-143">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="df0cd-143">Number of compliant devices</span></span>|
|<span data-ttu-id="df0cd-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df0cd-144">remediatedDeviceCount</span></span>|<span data-ttu-id="df0cd-145">Int32</span><span class="sxs-lookup"><span data-stu-id="df0cd-145">Int32</span></span>|<span data-ttu-id="df0cd-146">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="df0cd-146">Number of remediated devices</span></span>|
|<span data-ttu-id="df0cd-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df0cd-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="df0cd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="df0cd-148">Int32</span></span>|<span data-ttu-id="df0cd-149">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="df0cd-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="df0cd-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df0cd-150">errorDeviceCount</span></span>|<span data-ttu-id="df0cd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="df0cd-151">Int32</span></span>|<span data-ttu-id="df0cd-152">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="df0cd-152">Number of error devices</span></span>|
|<span data-ttu-id="df0cd-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="df0cd-153">conflictDeviceCount</span></span>|<span data-ttu-id="df0cd-154">Int32</span><span class="sxs-lookup"><span data-stu-id="df0cd-154">Int32</span></span>|<span data-ttu-id="df0cd-155">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="df0cd-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="df0cd-156">响应</span><span class="sxs-lookup"><span data-stu-id="df0cd-156">Response</span></span>
<span data-ttu-id="df0cd-157">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df0cd-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df0cd-158">示例</span><span class="sxs-lookup"><span data-stu-id="df0cd-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="df0cd-159">请求</span><span class="sxs-lookup"><span data-stu-id="df0cd-159">Request</span></span>
<span data-ttu-id="df0cd-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df0cd-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df0cd-161">响应</span><span class="sxs-lookup"><span data-stu-id="df0cd-161">Response</span></span>
<span data-ttu-id="df0cd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df0cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





