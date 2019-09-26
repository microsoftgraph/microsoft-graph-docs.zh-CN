---
title: 创建 mobileAppTroubleshootingEvent
description: 介绍了创建适用于 Intune 的 Microsoft Graph API 的 mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5708d3968b38351f26db5e1221c16fff442f93a0
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196061"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="f8960-103">创建 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="f8960-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="f8960-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f8960-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f8960-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8960-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8960-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8960-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8960-107">创建新的[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8960-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8960-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8960-108">Prerequisites</span></span>
<span data-ttu-id="f8960-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8960-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8960-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8960-111">Permission type</span></span>|<span data-ttu-id="f8960-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8960-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8960-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8960-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="f8960-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="f8960-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="f8960-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8960-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f8960-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="f8960-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="f8960-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8960-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f8960-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8960-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8960-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8960-119">Not supported.</span></span>|
|<span data-ttu-id="f8960-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8960-120">Application</span></span>||
|<span data-ttu-id="f8960-121">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="f8960-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="f8960-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8960-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f8960-123">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="f8960-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="f8960-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8960-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8960-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8960-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="f8960-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8960-126">Request headers</span></span>
|<span data-ttu-id="f8960-127">标头</span><span class="sxs-lookup"><span data-stu-id="f8960-127">Header</span></span>|<span data-ttu-id="f8960-128">值</span><span class="sxs-lookup"><span data-stu-id="f8960-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8960-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8960-129">Authorization</span></span>|<span data-ttu-id="f8960-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f8960-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8960-131">接受</span><span class="sxs-lookup"><span data-stu-id="f8960-131">Accept</span></span>|<span data-ttu-id="f8960-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f8960-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8960-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8960-133">Request body</span></span>
<span data-ttu-id="f8960-134">在请求正文中，提供 mobileAppTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8960-134">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="f8960-135">下表显示创建 mobileAppTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f8960-135">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="f8960-136">属性</span><span class="sxs-lookup"><span data-stu-id="f8960-136">Property</span></span>|<span data-ttu-id="f8960-137">类型</span><span class="sxs-lookup"><span data-stu-id="f8960-137">Type</span></span>|<span data-ttu-id="f8960-138">说明</span><span class="sxs-lookup"><span data-stu-id="f8960-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8960-139">id</span><span class="sxs-lookup"><span data-stu-id="f8960-139">id</span></span>|<span data-ttu-id="f8960-140">字符串</span><span class="sxs-lookup"><span data-stu-id="f8960-140">String</span></span>|<span data-ttu-id="f8960-141">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="f8960-141">The GUID for the object</span></span>|
|<span data-ttu-id="f8960-142">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="f8960-142">**Troubleshooting**</span></span>|
|<span data-ttu-id="f8960-143">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="f8960-143">additionalInformation</span></span>|<span data-ttu-id="f8960-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8960-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f8960-145">一组字符串键和字符串值对，提供有关疑难解答事件的其他信息。</span><span class="sxs-lookup"><span data-stu-id="f8960-145">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="f8960-146">applicationId</span><span class="sxs-lookup"><span data-stu-id="f8960-146">applicationId</span></span>|<span data-ttu-id="f8960-147">String</span><span class="sxs-lookup"><span data-stu-id="f8960-147">String</span></span>|<span data-ttu-id="f8960-148">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="f8960-148">Intune application identifier.</span></span>|
|<span data-ttu-id="f8960-149">correlationId</span><span class="sxs-lookup"><span data-stu-id="f8960-149">correlationId</span></span>|<span data-ttu-id="f8960-150">String</span><span class="sxs-lookup"><span data-stu-id="f8960-150">String</span></span>|<span data-ttu-id="f8960-151">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="f8960-151">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="f8960-152">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="f8960-152">eventDateTime</span></span>|<span data-ttu-id="f8960-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8960-153">DateTimeOffset</span></span>|<span data-ttu-id="f8960-154">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="f8960-154">Time when the event occurred .</span></span> |
|<span data-ttu-id="f8960-155">名</span><span class="sxs-lookup"><span data-stu-id="f8960-155">eventName</span></span>|<span data-ttu-id="f8960-156">String</span><span class="sxs-lookup"><span data-stu-id="f8960-156">String</span></span>|<span data-ttu-id="f8960-157">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="f8960-157">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="f8960-158">可选。</span><span class="sxs-lookup"><span data-stu-id="f8960-158">Optional.</span></span>|
|<span data-ttu-id="f8960-159">日志</span><span class="sxs-lookup"><span data-stu-id="f8960-159">history</span></span>|<span data-ttu-id="f8960-160">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="f8960-160">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="f8960-161">Intune 移动应用程序故障排除历史记录项</span><span class="sxs-lookup"><span data-stu-id="f8960-161">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="f8960-162">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f8960-162">managedDeviceIdentifier</span></span>|<span data-ttu-id="f8960-163">String</span><span class="sxs-lookup"><span data-stu-id="f8960-163">String</span></span>|<span data-ttu-id="f8960-164">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="f8960-164">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="f8960-165">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f8960-165">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="f8960-166">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f8960-166">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="f8960-167">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="f8960-167">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="f8960-168">userId</span><span class="sxs-lookup"><span data-stu-id="f8960-168">userId</span></span>|<span data-ttu-id="f8960-169">String</span><span class="sxs-lookup"><span data-stu-id="f8960-169">String</span></span>|<span data-ttu-id="f8960-170">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="f8960-170">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="f8960-171">响应</span><span class="sxs-lookup"><span data-stu-id="f8960-171">Response</span></span>
<span data-ttu-id="f8960-172">如果成功，此方法在响应`201 Created`正文中返回响应代码和[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8960-172">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8960-173">示例</span><span class="sxs-lookup"><span data-stu-id="f8960-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8960-174">请求</span><span class="sxs-lookup"><span data-stu-id="f8960-174">Request</span></span>
<span data-ttu-id="f8960-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8960-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="f8960-176">响应</span><span class="sxs-lookup"><span data-stu-id="f8960-176">Response</span></span>
<span data-ttu-id="f8960-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8960-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```








