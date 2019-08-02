---
title: 更新 deviceManagementTroubleshootingEvent
description: 更新 deviceManagementTroubleshootingEvent 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3efa4e717e006d54e0786b260cc77fd749412622
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025678"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="be777-103">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="be777-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="be777-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be777-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be777-105">更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="be777-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be777-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="be777-106">Prerequisites</span></span>
<span data-ttu-id="be777-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be777-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="be777-109">Permission type</span></span>|<span data-ttu-id="be777-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="be777-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be777-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be777-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be777-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be777-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="be777-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be777-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be777-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="be777-114">Not supported.</span></span>|
|<span data-ttu-id="be777-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="be777-115">Application</span></span>|<span data-ttu-id="be777-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="be777-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be777-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be777-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="be777-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="be777-118">Request headers</span></span>
|<span data-ttu-id="be777-119">标头</span><span class="sxs-lookup"><span data-stu-id="be777-119">Header</span></span>|<span data-ttu-id="be777-120">值</span><span class="sxs-lookup"><span data-stu-id="be777-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be777-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be777-121">Authorization</span></span>|<span data-ttu-id="be777-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="be777-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be777-123">接受</span><span class="sxs-lookup"><span data-stu-id="be777-123">Accept</span></span>|<span data-ttu-id="be777-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be777-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be777-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="be777-125">Request body</span></span>
<span data-ttu-id="be777-126">在请求正文中，提供 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be777-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="be777-127">下表显示创建 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="be777-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="be777-128">属性</span><span class="sxs-lookup"><span data-stu-id="be777-128">Property</span></span>|<span data-ttu-id="be777-129">类型</span><span class="sxs-lookup"><span data-stu-id="be777-129">Type</span></span>|<span data-ttu-id="be777-130">说明</span><span class="sxs-lookup"><span data-stu-id="be777-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be777-131">id</span><span class="sxs-lookup"><span data-stu-id="be777-131">id</span></span>|<span data-ttu-id="be777-132">字符串</span><span class="sxs-lookup"><span data-stu-id="be777-132">String</span></span>|<span data-ttu-id="be777-133">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="be777-133">UUID for the object</span></span>|
|<span data-ttu-id="be777-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="be777-134">eventDateTime</span></span>|<span data-ttu-id="be777-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be777-135">DateTimeOffset</span></span>|<span data-ttu-id="be777-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="be777-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="be777-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="be777-137">correlationId</span></span>|<span data-ttu-id="be777-138">String</span><span class="sxs-lookup"><span data-stu-id="be777-138">String</span></span>|<span data-ttu-id="be777-139">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="be777-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="be777-140">响应</span><span class="sxs-lookup"><span data-stu-id="be777-140">Response</span></span>
<span data-ttu-id="be777-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be777-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be777-142">示例</span><span class="sxs-lookup"><span data-stu-id="be777-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="be777-143">请求</span><span class="sxs-lookup"><span data-stu-id="be777-143">Request</span></span>
<span data-ttu-id="be777-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be777-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be777-145">响应</span><span class="sxs-lookup"><span data-stu-id="be777-145">Response</span></span>
<span data-ttu-id="be777-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be777-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



