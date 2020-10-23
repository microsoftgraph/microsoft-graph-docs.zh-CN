---
title: 更新 deviceManagementTroubleshootingEvent
description: 更新 deviceManagementTroubleshootingEvent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf13a36bf2e690396afe90f8e2ddac6287b8fd3f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731118"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="6f02b-103">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="6f02b-103">Update deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="6f02b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f02b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f02b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6f02b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f02b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f02b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f02b-107">更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6f02b-107">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f02b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f02b-108">Prerequisites</span></span>
<span data-ttu-id="6f02b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f02b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f02b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f02b-111">Permission type</span></span>|<span data-ttu-id="6f02b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f02b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f02b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f02b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f02b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f02b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6f02b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f02b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f02b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f02b-116">Not supported.</span></span>|
|<span data-ttu-id="6f02b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f02b-117">Application</span></span>|<span data-ttu-id="6f02b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f02b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f02b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f02b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="6f02b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f02b-120">Request headers</span></span>
|<span data-ttu-id="6f02b-121">标头</span><span class="sxs-lookup"><span data-stu-id="6f02b-121">Header</span></span>|<span data-ttu-id="6f02b-122">值</span><span class="sxs-lookup"><span data-stu-id="6f02b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f02b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f02b-123">Authorization</span></span>|<span data-ttu-id="6f02b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f02b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f02b-125">接受</span><span class="sxs-lookup"><span data-stu-id="6f02b-125">Accept</span></span>|<span data-ttu-id="6f02b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f02b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f02b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f02b-127">Request body</span></span>
<span data-ttu-id="6f02b-128">在请求正文中，提供 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f02b-128">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="6f02b-129">下表显示创建 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6f02b-129">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="6f02b-130">属性</span><span class="sxs-lookup"><span data-stu-id="6f02b-130">Property</span></span>|<span data-ttu-id="6f02b-131">类型</span><span class="sxs-lookup"><span data-stu-id="6f02b-131">Type</span></span>|<span data-ttu-id="6f02b-132">说明</span><span class="sxs-lookup"><span data-stu-id="6f02b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f02b-133">id</span><span class="sxs-lookup"><span data-stu-id="6f02b-133">id</span></span>|<span data-ttu-id="6f02b-134">String</span><span class="sxs-lookup"><span data-stu-id="6f02b-134">String</span></span>|<span data-ttu-id="6f02b-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="6f02b-135">UUID for the object</span></span>|
|<span data-ttu-id="6f02b-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="6f02b-136">eventDateTime</span></span>|<span data-ttu-id="6f02b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f02b-137">DateTimeOffset</span></span>|<span data-ttu-id="6f02b-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="6f02b-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="6f02b-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="6f02b-139">correlationId</span></span>|<span data-ttu-id="6f02b-140">String</span><span class="sxs-lookup"><span data-stu-id="6f02b-140">String</span></span>|<span data-ttu-id="6f02b-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="6f02b-141">Id used for tracing the failure in the service.</span></span>|
|<span data-ttu-id="6f02b-142">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="6f02b-142">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="6f02b-143">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="6f02b-143">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="6f02b-144">包含有关错误及其修正的详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="6f02b-144">Object containing detailed information about the error and its remediation.</span></span>|
|<span data-ttu-id="6f02b-145">名</span><span class="sxs-lookup"><span data-stu-id="6f02b-145">eventName</span></span>|<span data-ttu-id="6f02b-146">String</span><span class="sxs-lookup"><span data-stu-id="6f02b-146">String</span></span>|<span data-ttu-id="6f02b-147">与疑难解答事件对应的事件名称。</span><span class="sxs-lookup"><span data-stu-id="6f02b-147">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="6f02b-148">它是可选字段</span><span class="sxs-lookup"><span data-stu-id="6f02b-148">It is an Optional field</span></span>|
|<span data-ttu-id="6f02b-149">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="6f02b-149">additionalInformation</span></span>|<span data-ttu-id="6f02b-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f02b-150">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6f02b-151">一组字符串键和字符串值对，提供有关疑难解答事件的其他信息</span><span class="sxs-lookup"><span data-stu-id="6f02b-151">A set of string key and string value pairs which provides additional information on the Troubleshooting event</span></span>|



## <a name="response"></a><span data-ttu-id="6f02b-152">响应</span><span class="sxs-lookup"><span data-stu-id="6f02b-152">Response</span></span>
<span data-ttu-id="6f02b-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6f02b-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f02b-154">示例</span><span class="sxs-lookup"><span data-stu-id="6f02b-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f02b-155">请求</span><span class="sxs-lookup"><span data-stu-id="6f02b-155">Request</span></span>
<span data-ttu-id="6f02b-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f02b-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f02b-157">响应</span><span class="sxs-lookup"><span data-stu-id="6f02b-157">Response</span></span>
<span data-ttu-id="6f02b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f02b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





