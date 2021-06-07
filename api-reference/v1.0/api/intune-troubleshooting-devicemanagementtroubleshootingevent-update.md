---
title: 更新 deviceManagementTroubleshootingEvent
description: 更新 deviceManagementTroubleshootingEvent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e9768948b542a08901dcf43f728f90ab3c70535b
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732401"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="77aa4-103">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="77aa4-103">Update deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="77aa4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77aa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77aa4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77aa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77aa4-106">更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="77aa4-106">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77aa4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="77aa4-107">Prerequisites</span></span>
<span data-ttu-id="77aa4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77aa4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="77aa4-110">Permission type</span></span>|<span data-ttu-id="77aa4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="77aa4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77aa4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77aa4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77aa4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77aa4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="77aa4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77aa4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77aa4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77aa4-115">Not supported.</span></span>|
|<span data-ttu-id="77aa4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="77aa4-116">Application</span></span>|<span data-ttu-id="77aa4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="77aa4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77aa4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77aa4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="77aa4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="77aa4-119">Request headers</span></span>
|<span data-ttu-id="77aa4-120">标头</span><span class="sxs-lookup"><span data-stu-id="77aa4-120">Header</span></span>|<span data-ttu-id="77aa4-121">值</span><span class="sxs-lookup"><span data-stu-id="77aa4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77aa4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77aa4-122">Authorization</span></span>|<span data-ttu-id="77aa4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77aa4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77aa4-124">接受</span><span class="sxs-lookup"><span data-stu-id="77aa4-124">Accept</span></span>|<span data-ttu-id="77aa4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77aa4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77aa4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="77aa4-126">Request body</span></span>
<span data-ttu-id="77aa4-127">在请求正文中，提供 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77aa4-127">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="77aa4-128">下表显示创建 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="77aa4-128">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="77aa4-129">属性</span><span class="sxs-lookup"><span data-stu-id="77aa4-129">Property</span></span>|<span data-ttu-id="77aa4-130">类型</span><span class="sxs-lookup"><span data-stu-id="77aa4-130">Type</span></span>|<span data-ttu-id="77aa4-131">说明</span><span class="sxs-lookup"><span data-stu-id="77aa4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77aa4-132">id</span><span class="sxs-lookup"><span data-stu-id="77aa4-132">id</span></span>|<span data-ttu-id="77aa4-133">String</span><span class="sxs-lookup"><span data-stu-id="77aa4-133">String</span></span>|<span data-ttu-id="77aa4-134">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="77aa4-134">UUID for the object</span></span>|
|<span data-ttu-id="77aa4-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="77aa4-135">eventDateTime</span></span>|<span data-ttu-id="77aa4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77aa4-136">DateTimeOffset</span></span>|<span data-ttu-id="77aa4-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="77aa4-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="77aa4-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="77aa4-138">correlationId</span></span>|<span data-ttu-id="77aa4-139">String</span><span class="sxs-lookup"><span data-stu-id="77aa4-139">String</span></span>|<span data-ttu-id="77aa4-140">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="77aa4-140">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="77aa4-141">响应</span><span class="sxs-lookup"><span data-stu-id="77aa4-141">Response</span></span>
<span data-ttu-id="77aa4-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="77aa4-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77aa4-143">示例</span><span class="sxs-lookup"><span data-stu-id="77aa4-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="77aa4-144">请求</span><span class="sxs-lookup"><span data-stu-id="77aa4-144">Request</span></span>
<span data-ttu-id="77aa4-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77aa4-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="77aa4-146">响应</span><span class="sxs-lookup"><span data-stu-id="77aa4-146">Response</span></span>
<span data-ttu-id="77aa4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77aa4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```









