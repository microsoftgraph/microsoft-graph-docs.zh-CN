---
title: 创建 deviceManagementTroubleshootingEvent
description: 创建新的 deviceManagementTroubleshootingEvent 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7c135b669428b763568306aea7187b718f88ac32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450451"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="4a75a-103">创建 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="4a75a-103">Create deviceManagementTroubleshootingEvent</span></span>

<span data-ttu-id="4a75a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a75a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a75a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a75a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a75a-106">创建新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a75a-106">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a75a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4a75a-107">Prerequisites</span></span>
<span data-ttu-id="4a75a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a75a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a75a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a75a-110">Permission type</span></span>|<span data-ttu-id="4a75a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4a75a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a75a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a75a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4a75a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a75a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4a75a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a75a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a75a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a75a-115">Not supported.</span></span>|
|<span data-ttu-id="4a75a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a75a-116">Application</span></span>|<span data-ttu-id="4a75a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a75a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a75a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a75a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="4a75a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a75a-119">Request headers</span></span>
|<span data-ttu-id="4a75a-120">标头</span><span class="sxs-lookup"><span data-stu-id="4a75a-120">Header</span></span>|<span data-ttu-id="4a75a-121">值</span><span class="sxs-lookup"><span data-stu-id="4a75a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a75a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a75a-122">Authorization</span></span>|<span data-ttu-id="4a75a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4a75a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a75a-124">接受</span><span class="sxs-lookup"><span data-stu-id="4a75a-124">Accept</span></span>|<span data-ttu-id="4a75a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4a75a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a75a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a75a-126">Request body</span></span>
<span data-ttu-id="4a75a-127">在请求正文中，提供 deviceManagementTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a75a-127">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="4a75a-128">下表显示创建 deviceManagementTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4a75a-128">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="4a75a-129">属性</span><span class="sxs-lookup"><span data-stu-id="4a75a-129">Property</span></span>|<span data-ttu-id="4a75a-130">类型</span><span class="sxs-lookup"><span data-stu-id="4a75a-130">Type</span></span>|<span data-ttu-id="4a75a-131">说明</span><span class="sxs-lookup"><span data-stu-id="4a75a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a75a-132">id</span><span class="sxs-lookup"><span data-stu-id="4a75a-132">id</span></span>|<span data-ttu-id="4a75a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4a75a-133">String</span></span>|<span data-ttu-id="4a75a-134">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="4a75a-134">UUID for the object</span></span>|
|<span data-ttu-id="4a75a-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="4a75a-135">eventDateTime</span></span>|<span data-ttu-id="4a75a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a75a-136">DateTimeOffset</span></span>|<span data-ttu-id="4a75a-137">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="4a75a-137">Time when the event occurred .</span></span>|
|<span data-ttu-id="4a75a-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="4a75a-138">correlationId</span></span>|<span data-ttu-id="4a75a-139">String</span><span class="sxs-lookup"><span data-stu-id="4a75a-139">String</span></span>|<span data-ttu-id="4a75a-140">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="4a75a-140">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="4a75a-141">响应</span><span class="sxs-lookup"><span data-stu-id="4a75a-141">Response</span></span>
<span data-ttu-id="4a75a-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4a75a-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a75a-143">示例</span><span class="sxs-lookup"><span data-stu-id="4a75a-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a75a-144">请求</span><span class="sxs-lookup"><span data-stu-id="4a75a-144">Request</span></span>
<span data-ttu-id="4a75a-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4a75a-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="4a75a-146">响应</span><span class="sxs-lookup"><span data-stu-id="4a75a-146">Response</span></span>
<span data-ttu-id="4a75a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4a75a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```






