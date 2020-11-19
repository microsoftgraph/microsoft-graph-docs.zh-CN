---
title: 更新 deviceConfigurationDeviceStateSummary
description: 更新 deviceConfigurationDeviceStateSummary 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a618ff77525957148d62f7bcfdbd2e154faf028b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49213544"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="85627-103">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="85627-103">Update deviceConfigurationDeviceStateSummary</span></span>

<span data-ttu-id="85627-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85627-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85627-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85627-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85627-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85627-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85627-107">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="85627-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85627-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="85627-108">Prerequisites</span></span>
<span data-ttu-id="85627-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85627-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="85627-111">Permission type</span></span>|<span data-ttu-id="85627-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85627-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85627-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85627-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85627-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85627-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85627-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85627-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85627-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="85627-116">Not supported.</span></span>|
|<span data-ttu-id="85627-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="85627-117">Application</span></span>|<span data-ttu-id="85627-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85627-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85627-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85627-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="85627-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="85627-120">Request headers</span></span>
|<span data-ttu-id="85627-121">标头</span><span class="sxs-lookup"><span data-stu-id="85627-121">Header</span></span>|<span data-ttu-id="85627-122">值</span><span class="sxs-lookup"><span data-stu-id="85627-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85627-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85627-123">Authorization</span></span>|<span data-ttu-id="85627-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85627-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85627-125">接受</span><span class="sxs-lookup"><span data-stu-id="85627-125">Accept</span></span>|<span data-ttu-id="85627-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85627-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85627-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="85627-127">Request body</span></span>
<span data-ttu-id="85627-128">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85627-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="85627-129">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="85627-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="85627-130">属性</span><span class="sxs-lookup"><span data-stu-id="85627-130">Property</span></span>|<span data-ttu-id="85627-131">类型</span><span class="sxs-lookup"><span data-stu-id="85627-131">Type</span></span>|<span data-ttu-id="85627-132">说明</span><span class="sxs-lookup"><span data-stu-id="85627-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85627-133">id</span><span class="sxs-lookup"><span data-stu-id="85627-133">id</span></span>|<span data-ttu-id="85627-134">String</span><span class="sxs-lookup"><span data-stu-id="85627-134">String</span></span>|<span data-ttu-id="85627-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="85627-135">Key of the entity.</span></span>|
|<span data-ttu-id="85627-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85627-136">unknownDeviceCount</span></span>|<span data-ttu-id="85627-137">Int32</span><span class="sxs-lookup"><span data-stu-id="85627-137">Int32</span></span>|<span data-ttu-id="85627-138">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="85627-138">Number of unknown devices</span></span>|
|<span data-ttu-id="85627-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85627-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="85627-140">Int32</span><span class="sxs-lookup"><span data-stu-id="85627-140">Int32</span></span>|<span data-ttu-id="85627-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="85627-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="85627-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85627-142">compliantDeviceCount</span></span>|<span data-ttu-id="85627-143">Int32</span><span class="sxs-lookup"><span data-stu-id="85627-143">Int32</span></span>|<span data-ttu-id="85627-144">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="85627-144">Number of compliant devices</span></span>|
|<span data-ttu-id="85627-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85627-145">remediatedDeviceCount</span></span>|<span data-ttu-id="85627-146">Int32</span><span class="sxs-lookup"><span data-stu-id="85627-146">Int32</span></span>|<span data-ttu-id="85627-147">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="85627-147">Number of remediated devices</span></span>|
|<span data-ttu-id="85627-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85627-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="85627-149">Int32</span><span class="sxs-lookup"><span data-stu-id="85627-149">Int32</span></span>|<span data-ttu-id="85627-150">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="85627-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="85627-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85627-151">errorDeviceCount</span></span>|<span data-ttu-id="85627-152">Int32</span><span class="sxs-lookup"><span data-stu-id="85627-152">Int32</span></span>|<span data-ttu-id="85627-153">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="85627-153">Number of error devices</span></span>|
|<span data-ttu-id="85627-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="85627-154">conflictDeviceCount</span></span>|<span data-ttu-id="85627-155">Int32</span><span class="sxs-lookup"><span data-stu-id="85627-155">Int32</span></span>|<span data-ttu-id="85627-156">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="85627-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="85627-157">响应</span><span class="sxs-lookup"><span data-stu-id="85627-157">Response</span></span>
<span data-ttu-id="85627-158">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85627-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85627-159">示例</span><span class="sxs-lookup"><span data-stu-id="85627-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="85627-160">请求</span><span class="sxs-lookup"><span data-stu-id="85627-160">Request</span></span>
<span data-ttu-id="85627-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85627-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85627-162">响应</span><span class="sxs-lookup"><span data-stu-id="85627-162">Response</span></span>
<span data-ttu-id="85627-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85627-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




