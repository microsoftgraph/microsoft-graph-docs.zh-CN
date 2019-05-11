---
title: 更新 mobileAppTroubleshootingEvent
description: 介绍了适用于 Intune 的 Microsoft Graph API 的更新 mobileAppTroubleshootingEvent 方法, 该方法支持多个工作流。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: b94a62e896bda2cf6a39b065df0fd698924a4c21
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898274"
---
# <a name="update-mobileapptroubleshootingevent"></a><span data-ttu-id="3096c-103">更新 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3096c-103">Update mobileAppTroubleshootingEvent</span></span>

> <span data-ttu-id="3096c-104">**重要说明:** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3096c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3096c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3096c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3096c-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3096c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3096c-107">更新[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3096c-107">Update the properties of a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3096c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3096c-108">Prerequisites</span></span>
<span data-ttu-id="3096c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3096c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3096c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3096c-111">Permission type</span></span>|<span data-ttu-id="3096c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3096c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3096c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3096c-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="3096c-114">&nbsp;&nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="3096c-114">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="3096c-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3096c-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3096c-116">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="3096c-116">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="3096c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3096c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3096c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3096c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3096c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="3096c-119">Not supported.</span></span>|
|<span data-ttu-id="3096c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="3096c-120">Application</span></span>|<span data-ttu-id="3096c-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="3096c-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3096c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3096c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="3096c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="3096c-123">Request headers</span></span>
|<span data-ttu-id="3096c-124">标头</span><span class="sxs-lookup"><span data-stu-id="3096c-124">Header</span></span>|<span data-ttu-id="3096c-125">值</span><span class="sxs-lookup"><span data-stu-id="3096c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3096c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="3096c-126">Authorization</span></span>|<span data-ttu-id="3096c-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3096c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3096c-128">接受</span><span class="sxs-lookup"><span data-stu-id="3096c-128">Accept</span></span>|<span data-ttu-id="3096c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3096c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3096c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3096c-130">Request body</span></span>
<span data-ttu-id="3096c-131">在请求正文中, 提供[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3096c-131">In the request body, supply a JSON representation for the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

<span data-ttu-id="3096c-132">下表显示创建[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3096c-132">The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).</span></span>

|<span data-ttu-id="3096c-133">属性</span><span class="sxs-lookup"><span data-stu-id="3096c-133">Property</span></span>|<span data-ttu-id="3096c-134">类型</span><span class="sxs-lookup"><span data-stu-id="3096c-134">Type</span></span>|<span data-ttu-id="3096c-135">说明</span><span class="sxs-lookup"><span data-stu-id="3096c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3096c-136">id</span><span class="sxs-lookup"><span data-stu-id="3096c-136">id</span></span>|<span data-ttu-id="3096c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="3096c-137">String</span></span>|<span data-ttu-id="3096c-138">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="3096c-138">The GUID for the object</span></span>|
|<span data-ttu-id="3096c-139">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="3096c-139">**Troubleshooting**</span></span>|
|<span data-ttu-id="3096c-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="3096c-140">additionalInformation</span></span>|<span data-ttu-id="3096c-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3096c-141">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="3096c-142">一组字符串键和字符串值对, 提供有关疑难解答事件的其他信息。</span><span class="sxs-lookup"><span data-stu-id="3096c-142">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="3096c-143">applicationId</span><span class="sxs-lookup"><span data-stu-id="3096c-143">applicationId</span></span>|<span data-ttu-id="3096c-144">String</span><span class="sxs-lookup"><span data-stu-id="3096c-144">String</span></span>|<span data-ttu-id="3096c-145">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="3096c-145">Intune application identifier.</span></span>|
|<span data-ttu-id="3096c-146">correlationId</span><span class="sxs-lookup"><span data-stu-id="3096c-146">correlationId</span></span>|<span data-ttu-id="3096c-147">String</span><span class="sxs-lookup"><span data-stu-id="3096c-147">String</span></span>|<span data-ttu-id="3096c-148">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="3096c-148">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="3096c-149">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="3096c-149">eventDateTime</span></span>|<span data-ttu-id="3096c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3096c-150">DateTimeOffset</span></span>|<span data-ttu-id="3096c-151">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="3096c-151">Time when the event occurred.</span></span> |
|<span data-ttu-id="3096c-152">名</span><span class="sxs-lookup"><span data-stu-id="3096c-152">eventName</span></span>|<span data-ttu-id="3096c-153">String</span><span class="sxs-lookup"><span data-stu-id="3096c-153">String</span></span>|<span data-ttu-id="3096c-154">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="3096c-154">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="3096c-155">可选。</span><span class="sxs-lookup"><span data-stu-id="3096c-155">Optional.</span></span>|
|<span data-ttu-id="3096c-156">日志</span><span class="sxs-lookup"><span data-stu-id="3096c-156">history</span></span>|<span data-ttu-id="3096c-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="3096c-157">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="3096c-158">Intune 移动应用程序故障排除历史记录项。</span><span class="sxs-lookup"><span data-stu-id="3096c-158">Intune Mobile Application Troubleshooting History Item.</span></span>|
|<span data-ttu-id="3096c-159">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3096c-159">managedDeviceIdentifier</span></span>|<span data-ttu-id="3096c-160">String</span><span class="sxs-lookup"><span data-stu-id="3096c-160">String</span></span>|<span data-ttu-id="3096c-161">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="3096c-161">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="3096c-162">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3096c-162">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="3096c-163">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3096c-163">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="3096c-164">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="3096c-164">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="3096c-165">userId</span><span class="sxs-lookup"><span data-stu-id="3096c-165">userId</span></span>|<span data-ttu-id="3096c-166">String</span><span class="sxs-lookup"><span data-stu-id="3096c-166">String</span></span>|<span data-ttu-id="3096c-167">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="3096c-167">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="3096c-168">响应</span><span class="sxs-lookup"><span data-stu-id="3096c-168">Response</span></span>
<span data-ttu-id="3096c-169">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3096c-169">If successful, this method returns a `200 OK` response code and an updated [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3096c-170">示例</span><span class="sxs-lookup"><span data-stu-id="3096c-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="3096c-171">请求</span><span class="sxs-lookup"><span data-stu-id="3096c-171">Request</span></span>
<span data-ttu-id="3096c-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3096c-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="3096c-173">响应</span><span class="sxs-lookup"><span data-stu-id="3096c-173">Response</span></span>
<span data-ttu-id="3096c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3096c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




