---
title: 更新 deviceManagementTroubleshootingEvent
description: 更新 deviceManagementTroubleshootingEvent 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7afaf97d6329a3926bfa44be80793f07ee9fd890
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361096"
---
# <a name="update-devicemanagementtroubleshootingevent"></a><span data-ttu-id="3b461-103">更新 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="3b461-103">Update deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="3b461-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b461-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b461-105">更新 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3b461-105">Update the properties of a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b461-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b461-106">Prerequisites</span></span>
<span data-ttu-id="3b461-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b461-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b461-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b461-109">Permission type</span></span>|<span data-ttu-id="3b461-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3b461-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b461-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b461-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3b461-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b461-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3b461-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b461-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b461-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b461-114">Not supported.</span></span>|
|<span data-ttu-id="3b461-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b461-115">Application</span></span>|<span data-ttu-id="3b461-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b461-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b461-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b461-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="3b461-118">请求头</span><span class="sxs-lookup"><span data-stu-id="3b461-118">Request headers</span></span>
|<span data-ttu-id="3b461-119">标头</span><span class="sxs-lookup"><span data-stu-id="3b461-119">Header</span></span>|<span data-ttu-id="3b461-120">值</span><span class="sxs-lookup"><span data-stu-id="3b461-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b461-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b461-121">Authorization</span></span>|<span data-ttu-id="3b461-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b461-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b461-123">接受</span><span class="sxs-lookup"><span data-stu-id="3b461-123">Accept</span></span>|<span data-ttu-id="3b461-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3b461-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b461-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b461-125">Request body</span></span>
<span data-ttu-id="3b461-126">在请求正文中，提供 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b461-126">In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

<span data-ttu-id="3b461-127">下表显示创建 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b461-127">The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md).</span></span>

|<span data-ttu-id="3b461-128">属性</span><span class="sxs-lookup"><span data-stu-id="3b461-128">Property</span></span>|<span data-ttu-id="3b461-129">类型</span><span class="sxs-lookup"><span data-stu-id="3b461-129">Type</span></span>|<span data-ttu-id="3b461-130">说明</span><span class="sxs-lookup"><span data-stu-id="3b461-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b461-131">id</span><span class="sxs-lookup"><span data-stu-id="3b461-131">id</span></span>|<span data-ttu-id="3b461-132">字符串</span><span class="sxs-lookup"><span data-stu-id="3b461-132">String</span></span>|<span data-ttu-id="3b461-133">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="3b461-133">UUID for the object</span></span>|
|<span data-ttu-id="3b461-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="3b461-134">eventDateTime</span></span>|<span data-ttu-id="3b461-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b461-135">DateTimeOffset</span></span>|<span data-ttu-id="3b461-136">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="3b461-136">Time when the event occurred .</span></span>|
|<span data-ttu-id="3b461-137">correlationId</span><span class="sxs-lookup"><span data-stu-id="3b461-137">correlationId</span></span>|<span data-ttu-id="3b461-138">String</span><span class="sxs-lookup"><span data-stu-id="3b461-138">String</span></span>|<span data-ttu-id="3b461-139">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="3b461-139">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="3b461-140">响应</span><span class="sxs-lookup"><span data-stu-id="3b461-140">Response</span></span>
<span data-ttu-id="3b461-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3b461-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b461-142">示例</span><span class="sxs-lookup"><span data-stu-id="3b461-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b461-143">请求</span><span class="sxs-lookup"><span data-stu-id="3b461-143">Request</span></span>
<span data-ttu-id="3b461-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b461-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b461-145">响应</span><span class="sxs-lookup"><span data-stu-id="3b461-145">Response</span></span>
<span data-ttu-id="3b461-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b461-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




