---
title: 更新 deviceManagementTroubleshootingEvent
description: 更新 deviceManagementTroubleshootingEvent 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 935a5b835669a2d87fd761d8c62ccba537022f91
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415395"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="e1b44-103">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e1b44-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="e1b44-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e1b44-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1b44-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e1b44-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1b44-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1b44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1b44-107">更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e1b44-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1b44-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e1b44-108">Prerequisites</span></span>
<span data-ttu-id="e1b44-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e1b44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e1b44-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1b44-111">Permission type</span></span>|<span data-ttu-id="e1b44-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e1b44-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1b44-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1b44-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1b44-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1b44-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e1b44-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1b44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1b44-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1b44-116">Not supported.</span></span>|
|<span data-ttu-id="e1b44-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1b44-117">Application</span></span>|<span data-ttu-id="e1b44-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1b44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1b44-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1b44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="e1b44-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1b44-120">Request headers</span></span>
|<span data-ttu-id="e1b44-121">标头</span><span class="sxs-lookup"><span data-stu-id="e1b44-121">Header</span></span>|<span data-ttu-id="e1b44-122">值</span><span class="sxs-lookup"><span data-stu-id="e1b44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1b44-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1b44-123">Authorization</span></span>|<span data-ttu-id="e1b44-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e1b44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1b44-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1b44-125">Accept</span></span>|<span data-ttu-id="e1b44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1b44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1b44-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1b44-127">Request body</span></span>
<span data-ttu-id="e1b44-128">在请求正文中，提供 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1b44-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="e1b44-129">下表显示创建 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e1b44-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="e1b44-130">属性</span><span class="sxs-lookup"><span data-stu-id="e1b44-130">Property</span></span>|<span data-ttu-id="e1b44-131">类型</span><span class="sxs-lookup"><span data-stu-id="e1b44-131">Type</span></span>|<span data-ttu-id="e1b44-132">说明</span><span class="sxs-lookup"><span data-stu-id="e1b44-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1b44-133">id</span><span class="sxs-lookup"><span data-stu-id="e1b44-133">id</span></span>|<span data-ttu-id="e1b44-134">String</span><span class="sxs-lookup"><span data-stu-id="e1b44-134">String</span></span>|<span data-ttu-id="e1b44-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="e1b44-135">UUID for the object</span></span>|
|<span data-ttu-id="e1b44-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="e1b44-136">eventDateTime</span></span>|<span data-ttu-id="e1b44-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1b44-137">DateTimeOffset</span></span>|<span data-ttu-id="e1b44-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="e1b44-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="e1b44-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="e1b44-139">correlationId</span></span>|<span data-ttu-id="e1b44-140">String</span><span class="sxs-lookup"><span data-stu-id="e1b44-140">String</span></span>|<span data-ttu-id="e1b44-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="e1b44-141">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="e1b44-142">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e1b44-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="e1b44-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="e1b44-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="e1b44-144">对象包含有关错误和其修复的详细的信息。</span><span class="sxs-lookup"><span data-stu-id="e1b44-144">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="e1b44-145">事件名称</span><span class="sxs-lookup"><span data-stu-id="e1b44-145">eventName</span></span>|<span data-ttu-id="e1b44-146">String</span><span class="sxs-lookup"><span data-stu-id="e1b44-146">String</span></span>|<span data-ttu-id="e1b44-147">对应于疑难解答事件的事件名称。</span><span class="sxs-lookup"><span data-stu-id="e1b44-147">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="e1b44-148">它是一个可选字段</span><span class="sxs-lookup"><span data-stu-id="e1b44-148">It is an Optional field</span></span>|
|<span data-ttu-id="e1b44-149">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="e1b44-149">additionalInformation</span></span>|<span data-ttu-id="e1b44-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1b44-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e1b44-151">一组字符串键和字符串值对提供了有关疑难解答事件其他信息</span><span class="sxs-lookup"><span data-stu-id="e1b44-151">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="e1b44-152">响应</span><span class="sxs-lookup"><span data-stu-id="e1b44-152">Response</span></span>
<span data-ttu-id="e1b44-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e1b44-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1b44-154">示例</span><span class="sxs-lookup"><span data-stu-id="e1b44-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1b44-155">请求</span><span class="sxs-lookup"><span data-stu-id="e1b44-155">Request</span></span>
<span data-ttu-id="e1b44-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e1b44-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1b44-157">响应</span><span class="sxs-lookup"><span data-stu-id="e1b44-157">Response</span></span>
<span data-ttu-id="e1b44-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1b44-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




