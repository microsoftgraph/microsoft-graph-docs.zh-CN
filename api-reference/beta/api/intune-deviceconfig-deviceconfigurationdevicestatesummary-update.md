---
title: 更新 deviceConfigurationDeviceStateSummary
description: 更新 deviceConfigurationDeviceStateSummary 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1963e00e5f2cf6719932b1b26b388a72fff0fb28
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832527"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="02900-103">更新 deviceConfigurationDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="02900-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="02900-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="02900-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02900-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="02900-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02900-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="02900-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02900-107">更新 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="02900-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02900-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="02900-108">Prerequisites</span></span>
<span data-ttu-id="02900-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="02900-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02900-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="02900-111">Permission type</span></span>|<span data-ttu-id="02900-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="02900-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02900-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02900-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02900-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02900-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02900-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02900-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02900-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="02900-116">Not supported.</span></span>|
|<span data-ttu-id="02900-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="02900-117">Application</span></span>|<span data-ttu-id="02900-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="02900-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02900-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02900-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="02900-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="02900-120">Request headers</span></span>
|<span data-ttu-id="02900-121">标头</span><span class="sxs-lookup"><span data-stu-id="02900-121">Header</span></span>|<span data-ttu-id="02900-122">值</span><span class="sxs-lookup"><span data-stu-id="02900-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02900-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02900-123">Authorization</span></span>|<span data-ttu-id="02900-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="02900-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02900-125">Accept</span><span class="sxs-lookup"><span data-stu-id="02900-125">Accept</span></span>|<span data-ttu-id="02900-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02900-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02900-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="02900-127">Request body</span></span>
<span data-ttu-id="02900-128">在请求正文中，提供 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02900-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="02900-129">下表显示创建 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="02900-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="02900-130">属性</span><span class="sxs-lookup"><span data-stu-id="02900-130">Property</span></span>|<span data-ttu-id="02900-131">类型</span><span class="sxs-lookup"><span data-stu-id="02900-131">Type</span></span>|<span data-ttu-id="02900-132">说明</span><span class="sxs-lookup"><span data-stu-id="02900-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02900-133">id</span><span class="sxs-lookup"><span data-stu-id="02900-133">id</span></span>|<span data-ttu-id="02900-134">String</span><span class="sxs-lookup"><span data-stu-id="02900-134">String</span></span>|<span data-ttu-id="02900-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="02900-135">Key of the entity.</span></span>|
|<span data-ttu-id="02900-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02900-136">unknownDeviceCount</span></span>|<span data-ttu-id="02900-137">Int32</span><span class="sxs-lookup"><span data-stu-id="02900-137">Int32</span></span>|<span data-ttu-id="02900-138">未知设备的数量</span><span class="sxs-lookup"><span data-stu-id="02900-138">Number of unknown devices</span></span>|
|<span data-ttu-id="02900-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02900-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="02900-140">Int32</span><span class="sxs-lookup"><span data-stu-id="02900-140">Int32</span></span>|<span data-ttu-id="02900-141">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="02900-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="02900-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02900-142">compliantDeviceCount</span></span>|<span data-ttu-id="02900-143">Int32</span><span class="sxs-lookup"><span data-stu-id="02900-143">Int32</span></span>|<span data-ttu-id="02900-144">兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="02900-144">Number of compliant devices</span></span>|
|<span data-ttu-id="02900-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02900-145">remediatedDeviceCount</span></span>|<span data-ttu-id="02900-146">Int32</span><span class="sxs-lookup"><span data-stu-id="02900-146">Int32</span></span>|<span data-ttu-id="02900-147">已修复设备的数量</span><span class="sxs-lookup"><span data-stu-id="02900-147">Number of remediated devices</span></span>|
|<span data-ttu-id="02900-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02900-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="02900-149">Int32</span><span class="sxs-lookup"><span data-stu-id="02900-149">Int32</span></span>|<span data-ttu-id="02900-150">不兼容设备的数量</span><span class="sxs-lookup"><span data-stu-id="02900-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="02900-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02900-151">errorDeviceCount</span></span>|<span data-ttu-id="02900-152">Int32</span><span class="sxs-lookup"><span data-stu-id="02900-152">Int32</span></span>|<span data-ttu-id="02900-153">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="02900-153">Number of error devices</span></span>|
|<span data-ttu-id="02900-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="02900-154">conflictDeviceCount</span></span>|<span data-ttu-id="02900-155">Int32</span><span class="sxs-lookup"><span data-stu-id="02900-155">Int32</span></span>|<span data-ttu-id="02900-156">冲突设备的数量</span><span class="sxs-lookup"><span data-stu-id="02900-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="02900-157">响应</span><span class="sxs-lookup"><span data-stu-id="02900-157">Response</span></span>
<span data-ttu-id="02900-158">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="02900-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02900-159">示例</span><span class="sxs-lookup"><span data-stu-id="02900-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="02900-160">请求</span><span class="sxs-lookup"><span data-stu-id="02900-160">Request</span></span>
<span data-ttu-id="02900-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02900-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="02900-162">响应</span><span class="sxs-lookup"><span data-stu-id="02900-162">Response</span></span>
<span data-ttu-id="02900-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02900-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





