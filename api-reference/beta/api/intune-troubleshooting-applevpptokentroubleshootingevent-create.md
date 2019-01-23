---
title: 创建 appleVppTokenTroubleshootingEvent
description: 创建新的 appleVppTokenTroubleshootingEvent 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2db5607059ca16d1b1df00f4f0f21d7233ab6db
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431354"
---
# <a name="create-applevpptokentroubleshootingevent"></a><span data-ttu-id="17455-103">创建 appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="17455-103">Create appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="17455-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="17455-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="17455-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="17455-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17455-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17455-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17455-107">创建新的[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="17455-107">Create a new [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17455-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="17455-108">Prerequisites</span></span>
<span data-ttu-id="17455-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="17455-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="17455-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="17455-111">Permission type</span></span>|<span data-ttu-id="17455-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="17455-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17455-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17455-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17455-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17455-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="17455-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17455-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17455-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="17455-116">Not supported.</span></span>|
|<span data-ttu-id="17455-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="17455-117">Application</span></span>|<span data-ttu-id="17455-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="17455-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17455-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17455-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="17455-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="17455-120">Request headers</span></span>
|<span data-ttu-id="17455-121">标头</span><span class="sxs-lookup"><span data-stu-id="17455-121">Header</span></span>|<span data-ttu-id="17455-122">值</span><span class="sxs-lookup"><span data-stu-id="17455-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17455-123">授权</span><span class="sxs-lookup"><span data-stu-id="17455-123">Authorization</span></span>|<span data-ttu-id="17455-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="17455-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17455-125">Accept</span><span class="sxs-lookup"><span data-stu-id="17455-125">Accept</span></span>|<span data-ttu-id="17455-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17455-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17455-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="17455-127">Request body</span></span>
<span data-ttu-id="17455-128">在请求正文中，提供 appleVppTokenTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17455-128">In the request body, supply a JSON representation for the appleVppTokenTroubleshootingEvent object.</span></span>

<span data-ttu-id="17455-129">下表显示时创建 appleVppTokenTroubleshootingEvent 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="17455-129">The following table shows the properties that are required when you create the appleVppTokenTroubleshootingEvent.</span></span>

|<span data-ttu-id="17455-130">属性</span><span class="sxs-lookup"><span data-stu-id="17455-130">Property</span></span>|<span data-ttu-id="17455-131">类型</span><span class="sxs-lookup"><span data-stu-id="17455-131">Type</span></span>|<span data-ttu-id="17455-132">说明</span><span class="sxs-lookup"><span data-stu-id="17455-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17455-133">id</span><span class="sxs-lookup"><span data-stu-id="17455-133">id</span></span>|<span data-ttu-id="17455-134">String</span><span class="sxs-lookup"><span data-stu-id="17455-134">String</span></span>|<span data-ttu-id="17455-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="17455-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="17455-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="17455-136">eventDateTime</span></span>|<span data-ttu-id="17455-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17455-137">DateTimeOffset</span></span>|<span data-ttu-id="17455-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="17455-138">Time when the event occurred .</span></span> <span data-ttu-id="17455-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="17455-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="17455-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="17455-140">correlationId</span></span>|<span data-ttu-id="17455-141">String</span><span class="sxs-lookup"><span data-stu-id="17455-141">String</span></span>|<span data-ttu-id="17455-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="17455-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="17455-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="17455-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="17455-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="17455-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="17455-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="17455-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="17455-146">对象包含有关错误和其修复的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="17455-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="17455-147">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="17455-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="17455-148">事件名称</span><span class="sxs-lookup"><span data-stu-id="17455-148">eventName</span></span>|<span data-ttu-id="17455-149">String</span><span class="sxs-lookup"><span data-stu-id="17455-149">String</span></span>|<span data-ttu-id="17455-150">对应于疑难解答事件的事件名称。</span><span class="sxs-lookup"><span data-stu-id="17455-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="17455-151">它是一个可选字段继承从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="17455-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="17455-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="17455-152">additionalInformation</span></span>|<span data-ttu-id="17455-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17455-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="17455-154">一组字符串键和字符串值对提供了有关从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)疑难解答事件继承其他信息</span><span class="sxs-lookup"><span data-stu-id="17455-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="17455-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="17455-155">tokenId</span></span>|<span data-ttu-id="17455-156">String</span><span class="sxs-lookup"><span data-stu-id="17455-156">String</span></span>|<span data-ttu-id="17455-157">Apple 卷购买程序令牌标识符。</span><span class="sxs-lookup"><span data-stu-id="17455-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="17455-158">响应</span><span class="sxs-lookup"><span data-stu-id="17455-158">Response</span></span>
<span data-ttu-id="17455-159">如果成功，此方法返回`201 Created`响应代码和响应正文中的[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="17455-159">If successful, this method returns a `201 Created` response code and a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17455-160">示例</span><span class="sxs-lookup"><span data-stu-id="17455-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="17455-161">请求</span><span class="sxs-lookup"><span data-stu-id="17455-161">Request</span></span>
<span data-ttu-id="17455-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17455-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 881

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "tokenId": "Token Id value"
}
```

### <a name="response"></a><span data-ttu-id="17455-163">响应</span><span class="sxs-lookup"><span data-stu-id="17455-163">Response</span></span>
<span data-ttu-id="17455-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17455-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 930

{
  "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
  "id": "09295f26-5f26-0929-265f-2909265f2909",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "tokenId": "Token Id value"
}
```




