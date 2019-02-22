---
title: 更新 deviceManagementTroubleshootingEvent
description: 更新 deviceManagementTroubleshootingEvent 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ad17f38f4f9f078c956045f9f29950105f3461f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174746"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="e5e88-103">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e5e88-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="e5e88-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5e88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5e88-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5e88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5e88-106">更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e5e88-106">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5e88-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e5e88-107">Prerequisites</span></span>
<span data-ttu-id="e5e88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e5e88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e5e88-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5e88-110">Permission type</span></span>|<span data-ttu-id="e5e88-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e5e88-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5e88-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5e88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5e88-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5e88-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e5e88-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5e88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5e88-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5e88-115">Not supported.</span></span>|
|<span data-ttu-id="e5e88-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5e88-116">Application</span></span>|<span data-ttu-id="e5e88-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5e88-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5e88-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5e88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="e5e88-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5e88-119">Request headers</span></span>
|<span data-ttu-id="e5e88-120">标头</span><span class="sxs-lookup"><span data-stu-id="e5e88-120">Header</span></span>|<span data-ttu-id="e5e88-121">值</span><span class="sxs-lookup"><span data-stu-id="e5e88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5e88-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5e88-122">Authorization</span></span>|<span data-ttu-id="e5e88-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e5e88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5e88-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e5e88-124">Accept</span></span>|<span data-ttu-id="e5e88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5e88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5e88-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5e88-126">Request body</span></span>
<span data-ttu-id="e5e88-127">在请求正文中，提供 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5e88-127">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="e5e88-128">下表显示创建 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e5e88-128">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="e5e88-129">属性</span><span class="sxs-lookup"><span data-stu-id="e5e88-129">Property</span></span>|<span data-ttu-id="e5e88-130">类型</span><span class="sxs-lookup"><span data-stu-id="e5e88-130">Type</span></span>|<span data-ttu-id="e5e88-131">说明</span><span class="sxs-lookup"><span data-stu-id="e5e88-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5e88-132">id</span><span class="sxs-lookup"><span data-stu-id="e5e88-132">id</span></span>|<span data-ttu-id="e5e88-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e5e88-133">String</span></span>|<span data-ttu-id="e5e88-134">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="e5e88-134">UUID for the object</span></span>|
|<span data-ttu-id="e5e88-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e5e88-135">eventDateTime</span></span>|<span data-ttu-id="e5e88-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5e88-136">DateTimeOffset</span></span>|<span data-ttu-id="e5e88-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="e5e88-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="e5e88-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="e5e88-138">correlationId</span></span>|<span data-ttu-id="e5e88-139">String</span><span class="sxs-lookup"><span data-stu-id="e5e88-139">String</span></span>|<span data-ttu-id="e5e88-140">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="e5e88-140">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="e5e88-141">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e5e88-141">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="e5e88-142">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e5e88-142">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="e5e88-143">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="e5e88-143">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="e5e88-144">名</span><span class="sxs-lookup"><span data-stu-id="e5e88-144">eventName</span></span>|<span data-ttu-id="e5e88-145">字符串</span><span class="sxs-lookup"><span data-stu-id="e5e88-145">String</span></span>|<span data-ttu-id="e5e88-146">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="e5e88-146">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="e5e88-147">它是可选字段</span><span class="sxs-lookup"><span data-stu-id="e5e88-147">It is an Optional field</span></span>|
|<span data-ttu-id="e5e88-148">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="e5e88-148">additionalInformation</span></span>|<span data-ttu-id="e5e88-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5e88-149">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e5e88-150">一组字符串键和字符串值对, 提供有关疑难解答事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="e5e88-150">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="e5e88-151">响应</span><span class="sxs-lookup"><span data-stu-id="e5e88-151">Response</span></span>
<span data-ttu-id="e5e88-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e5e88-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5e88-153">示例</span><span class="sxs-lookup"><span data-stu-id="e5e88-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5e88-154">请求</span><span class="sxs-lookup"><span data-stu-id="e5e88-154">Request</span></span>
<span data-ttu-id="e5e88-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e5e88-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 852

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="e5e88-156">响应</span><span class="sxs-lookup"><span data-stu-id="e5e88-156">Response</span></span>
<span data-ttu-id="e5e88-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e5e88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 901

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
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
  ]
}
```




