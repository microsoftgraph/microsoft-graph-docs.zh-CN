---
title: 更新 appleVppTokenTroubleshootingEvent
description: 更新 appleVppTokenTroubleshootingEvent 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0382305cb7b597d3972d7acc671d20878d210ae9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792781"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="87b31-103">更新 appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="87b31-103">Update appleVppTokenTroubleshootingEvent</span></span>

> <span data-ttu-id="87b31-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="87b31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87b31-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87b31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87b31-106">更新[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="87b31-106">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87b31-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="87b31-107">Prerequisites</span></span>
<span data-ttu-id="87b31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87b31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87b31-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="87b31-110">Permission type</span></span>|<span data-ttu-id="87b31-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="87b31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87b31-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87b31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87b31-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87b31-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="87b31-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87b31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87b31-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="87b31-115">Not supported.</span></span>|
|<span data-ttu-id="87b31-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="87b31-116">Application</span></span>|<span data-ttu-id="87b31-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="87b31-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87b31-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87b31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="87b31-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="87b31-119">Request headers</span></span>
|<span data-ttu-id="87b31-120">标头</span><span class="sxs-lookup"><span data-stu-id="87b31-120">Header</span></span>|<span data-ttu-id="87b31-121">值</span><span class="sxs-lookup"><span data-stu-id="87b31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87b31-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87b31-122">Authorization</span></span>|<span data-ttu-id="87b31-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="87b31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87b31-124">接受</span><span class="sxs-lookup"><span data-stu-id="87b31-124">Accept</span></span>|<span data-ttu-id="87b31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87b31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87b31-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="87b31-126">Request body</span></span>
<span data-ttu-id="87b31-127">在请求正文中, 提供[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87b31-127">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="87b31-128">下表显示创建[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="87b31-128">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="87b31-129">属性</span><span class="sxs-lookup"><span data-stu-id="87b31-129">Property</span></span>|<span data-ttu-id="87b31-130">类型</span><span class="sxs-lookup"><span data-stu-id="87b31-130">Type</span></span>|<span data-ttu-id="87b31-131">说明</span><span class="sxs-lookup"><span data-stu-id="87b31-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87b31-132">id</span><span class="sxs-lookup"><span data-stu-id="87b31-132">id</span></span>|<span data-ttu-id="87b31-133">String</span><span class="sxs-lookup"><span data-stu-id="87b31-133">String</span></span>|<span data-ttu-id="87b31-134">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="87b31-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="87b31-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="87b31-135">eventDateTime</span></span>|<span data-ttu-id="87b31-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87b31-136">DateTimeOffset</span></span>|<span data-ttu-id="87b31-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="87b31-137">Time when the event occurred .</span></span> <span data-ttu-id="87b31-138">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="87b31-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="87b31-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="87b31-139">correlationId</span></span>|<span data-ttu-id="87b31-140">String</span><span class="sxs-lookup"><span data-stu-id="87b31-140">String</span></span>|<span data-ttu-id="87b31-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="87b31-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="87b31-142">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="87b31-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="87b31-143">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="87b31-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="87b31-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="87b31-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="87b31-145">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="87b31-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="87b31-146">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="87b31-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="87b31-147">名</span><span class="sxs-lookup"><span data-stu-id="87b31-147">eventName</span></span>|<span data-ttu-id="87b31-148">String</span><span class="sxs-lookup"><span data-stu-id="87b31-148">String</span></span>|<span data-ttu-id="87b31-149">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="87b31-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="87b31-150">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="87b31-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="87b31-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="87b31-151">additionalInformation</span></span>|<span data-ttu-id="87b31-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="87b31-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="87b31-153">一组字符串键和字符串值对, 提供有关从[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="87b31-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="87b31-154">tokenId</span><span class="sxs-lookup"><span data-stu-id="87b31-154">tokenId</span></span>|<span data-ttu-id="87b31-155">String</span><span class="sxs-lookup"><span data-stu-id="87b31-155">String</span></span>|<span data-ttu-id="87b31-156">Apple volume purchase Program 令牌标识符。</span><span class="sxs-lookup"><span data-stu-id="87b31-156">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="87b31-157">响应</span><span class="sxs-lookup"><span data-stu-id="87b31-157">Response</span></span>
<span data-ttu-id="87b31-158">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="87b31-158">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87b31-159">示例</span><span class="sxs-lookup"><span data-stu-id="87b31-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="87b31-160">请求</span><span class="sxs-lookup"><span data-stu-id="87b31-160">Request</span></span>
<span data-ttu-id="87b31-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="87b31-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="87b31-162">响应</span><span class="sxs-lookup"><span data-stu-id="87b31-162">Response</span></span>
<span data-ttu-id="87b31-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="87b31-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



