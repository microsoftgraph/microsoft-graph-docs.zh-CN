---
title: 更新 deviceConfigurationDeviceStateSummary
description: 更新 deviceConfigurationDeviceStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 64182b6155346b509ed16ce0a2029d08e8597c1d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131657"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="22f21-103">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="22f21-103">Update deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="22f21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22f21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22f21-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22f21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22f21-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22f21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22f21-107">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="22f21-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22f21-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="22f21-108">Prerequisites</span></span>
<span data-ttu-id="22f21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22f21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22f21-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="22f21-111">Permission type</span></span>|<span data-ttu-id="22f21-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22f21-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22f21-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22f21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22f21-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22f21-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22f21-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22f21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22f21-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="22f21-116">Not supported.</span></span>|
|<span data-ttu-id="22f21-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="22f21-117">Application</span></span>|<span data-ttu-id="22f21-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22f21-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22f21-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22f21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="22f21-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="22f21-120">Request headers</span></span>
|<span data-ttu-id="22f21-121">标头</span><span class="sxs-lookup"><span data-stu-id="22f21-121">Header</span></span>|<span data-ttu-id="22f21-122">值</span><span class="sxs-lookup"><span data-stu-id="22f21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22f21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22f21-123">Authorization</span></span>|<span data-ttu-id="22f21-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="22f21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22f21-125">接受</span><span class="sxs-lookup"><span data-stu-id="22f21-125">Accept</span></span>|<span data-ttu-id="22f21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22f21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22f21-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="22f21-127">Request body</span></span>
<span data-ttu-id="22f21-128">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22f21-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="22f21-129">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="22f21-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="22f21-130">属性</span><span class="sxs-lookup"><span data-stu-id="22f21-130">Property</span></span>|<span data-ttu-id="22f21-131">类型</span><span class="sxs-lookup"><span data-stu-id="22f21-131">Type</span></span>|<span data-ttu-id="22f21-132">说明</span><span class="sxs-lookup"><span data-stu-id="22f21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22f21-133">id</span><span class="sxs-lookup"><span data-stu-id="22f21-133">id</span></span>|<span data-ttu-id="22f21-134">String</span><span class="sxs-lookup"><span data-stu-id="22f21-134">String</span></span>|<span data-ttu-id="22f21-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="22f21-135">Key of the entity.</span></span>|
|<span data-ttu-id="22f21-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22f21-136">unknownDeviceCount</span></span>|<span data-ttu-id="22f21-137">Int32</span><span class="sxs-lookup"><span data-stu-id="22f21-137">Int32</span></span>|<span data-ttu-id="22f21-138">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="22f21-138">Number of unknown devices</span></span>|
|<span data-ttu-id="22f21-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22f21-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="22f21-140">Int32</span><span class="sxs-lookup"><span data-stu-id="22f21-140">Int32</span></span>|<span data-ttu-id="22f21-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="22f21-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="22f21-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22f21-142">compliantDeviceCount</span></span>|<span data-ttu-id="22f21-143">Int32</span><span class="sxs-lookup"><span data-stu-id="22f21-143">Int32</span></span>|<span data-ttu-id="22f21-144">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="22f21-144">Number of compliant devices</span></span>|
|<span data-ttu-id="22f21-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22f21-145">remediatedDeviceCount</span></span>|<span data-ttu-id="22f21-146">Int32</span><span class="sxs-lookup"><span data-stu-id="22f21-146">Int32</span></span>|<span data-ttu-id="22f21-147">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="22f21-147">Number of remediated devices</span></span>|
|<span data-ttu-id="22f21-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22f21-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="22f21-149">Int32</span><span class="sxs-lookup"><span data-stu-id="22f21-149">Int32</span></span>|<span data-ttu-id="22f21-150">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="22f21-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="22f21-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22f21-151">errorDeviceCount</span></span>|<span data-ttu-id="22f21-152">Int32</span><span class="sxs-lookup"><span data-stu-id="22f21-152">Int32</span></span>|<span data-ttu-id="22f21-153">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="22f21-153">Number of error devices</span></span>|
|<span data-ttu-id="22f21-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22f21-154">conflictDeviceCount</span></span>|<span data-ttu-id="22f21-155">Int32</span><span class="sxs-lookup"><span data-stu-id="22f21-155">Int32</span></span>|<span data-ttu-id="22f21-156">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="22f21-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="22f21-157">响应</span><span class="sxs-lookup"><span data-stu-id="22f21-157">Response</span></span>
<span data-ttu-id="22f21-158">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22f21-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22f21-159">示例</span><span class="sxs-lookup"><span data-stu-id="22f21-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="22f21-160">请求</span><span class="sxs-lookup"><span data-stu-id="22f21-160">Request</span></span>
<span data-ttu-id="22f21-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22f21-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="22f21-162">响应</span><span class="sxs-lookup"><span data-stu-id="22f21-162">Response</span></span>
<span data-ttu-id="22f21-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22f21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




