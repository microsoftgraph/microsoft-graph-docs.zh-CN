---
title: 创建 mobileAppTroubleshootingEvent
description: 介绍了创建适用于 Intune 的 Microsoft Graph API 的 mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56fed3deec707ef7627d73fcc8f8e20937593a07
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939667"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="32e26-103">创建 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="32e26-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="32e26-104">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="32e26-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="32e26-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="32e26-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32e26-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32e26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32e26-107">创建新的[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="32e26-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32e26-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="32e26-108">Prerequisites</span></span>
<span data-ttu-id="32e26-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32e26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32e26-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="32e26-111">Permission type</span></span>|<span data-ttu-id="32e26-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32e26-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32e26-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32e26-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="32e26-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="32e26-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="32e26-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32e26-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="32e26-116">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="32e26-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="32e26-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32e26-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="32e26-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32e26-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32e26-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="32e26-119">Not supported.</span></span>|
|<span data-ttu-id="32e26-120">Application</span><span class="sxs-lookup"><span data-stu-id="32e26-120">Application</span></span>||
|<span data-ttu-id="32e26-121">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="32e26-121">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="32e26-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32e26-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="32e26-123">&nbsp; &nbsp; **故障排除**</span><span class="sxs-lookup"><span data-stu-id="32e26-123">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="32e26-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32e26-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32e26-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32e26-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="32e26-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="32e26-126">Request headers</span></span>
|<span data-ttu-id="32e26-127">标头</span><span class="sxs-lookup"><span data-stu-id="32e26-127">Header</span></span>|<span data-ttu-id="32e26-128">值</span><span class="sxs-lookup"><span data-stu-id="32e26-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32e26-129">授权</span><span class="sxs-lookup"><span data-stu-id="32e26-129">Authorization</span></span>|<span data-ttu-id="32e26-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="32e26-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32e26-131">接受</span><span class="sxs-lookup"><span data-stu-id="32e26-131">Accept</span></span>|<span data-ttu-id="32e26-132">application/json</span><span class="sxs-lookup"><span data-stu-id="32e26-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32e26-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="32e26-133">Request body</span></span>
<span data-ttu-id="32e26-134">在请求正文中，提供 mobileAppTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32e26-134">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="32e26-135">下表显示创建 mobileAppTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="32e26-135">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="32e26-136">属性</span><span class="sxs-lookup"><span data-stu-id="32e26-136">Property</span></span>|<span data-ttu-id="32e26-137">类型</span><span class="sxs-lookup"><span data-stu-id="32e26-137">Type</span></span>|<span data-ttu-id="32e26-138">说明</span><span class="sxs-lookup"><span data-stu-id="32e26-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32e26-139">id</span><span class="sxs-lookup"><span data-stu-id="32e26-139">id</span></span>|<span data-ttu-id="32e26-140">字符串</span><span class="sxs-lookup"><span data-stu-id="32e26-140">String</span></span>|<span data-ttu-id="32e26-141">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="32e26-141">The GUID for the object</span></span>|
|<span data-ttu-id="32e26-142">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="32e26-142">**Troubleshooting**</span></span>|
|<span data-ttu-id="32e26-143">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="32e26-143">additionalInformation</span></span>|<span data-ttu-id="32e26-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32e26-144">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="32e26-145">一组字符串键和字符串值对，提供有关疑难解答事件的其他信息。</span><span class="sxs-lookup"><span data-stu-id="32e26-145">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="32e26-146">applicationId</span><span class="sxs-lookup"><span data-stu-id="32e26-146">applicationId</span></span>|<span data-ttu-id="32e26-147">字符串</span><span class="sxs-lookup"><span data-stu-id="32e26-147">String</span></span>|<span data-ttu-id="32e26-148">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="32e26-148">Intune application identifier.</span></span>|
|<span data-ttu-id="32e26-149">correlationId</span><span class="sxs-lookup"><span data-stu-id="32e26-149">correlationId</span></span>|<span data-ttu-id="32e26-150">字符串</span><span class="sxs-lookup"><span data-stu-id="32e26-150">String</span></span>|<span data-ttu-id="32e26-151">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="32e26-151">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="32e26-152">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="32e26-152">eventDateTime</span></span>|<span data-ttu-id="32e26-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32e26-153">DateTimeOffset</span></span>|<span data-ttu-id="32e26-154">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="32e26-154">Time when the event occurred .</span></span> |
|<span data-ttu-id="32e26-155">名</span><span class="sxs-lookup"><span data-stu-id="32e26-155">eventName</span></span>|<span data-ttu-id="32e26-156">字符串</span><span class="sxs-lookup"><span data-stu-id="32e26-156">String</span></span>|<span data-ttu-id="32e26-157">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="32e26-157">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="32e26-158">可选。</span><span class="sxs-lookup"><span data-stu-id="32e26-158">Optional.</span></span>|
|<span data-ttu-id="32e26-159">日志</span><span class="sxs-lookup"><span data-stu-id="32e26-159">history</span></span>|<span data-ttu-id="32e26-160">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="32e26-160">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="32e26-161">Intune 移动应用程序故障排除历史记录项</span><span class="sxs-lookup"><span data-stu-id="32e26-161">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="32e26-162">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="32e26-162">managedDeviceIdentifier</span></span>|<span data-ttu-id="32e26-163">String</span><span class="sxs-lookup"><span data-stu-id="32e26-163">String</span></span>|<span data-ttu-id="32e26-164">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="32e26-164">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="32e26-165">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="32e26-165">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="32e26-166">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="32e26-166">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="32e26-167">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="32e26-167">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="32e26-168">userId</span><span class="sxs-lookup"><span data-stu-id="32e26-168">userId</span></span>|<span data-ttu-id="32e26-169">String</span><span class="sxs-lookup"><span data-stu-id="32e26-169">String</span></span>|<span data-ttu-id="32e26-170">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="32e26-170">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="32e26-171">响应</span><span class="sxs-lookup"><span data-stu-id="32e26-171">Response</span></span>
<span data-ttu-id="32e26-172">如果成功，此方法在响应`201 Created`正文中返回响应代码和[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="32e26-172">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32e26-173">示例</span><span class="sxs-lookup"><span data-stu-id="32e26-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="32e26-174">请求</span><span class="sxs-lookup"><span data-stu-id="32e26-174">Request</span></span>
<span data-ttu-id="32e26-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32e26-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="32e26-176">响应</span><span class="sxs-lookup"><span data-stu-id="32e26-176">Response</span></span>
<span data-ttu-id="32e26-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32e26-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```












