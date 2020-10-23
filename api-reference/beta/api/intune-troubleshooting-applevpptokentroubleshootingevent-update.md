---
title: 更新 appleVppTokenTroubleshootingEvent
description: 更新 appleVppTokenTroubleshootingEvent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ccedce96c47ac6d55a7f46cbff76a5fa710f94bc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48721516"
---
# <a name="update-applevpptokentroubleshootingevent"></a><span data-ttu-id="32557-103">更新 appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="32557-103">Update appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="32557-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32557-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32557-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="32557-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32557-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="32557-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32557-107">更新 [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="32557-107">Update the properties of a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32557-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="32557-108">Prerequisites</span></span>
<span data-ttu-id="32557-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32557-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32557-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="32557-111">Permission type</span></span>|<span data-ttu-id="32557-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="32557-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32557-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32557-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32557-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32557-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="32557-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32557-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32557-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="32557-116">Not supported.</span></span>|
|<span data-ttu-id="32557-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="32557-117">Application</span></span>|<span data-ttu-id="32557-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32557-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32557-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32557-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="32557-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="32557-120">Request headers</span></span>
|<span data-ttu-id="32557-121">标头</span><span class="sxs-lookup"><span data-stu-id="32557-121">Header</span></span>|<span data-ttu-id="32557-122">值</span><span class="sxs-lookup"><span data-stu-id="32557-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32557-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32557-123">Authorization</span></span>|<span data-ttu-id="32557-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="32557-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32557-125">接受</span><span class="sxs-lookup"><span data-stu-id="32557-125">Accept</span></span>|<span data-ttu-id="32557-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32557-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32557-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="32557-127">Request body</span></span>
<span data-ttu-id="32557-128">在请求正文中，提供 [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32557-128">In the request body, supply a JSON representation for the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

<span data-ttu-id="32557-129">下表显示创建 [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="32557-129">The following table shows the properties that are required when you create the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md).</span></span>

|<span data-ttu-id="32557-130">属性</span><span class="sxs-lookup"><span data-stu-id="32557-130">Property</span></span>|<span data-ttu-id="32557-131">类型</span><span class="sxs-lookup"><span data-stu-id="32557-131">Type</span></span>|<span data-ttu-id="32557-132">说明</span><span class="sxs-lookup"><span data-stu-id="32557-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32557-133">id</span><span class="sxs-lookup"><span data-stu-id="32557-133">id</span></span>|<span data-ttu-id="32557-134">String</span><span class="sxs-lookup"><span data-stu-id="32557-134">String</span></span>|<span data-ttu-id="32557-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="32557-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="32557-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="32557-136">eventDateTime</span></span>|<span data-ttu-id="32557-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32557-137">DateTimeOffset</span></span>|<span data-ttu-id="32557-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="32557-138">Time when the event occurred .</span></span> <span data-ttu-id="32557-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="32557-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="32557-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="32557-140">correlationId</span></span>|<span data-ttu-id="32557-141">String</span><span class="sxs-lookup"><span data-stu-id="32557-141">String</span></span>|<span data-ttu-id="32557-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="32557-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="32557-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="32557-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="32557-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="32557-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="32557-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="32557-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="32557-146">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="32557-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="32557-147">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="32557-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="32557-148">名</span><span class="sxs-lookup"><span data-stu-id="32557-148">eventName</span></span>|<span data-ttu-id="32557-149">String</span><span class="sxs-lookup"><span data-stu-id="32557-149">String</span></span>|<span data-ttu-id="32557-150">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="32557-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="32557-151">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="32557-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="32557-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="32557-152">additionalInformation</span></span>|<span data-ttu-id="32557-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="32557-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="32557-154">一组字符串键和字符串值对，提供有关从[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="32557-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="32557-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="32557-155">tokenId</span></span>|<span data-ttu-id="32557-156">String</span><span class="sxs-lookup"><span data-stu-id="32557-156">String</span></span>|<span data-ttu-id="32557-157">Apple Volume Purchase Program 令牌标识符。</span><span class="sxs-lookup"><span data-stu-id="32557-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="32557-158">响应</span><span class="sxs-lookup"><span data-stu-id="32557-158">Response</span></span>
<span data-ttu-id="32557-159">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="32557-159">If successful, this method returns a `200 OK` response code and an updated [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32557-160">示例</span><span class="sxs-lookup"><span data-stu-id="32557-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="32557-161">请求</span><span class="sxs-lookup"><span data-stu-id="32557-161">Request</span></span>
<span data-ttu-id="32557-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32557-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32557-163">响应</span><span class="sxs-lookup"><span data-stu-id="32557-163">Response</span></span>
<span data-ttu-id="32557-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="32557-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





