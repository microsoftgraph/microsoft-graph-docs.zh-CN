---
title: 更新 deviceConfigurationDeviceStateSummary
description: 更新 deviceConfigurationDeviceStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f7077e76e6bfc0c0652291a491eab4e1aee0d97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32469395"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="be48f-103">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="be48f-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="be48f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="be48f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be48f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be48f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be48f-106">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="be48f-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be48f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="be48f-107">Prerequisites</span></span>
<span data-ttu-id="be48f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be48f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be48f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="be48f-110">Permission type</span></span>|<span data-ttu-id="be48f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="be48f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be48f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be48f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be48f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be48f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be48f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be48f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be48f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="be48f-115">Not supported.</span></span>|
|<span data-ttu-id="be48f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="be48f-116">Application</span></span>|<span data-ttu-id="be48f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="be48f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be48f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be48f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="be48f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="be48f-119">Request headers</span></span>
|<span data-ttu-id="be48f-120">标头</span><span class="sxs-lookup"><span data-stu-id="be48f-120">Header</span></span>|<span data-ttu-id="be48f-121">值</span><span class="sxs-lookup"><span data-stu-id="be48f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be48f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be48f-122">Authorization</span></span>|<span data-ttu-id="be48f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="be48f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be48f-124">接受</span><span class="sxs-lookup"><span data-stu-id="be48f-124">Accept</span></span>|<span data-ttu-id="be48f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be48f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be48f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="be48f-126">Request body</span></span>
<span data-ttu-id="be48f-127">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be48f-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="be48f-128">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be48f-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="be48f-129">属性</span><span class="sxs-lookup"><span data-stu-id="be48f-129">Property</span></span>|<span data-ttu-id="be48f-130">类型</span><span class="sxs-lookup"><span data-stu-id="be48f-130">Type</span></span>|<span data-ttu-id="be48f-131">说明</span><span class="sxs-lookup"><span data-stu-id="be48f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be48f-132">id</span><span class="sxs-lookup"><span data-stu-id="be48f-132">id</span></span>|<span data-ttu-id="be48f-133">String</span><span class="sxs-lookup"><span data-stu-id="be48f-133">String</span></span>|<span data-ttu-id="be48f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="be48f-134">Key of the entity.</span></span>|
|<span data-ttu-id="be48f-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="be48f-135">unknownDeviceCount</span></span>|<span data-ttu-id="be48f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="be48f-136">Int32</span></span>|<span data-ttu-id="be48f-137">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="be48f-137">Number of unknown devices</span></span>|
|<span data-ttu-id="be48f-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="be48f-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="be48f-139">Int32</span><span class="sxs-lookup"><span data-stu-id="be48f-139">Int32</span></span>|<span data-ttu-id="be48f-140">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="be48f-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="be48f-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="be48f-141">compliantDeviceCount</span></span>|<span data-ttu-id="be48f-142">Int32</span><span class="sxs-lookup"><span data-stu-id="be48f-142">Int32</span></span>|<span data-ttu-id="be48f-143">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="be48f-143">Number of compliant devices</span></span>|
|<span data-ttu-id="be48f-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="be48f-144">remediatedDeviceCount</span></span>|<span data-ttu-id="be48f-145">Int32</span><span class="sxs-lookup"><span data-stu-id="be48f-145">Int32</span></span>|<span data-ttu-id="be48f-146">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="be48f-146">Number of remediated devices</span></span>|
|<span data-ttu-id="be48f-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="be48f-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="be48f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="be48f-148">Int32</span></span>|<span data-ttu-id="be48f-149">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="be48f-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="be48f-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="be48f-150">errorDeviceCount</span></span>|<span data-ttu-id="be48f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="be48f-151">Int32</span></span>|<span data-ttu-id="be48f-152">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="be48f-152">Number of error devices</span></span>|
|<span data-ttu-id="be48f-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="be48f-153">conflictDeviceCount</span></span>|<span data-ttu-id="be48f-154">Int32</span><span class="sxs-lookup"><span data-stu-id="be48f-154">Int32</span></span>|<span data-ttu-id="be48f-155">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="be48f-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="be48f-156">响应</span><span class="sxs-lookup"><span data-stu-id="be48f-156">Response</span></span>
<span data-ttu-id="be48f-157">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be48f-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be48f-158">示例</span><span class="sxs-lookup"><span data-stu-id="be48f-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="be48f-159">请求</span><span class="sxs-lookup"><span data-stu-id="be48f-159">Request</span></span>
<span data-ttu-id="be48f-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be48f-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be48f-161">响应</span><span class="sxs-lookup"><span data-stu-id="be48f-161">Response</span></span>
<span data-ttu-id="be48f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be48f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





