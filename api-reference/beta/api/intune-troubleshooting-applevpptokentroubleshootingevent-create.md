---
title: 创建 appleVppTokenTroubleshootingEvent
description: 创建新的 appleVppTokenTroubleshootingEvent 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 849d13c0ddf93578f2132291c9a7de8029806ee6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980349"
---
# <a name="create-applevpptokentroubleshootingevent"></a><span data-ttu-id="ba825-103">创建 appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="ba825-103">Create appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="ba825-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba825-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba825-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba825-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba825-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba825-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba825-107">创建新的 [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba825-107">Create a new [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba825-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ba825-108">Prerequisites</span></span>
<span data-ttu-id="ba825-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba825-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba825-111">Permission type</span></span>|<span data-ttu-id="ba825-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ba825-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba825-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba825-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba825-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba825-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ba825-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba825-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba825-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba825-116">Not supported.</span></span>|
|<span data-ttu-id="ba825-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba825-117">Application</span></span>|<span data-ttu-id="ba825-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba825-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba825-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba825-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="ba825-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba825-120">Request headers</span></span>
|<span data-ttu-id="ba825-121">标头</span><span class="sxs-lookup"><span data-stu-id="ba825-121">Header</span></span>|<span data-ttu-id="ba825-122">值</span><span class="sxs-lookup"><span data-stu-id="ba825-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba825-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba825-123">Authorization</span></span>|<span data-ttu-id="ba825-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ba825-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba825-125">接受</span><span class="sxs-lookup"><span data-stu-id="ba825-125">Accept</span></span>|<span data-ttu-id="ba825-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba825-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba825-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba825-127">Request body</span></span>
<span data-ttu-id="ba825-128">在请求正文中，提供 appleVppTokenTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba825-128">In the request body, supply a JSON representation for the appleVppTokenTroubleshootingEvent object.</span></span>

<span data-ttu-id="ba825-129">下表显示创建 appleVppTokenTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ba825-129">The following table shows the properties that are required when you create the appleVppTokenTroubleshootingEvent.</span></span>

|<span data-ttu-id="ba825-130">属性</span><span class="sxs-lookup"><span data-stu-id="ba825-130">Property</span></span>|<span data-ttu-id="ba825-131">类型</span><span class="sxs-lookup"><span data-stu-id="ba825-131">Type</span></span>|<span data-ttu-id="ba825-132">说明</span><span class="sxs-lookup"><span data-stu-id="ba825-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba825-133">id</span><span class="sxs-lookup"><span data-stu-id="ba825-133">id</span></span>|<span data-ttu-id="ba825-134">String</span><span class="sxs-lookup"><span data-stu-id="ba825-134">String</span></span>|<span data-ttu-id="ba825-135">对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="ba825-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ba825-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="ba825-136">eventDateTime</span></span>|<span data-ttu-id="ba825-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba825-137">DateTimeOffset</span></span>|<span data-ttu-id="ba825-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="ba825-138">Time when the event occurred .</span></span> <span data-ttu-id="ba825-139">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="ba825-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ba825-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="ba825-140">correlationId</span></span>|<span data-ttu-id="ba825-141">String</span><span class="sxs-lookup"><span data-stu-id="ba825-141">String</span></span>|<span data-ttu-id="ba825-142">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="ba825-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="ba825-143">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="ba825-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ba825-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ba825-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="ba825-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="ba825-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="ba825-146">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="ba825-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="ba825-147">继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span><span class="sxs-lookup"><span data-stu-id="ba825-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ba825-148">名</span><span class="sxs-lookup"><span data-stu-id="ba825-148">eventName</span></span>|<span data-ttu-id="ba825-149">String</span><span class="sxs-lookup"><span data-stu-id="ba825-149">String</span></span>|<span data-ttu-id="ba825-150">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="ba825-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="ba825-151">它是一个继承自[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)的可选字段</span><span class="sxs-lookup"><span data-stu-id="ba825-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ba825-152">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="ba825-152">additionalInformation</span></span>|<span data-ttu-id="ba825-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba825-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ba825-154">一组字符串键和字符串值对，提供有关从[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)继承的故障排除事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="ba825-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="ba825-155">tokenId</span><span class="sxs-lookup"><span data-stu-id="ba825-155">tokenId</span></span>|<span data-ttu-id="ba825-156">String</span><span class="sxs-lookup"><span data-stu-id="ba825-156">String</span></span>|<span data-ttu-id="ba825-157">Apple Volume Purchase Program 令牌标识符。</span><span class="sxs-lookup"><span data-stu-id="ba825-157">Apple Volume Purchase Program Token Identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="ba825-158">响应</span><span class="sxs-lookup"><span data-stu-id="ba825-158">Response</span></span>
<span data-ttu-id="ba825-159">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba825-159">If successful, this method returns a `201 Created` response code and a [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba825-160">示例</span><span class="sxs-lookup"><span data-stu-id="ba825-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba825-161">请求</span><span class="sxs-lookup"><span data-stu-id="ba825-161">Request</span></span>
<span data-ttu-id="ba825-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba825-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ba825-163">响应</span><span class="sxs-lookup"><span data-stu-id="ba825-163">Response</span></span>
<span data-ttu-id="ba825-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ba825-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






