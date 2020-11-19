---
title: 创建 mobileAppTroubleshootingEvent
description: 介绍了创建适用于 Intune 的 Microsoft Graph API 的 mobileAppTroubleshootingEvent 方法，该方法支持多个工作流。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ba86467fc6b968fef5eadde48886b227772d352
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217506"
---
# <a name="create-mobileapptroubleshootingevent"></a><span data-ttu-id="0c3ef-103">创建 mobileAppTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="0c3ef-103">Create mobileAppTroubleshootingEvent</span></span>

<span data-ttu-id="0c3ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c3ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c3ef-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c3ef-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c3ef-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c3ef-108">创建新的 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-108">Create a new [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c3ef-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="0c3ef-109">Prerequisites</span></span>
<span data-ttu-id="0c3ef-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c3ef-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c3ef-112">Permission type</span></span>|<span data-ttu-id="0c3ef-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0c3ef-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c3ef-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c3ef-114">Delegated (work or school account)</span></span>||
|<span data-ttu-id="0c3ef-115">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="0c3ef-115">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="0c3ef-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3ef-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0c3ef-117">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="0c3ef-117">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="0c3ef-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3ef-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0c3ef-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c3ef-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c3ef-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-120">Not supported.</span></span>|
|<span data-ttu-id="0c3ef-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c3ef-121">Application</span></span>||
|<span data-ttu-id="0c3ef-122">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="0c3ef-122">&nbsp; &nbsp; **Device management**</span></span>|<span data-ttu-id="0c3ef-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3ef-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0c3ef-124">&nbsp; &nbsp; **疑难解答**</span><span class="sxs-lookup"><span data-stu-id="0c3ef-124">&nbsp; &nbsp; **Troubleshooting**</span></span>|<span data-ttu-id="0c3ef-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3ef-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c3ef-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c3ef-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="0c3ef-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c3ef-127">Request headers</span></span>
|<span data-ttu-id="0c3ef-128">标头</span><span class="sxs-lookup"><span data-stu-id="0c3ef-128">Header</span></span>|<span data-ttu-id="0c3ef-129">值</span><span class="sxs-lookup"><span data-stu-id="0c3ef-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c3ef-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c3ef-130">Authorization</span></span>|<span data-ttu-id="0c3ef-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c3ef-132">接受</span><span class="sxs-lookup"><span data-stu-id="0c3ef-132">Accept</span></span>|<span data-ttu-id="0c3ef-133">application/json</span><span class="sxs-lookup"><span data-stu-id="0c3ef-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c3ef-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c3ef-134">Request body</span></span>
<span data-ttu-id="0c3ef-135">在请求正文中，提供 mobileAppTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-135">In the request body, supply a JSON representation for the mobileAppTroubleshootingEvent object.</span></span>

<span data-ttu-id="0c3ef-136">下表显示创建 mobileAppTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-136">The following table shows the properties that are required when you create the mobileAppTroubleshootingEvent.</span></span>

