---
title: 更新 appleVppTokenTroubleshootingEvent
description: 更新 appleVppTokenTroubleshootingEvent 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3382eb7069be27fb47bf094d4a0688d7cd128de6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429388"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="a46dc-103">更新 appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="a46dc-103">Update appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="a46dc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a46dc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a46dc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a46dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a46dc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a46dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a46dc-107">更新[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a46dc-107">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a46dc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a46dc-108">Prerequisites</span></span>
<span data-ttu-id="a46dc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a46dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a46dc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a46dc-111">Permission type</span></span>|<span data-ttu-id="a46dc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a46dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a46dc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a46dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a46dc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a46dc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a46dc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a46dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a46dc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a46dc-116">Not supported.</span></span>|
|<span data-ttu-id="a46dc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a46dc-117">Application</span></span>|<span data-ttu-id="a46dc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a46dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a46dc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a46dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="a46dc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a46dc-120">Request headers</span></span>
|<span data-ttu-id="a46dc-121">标头</span><span class="sxs-lookup"><span data-stu-id="a46dc-121">Header</span></span>|<span data-ttu-id="a46dc-122">值</span><span class="sxs-lookup"><span data-stu-id="a46dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a46dc-123">授权</span><span class="sxs-lookup"><span data-stu-id="a46dc-123">Authorization</span></span>|<span data-ttu-id="a46dc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a46dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a46dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a46dc-125">Accept</span></span>|<span data-ttu-id="a46dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a46dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a46dc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a46dc-127">Request body</span></span>
<span data-ttu-id="a46dc-128">在请求正文中，提供[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a46dc-128">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="a46dc-129">下表显示时创建[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a46dc-129">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="a46dc-130">属性</span><span class="sxs-lookup"><span data-stu-id="a46dc-130">Property</span></span>|<span data-ttu-id="a46dc-131">类型</span><span class="sxs-lookup"><span data-stu-id="a46dc-131">Type</span></span>|<span data-ttu-id="a46dc-132">说明</span><span class="sxs-lookup"><span data-stu-id="a46dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a46dc-133">id</span><span class="sxs-lookup"><span data-stu-id="a46dc-133">id</span></span>|<span data-ttu-id="a46dc-134">String</span><span class="sxs-lookup"><span data-stu-id="a46dc-134">String</span></span>|<span data-ttu-id="a46dc-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a46dc-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a46dc-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a46dc-136">eventDateTime</span></span>|<span data-ttu-id="a46dc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a46dc-137">DateTimeOffset</span></span>|<span data-ttu-id="a46dc-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="a46dc-138">Time when the event occurred .</span></span> <span data-ttu-id="a46dc-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a46dc-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a46dc-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="a46dc-140">correlationId</span></span>|<span data-ttu-id="a46dc-141">String</span><span class="sxs-lookup"><span data-stu-id="a46dc-141">String</span></span>|<span data-ttu-id="a46dc-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="a46dc-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="a46dc-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a46dc-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a46dc-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a46dc-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="a46dc-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a46dc-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="a46dc-146">对象包含有关错误和其修复的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="a46dc-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="a46dc-147">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a46dc-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a46dc-148">事件名称</span><span class="sxs-lookup"><span data-stu-id="a46dc-148">eventName</span></span>|<span data-ttu-id="a46dc-149">String</span><span class="sxs-lookup"><span data-stu-id="a46dc-149">String</span></span>|<span data-ttu-id="a46dc-150">对应于疑难解答事件的事件名称。</span><span class="sxs-lookup"><span data-stu-id="a46dc-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="a46dc-151">它是一个可选字段继承从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="a46dc-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a46dc-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="a46dc-152">additionalInformation</span></span>|<span data-ttu-id="a46dc-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a46dc-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a46dc-154">一组字符串键和字符串值对提供了有关从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)疑难解答事件继承其他信息</span><span class="sxs-lookup"><span data-stu-id="a46dc-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="a46dc-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="a46dc-155">tokenId</span></span>|<span data-ttu-id="a46dc-156">String</span><span class="sxs-lookup"><span data-stu-id="a46dc-156">String</span></span>|<span data-ttu-id="a46dc-157">Apple 卷购买程序令牌标识符。</span><span class="sxs-lookup"><span data-stu-id="a46dc-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="a46dc-158">响应</span><span class="sxs-lookup"><span data-stu-id="a46dc-158">Response</span></span>
<span data-ttu-id="a46dc-159">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a46dc-159">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a46dc-160">示例</span><span class="sxs-lookup"><span data-stu-id="a46dc-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="a46dc-161">请求</span><span class="sxs-lookup"><span data-stu-id="a46dc-161">Request</span></span>
<span data-ttu-id="a46dc-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a46dc-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
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

### <a name="response"></a><span data-ttu-id="a46dc-163">响应</span><span class="sxs-lookup"><span data-stu-id="a46dc-163">Response</span></span>
<span data-ttu-id="a46dc-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a46dc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




