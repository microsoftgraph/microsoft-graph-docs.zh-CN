---
title: 创建 mobileAppTroubleshootingEvent
description: 介绍了创建适用于 Intune 的 Microsoft Graph API 的 mobileAppTroubleshootingEvent 方法, 该方法支持多个工作流。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: d258a2d05d260a7820efcbdccc423743b9e6a4cd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899261"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="e2abb-103">创建 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e2abb-103">Create mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="e2abb-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e2abb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2abb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2abb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2abb-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2abb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2abb-107">创建新的[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2abb-107">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2abb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e2abb-108">Prerequisites</span></span>
<span data-ttu-id="e2abb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2abb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2abb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2abb-111">Permission type</span></span>|<span data-ttu-id="e2abb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e2abb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2abb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2abb-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="e2abb-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="e2abb-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="e2abb-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2abb-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e2abb-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="e2abb-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="e2abb-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2abb-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e2abb-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2abb-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2abb-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2abb-119">Not supported.</span></span>|
|<span data-ttu-id="e2abb-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2abb-120">Application</span></span>|<span data-ttu-id="e2abb-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2abb-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2abb-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2abb-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="e2abb-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2abb-123">Request headers</span></span>
|<span data-ttu-id="e2abb-124">标头</span><span class="sxs-lookup"><span data-stu-id="e2abb-124">Header</span></span>|<span data-ttu-id="e2abb-125">值</span><span class="sxs-lookup"><span data-stu-id="e2abb-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2abb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2abb-126">Authorization</span></span>|<span data-ttu-id="e2abb-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e2abb-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2abb-128">接受</span><span class="sxs-lookup"><span data-stu-id="e2abb-128">Accept</span></span>|<span data-ttu-id="e2abb-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e2abb-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2abb-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2abb-130">Request body</span></span>
<span data-ttu-id="e2abb-131">在请求正文中, 提供 mobileAppTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2abb-131">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="e2abb-132">下表显示创建 mobileAppTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e2abb-132">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="e2abb-133">属性</span><span class="sxs-lookup"><span data-stu-id="e2abb-133">Property</span></span>|<span data-ttu-id="e2abb-134">类型</span><span class="sxs-lookup"><span data-stu-id="e2abb-134">Type</span></span>|<span data-ttu-id="e2abb-135">说明</span><span class="sxs-lookup"><span data-stu-id="e2abb-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2abb-136">id</span><span class="sxs-lookup"><span data-stu-id="e2abb-136">id</span></span>|<span data-ttu-id="e2abb-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e2abb-137">String</span></span>|<span data-ttu-id="e2abb-138">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="e2abb-138">The GUID for the object</span></span>|
|<span data-ttu-id="e2abb-139">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="e2abb-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="e2abb-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="e2abb-140">additionalInformation</span></span>|<span data-ttu-id="e2abb-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2abb-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e2abb-142">一组字符串键和字符串值对, 提供有关疑难解答事件的其他信息。</span><span class="sxs-lookup"><span data-stu-id="e2abb-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="e2abb-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="e2abb-143">applicationId</span></span>|<span data-ttu-id="e2abb-144">String</span><span class="sxs-lookup"><span data-stu-id="e2abb-144">String</span></span>|<span data-ttu-id="e2abb-145">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="e2abb-145">Intune application identifier.</span></span>|
|<span data-ttu-id="e2abb-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="e2abb-146">correlationId</span></span>|<span data-ttu-id="e2abb-147">String</span><span class="sxs-lookup"><span data-stu-id="e2abb-147">String</span></span>|<span data-ttu-id="e2abb-148">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="e2abb-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="e2abb-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e2abb-149">eventDateTime</span></span>|<span data-ttu-id="e2abb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2abb-150">DateTimeOffset</span></span>|<span data-ttu-id="e2abb-151">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="e2abb-151">Time when the event occurred .</span></span> |
|<span data-ttu-id="e2abb-152">名</span><span class="sxs-lookup"><span data-stu-id="e2abb-152">eventName</span></span>|<span data-ttu-id="e2abb-153">String</span><span class="sxs-lookup"><span data-stu-id="e2abb-153">String</span></span>|<span data-ttu-id="e2abb-154">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="e2abb-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="e2abb-155">可选。</span><span class="sxs-lookup"><span data-stu-id="e2abb-155">Optional.</span></span>|
|<span data-ttu-id="e2abb-156">日志</span><span class="sxs-lookup"><span data-stu-id="e2abb-156">history</span></span>|<span data-ttu-id="e2abb-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2abb-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="e2abb-158">Intune 移动应用程序故障排除历史记录项</span><span class="sxs-lookup"><span data-stu-id="e2abb-158">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="e2abb-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e2abb-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="e2abb-160">String</span><span class="sxs-lookup"><span data-stu-id="e2abb-160">String</span></span>|<span data-ttu-id="e2abb-161">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="e2abb-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="e2abb-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e2abb-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="e2abb-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e2abb-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="e2abb-164">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="e2abb-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="e2abb-165">userId</span><span class="sxs-lookup"><span data-stu-id="e2abb-165">userId</span></span>|<span data-ttu-id="e2abb-166">String</span><span class="sxs-lookup"><span data-stu-id="e2abb-166">String</span></span>|<span data-ttu-id="e2abb-167">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="e2abb-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="e2abb-168">响应</span><span class="sxs-lookup"><span data-stu-id="e2abb-168">Response</span></span>
<span data-ttu-id="e2abb-169">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2abb-169">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2abb-170">示例</span><span class="sxs-lookup"><span data-stu-id="e2abb-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2abb-171">请求</span><span class="sxs-lookup"><span data-stu-id="e2abb-171">Request</span></span>
<span data-ttu-id="e2abb-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2abb-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="e2abb-173">响应</span><span class="sxs-lookup"><span data-stu-id="e2abb-173">Response</span></span>
<span data-ttu-id="e2abb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2abb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