|<span data-ttu-id="0c3ef-137">属性</span><span class="sxs-lookup"><span data-stu-id="0c3ef-137">Property</span></span>|<span data-ttu-id="0c3ef-138">类型</span><span class="sxs-lookup"><span data-stu-id="0c3ef-138">Type</span></span>|<span data-ttu-id="0c3ef-139">说明</span><span class="sxs-lookup"><span data-stu-id="0c3ef-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c3ef-140">id</span><span class="sxs-lookup"><span data-stu-id="0c3ef-140">id</span></span>|<span data-ttu-id="0c3ef-141">String</span><span class="sxs-lookup"><span data-stu-id="0c3ef-141">String</span></span>|<span data-ttu-id="0c3ef-142">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="0c3ef-142">The GUID for the object</span></span>|
|<span data-ttu-id="0c3ef-143">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="0c3ef-143">**Troubleshooting**</span></span>|
|<span data-ttu-id="0c3ef-144">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="0c3ef-144">additionalInformation</span></span>|<span data-ttu-id="0c3ef-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c3ef-145">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0c3ef-146">一组字符串键和字符串值对，提供有关疑难解答事件的其他信息。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-146">A set of string key and string value pairs which provides additional information on the Troubleshooting event.</span></span>|
|<span data-ttu-id="0c3ef-147">applicationId</span><span class="sxs-lookup"><span data-stu-id="0c3ef-147">applicationId</span></span>|<span data-ttu-id="0c3ef-148">String</span><span class="sxs-lookup"><span data-stu-id="0c3ef-148">String</span></span>|<span data-ttu-id="0c3ef-149">Intune 应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-149">Intune application identifier.</span></span>|
|<span data-ttu-id="0c3ef-150">correlationId</span><span class="sxs-lookup"><span data-stu-id="0c3ef-150">correlationId</span></span>|<span data-ttu-id="0c3ef-151">String</span><span class="sxs-lookup"><span data-stu-id="0c3ef-151">String</span></span>|<span data-ttu-id="0c3ef-152">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-152">ID used for tracing the failure in the service.</span></span> |
|<span data-ttu-id="0c3ef-153">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="0c3ef-153">eventDateTime</span></span>|<span data-ttu-id="0c3ef-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c3ef-154">DateTimeOffset</span></span>|<span data-ttu-id="0c3ef-155">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-155">Time when the event occurred .</span></span> |
|<span data-ttu-id="0c3ef-156">名</span><span class="sxs-lookup"><span data-stu-id="0c3ef-156">eventName</span></span>|<span data-ttu-id="0c3ef-157">String</span><span class="sxs-lookup"><span data-stu-id="0c3ef-157">String</span></span>|<span data-ttu-id="0c3ef-158">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-158">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="0c3ef-159">可选。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-159">Optional.</span></span>|
|<span data-ttu-id="0c3ef-160">日志</span><span class="sxs-lookup"><span data-stu-id="0c3ef-160">history</span></span>|<span data-ttu-id="0c3ef-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0c3ef-161">[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md) collection</span></span>|<span data-ttu-id="0c3ef-162">Intune 移动应用程序故障排除历史记录项</span><span class="sxs-lookup"><span data-stu-id="0c3ef-162">Intune Mobile Application Troubleshooting History Item</span></span>|
|<span data-ttu-id="0c3ef-163">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0c3ef-163">managedDeviceIdentifier</span></span>|<span data-ttu-id="0c3ef-164">String</span><span class="sxs-lookup"><span data-stu-id="0c3ef-164">String</span></span>|<span data-ttu-id="0c3ef-165">Intune 创建或收集的设备标识符。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-165">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="0c3ef-166">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0c3ef-166">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="0c3ef-167">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="0c3ef-167">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="0c3ef-168">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-168">Object containing detailed information about the error and its remediation.</span></span> |
|<span data-ttu-id="0c3ef-169">userId</span><span class="sxs-lookup"><span data-stu-id="0c3ef-169">userId</span></span>|<span data-ttu-id="0c3ef-170">String</span><span class="sxs-lookup"><span data-stu-id="0c3ef-170">String</span></span>|<span data-ttu-id="0c3ef-171">尝试注册设备的用户的标识符。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-171">Identifier for the user that tried to enroll the device.</span></span>|

## <a name="response"></a><span data-ttu-id="0c3ef-172">响应</span><span class="sxs-lookup"><span data-stu-id="0c3ef-172">Response</span></span>
<span data-ttu-id="0c3ef-173">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-173">If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c3ef-174">示例</span><span class="sxs-lookup"><span data-stu-id="0c3ef-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c3ef-175">请求</span><span class="sxs-lookup"><span data-stu-id="0c3ef-175">Request</span></span>
<span data-ttu-id="0c3ef-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a><span data-ttu-id="0c3ef-177">响应</span><span class="sxs-lookup"><span data-stu-id="0c3ef-177">Response</span></span>
<span data-ttu-id="0c3ef-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c3ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```











