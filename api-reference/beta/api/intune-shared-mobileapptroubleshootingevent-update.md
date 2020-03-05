---
title: 更新 mobileAppTroubleshootingEvent
description: 介绍了适用于 Intune 的 Microsoft Graph API 的更新 mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0c592bd2ac23543333601c030a3aa28dcc3d848
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458222"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="78e0f-103">更新 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="78e0f-103">Update mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="78e0f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="78e0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78e0f-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="78e0f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="78e0f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="78e0f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78e0f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78e0f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78e0f-108">更新[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="78e0f-108">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78e0f-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="78e0f-109">Prerequisites</span></span>
<span data-ttu-id="78e0f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78e0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e0f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="78e0f-112">Permission type</span></span>|<span data-ttu-id="78e0f-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="78e0f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78e0f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78e0f-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="78e0f-115">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="78e0f-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="78e0f-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e0f-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="78e0f-117">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="78e0f-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="78e0f-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e0f-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="78e0f-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78e0f-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78e0f-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="78e0f-120">Not supported.</span></span>|
|<span data-ttu-id="78e0f-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="78e0f-121">Application</span></span>||
|<span data-ttu-id="78e0f-122">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="78e0f-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="78e0f-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e0f-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="78e0f-124">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="78e0f-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="78e0f-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e0f-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="78e0f-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78e0f-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="78e0f-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="78e0f-127">Request headers</span></span>
|<span data-ttu-id="78e0f-128">标头</span><span class="sxs-lookup"><span data-stu-id="78e0f-128">Header</span></span>|<span data-ttu-id="78e0f-129">值</span><span class="sxs-lookup"><span data-stu-id="78e0f-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78e0f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="78e0f-130">Authorization</span></span>|<span data-ttu-id="78e0f-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="78e0f-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78e0f-132">接受</span><span class="sxs-lookup"><span data-stu-id="78e0f-132">Accept</span></span>|<span data-ttu-id="78e0f-133">application/json</span><span class="sxs-lookup"><span data-stu-id="78e0f-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78e0f-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="78e0f-134">Request body</span></span>
<span data-ttu-id="78e0f-135">在请求正文中，提供[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78e0f-135">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="78e0f-136">下表显示创建[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="78e0f-136">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="78e0f-137">属性</span><span class="sxs-lookup"><span data-stu-id="78e0f-137">Property</span></span>|<span data-ttu-id="78e0f-138">类型</span><span class="sxs-lookup"><span data-stu-id="78e0f-138">Type</span></span>|<span data-ttu-id="78e0f-139">说明</span><span class="sxs-lookup"><span data-stu-id="78e0f-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e0f-140">id</span><span class="sxs-lookup"><span data-stu-id="78e0f-140">id</span></span>|<span data-ttu-id="78e0f-141">字符串</span><span class="sxs-lookup"><span data-stu-id="78e0f-141">String</span></span>|<span data-ttu-id="78e0f-142">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="78e0f-142">The GUID for the object</span></span>|
|<span data-ttu-id="78e0f-143">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="78e0f-143">**Troubleshooting**</span></span>|
|<span data-ttu-id="78e0f-144">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="78e0f-144">additionalInformation</span></span>|<span data-ttu-id="78e0f-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78e0f-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="78e0f-146">一组字符串键和字符串值对，提供有关疑难解答事件的其他信息。</span><span class="sxs-lookup"><span data-stu-id="78e0f-146">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="78e0f-147">applicationId</span><span class="sxs-lookup"><span data-stu-id="78e0f-147">applicationId</span></span>|<span data-ttu-id="78e0f-148">String</span><span class="sxs-lookup"><span data-stu-id="78e0f-148">String</span></span>|<span data-ttu-id="78e0f-149">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="78e0f-149">Intune application identifier.</span></span>|
|<span data-ttu-id="78e0f-150">correlationId</span><span class="sxs-lookup"><span data-stu-id="78e0f-150">correlationId</span></span>|<span data-ttu-id="78e0f-151">String</span><span class="sxs-lookup"><span data-stu-id="78e0f-151">String</span></span>|<span data-ttu-id="78e0f-152">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="78e0f-152">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="78e0f-153">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="78e0f-153">eventDateTime</span></span>|<span data-ttu-id="78e0f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78e0f-154">DateTimeOffset</span></span>|<span data-ttu-id="78e0f-155">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="78e0f-155">Time when the event occurred.</span></span> |
|<span data-ttu-id="78e0f-156">名</span><span class="sxs-lookup"><span data-stu-id="78e0f-156">eventName</span></span>|<span data-ttu-id="78e0f-157">String</span><span class="sxs-lookup"><span data-stu-id="78e0f-157">String</span></span>|<span data-ttu-id="78e0f-158">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="78e0f-158">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="78e0f-159">可选。</span><span class="sxs-lookup"><span data-stu-id="78e0f-159">Optional.</span></span>|
|<span data-ttu-id="78e0f-160">日志</span><span class="sxs-lookup"><span data-stu-id="78e0f-160">history</span></span>|<span data-ttu-id="78e0f-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="78e0f-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="78e0f-162">Intune 移动应用程序故障排除历史记录项。</span><span class="sxs-lookup"><span data-stu-id="78e0f-162">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="78e0f-163">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="78e0f-163">managedDeviceIdentifier</span></span>|<span data-ttu-id="78e0f-164">String</span><span class="sxs-lookup"><span data-stu-id="78e0f-164">String</span></span>|<span data-ttu-id="78e0f-165">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="78e0f-165">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="78e0f-166">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="78e0f-166">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="78e0f-167">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="78e0f-167">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="78e0f-168">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="78e0f-168">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="78e0f-169">userId</span><span class="sxs-lookup"><span data-stu-id="78e0f-169">userId</span></span>|<span data-ttu-id="78e0f-170">String</span><span class="sxs-lookup"><span data-stu-id="78e0f-170">String</span></span>|<span data-ttu-id="78e0f-171">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="78e0f-171">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="78e0f-172">响应</span><span class="sxs-lookup"><span data-stu-id="78e0f-172">Response</span></span>
<span data-ttu-id="78e0f-173">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="78e0f-173">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e0f-174">示例</span><span class="sxs-lookup"><span data-stu-id="78e0f-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="78e0f-175">请求</span><span class="sxs-lookup"><span data-stu-id="78e0f-175">Request</span></span>
<span data-ttu-id="78e0f-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78e0f-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="78e0f-177">响应</span><span class="sxs-lookup"><span data-stu-id="78e0f-177">Response</span></span>
<span data-ttu-id="78e0f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="78e0f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```












