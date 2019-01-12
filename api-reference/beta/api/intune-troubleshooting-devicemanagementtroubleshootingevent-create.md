---
title: 创建 deviceManagementTroubleshootingEvent
description: 创建新的 deviceManagementTroubleshootingEvent 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 108827de4760ad8573d34dccba8403cc34d40a63
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934168"
---
# <a name="create-devicemanagementtroubleshootingevent"></a><span data-ttu-id="69932-103">创建 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="69932-103">Create deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="69932-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69932-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69932-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69932-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69932-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="69932-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69932-107">创建新的 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69932-107">Create a new [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69932-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="69932-108">Prerequisites</span></span>
<span data-ttu-id="69932-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="69932-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69932-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="69932-111">Permission type</span></span>|<span data-ttu-id="69932-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69932-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69932-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69932-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69932-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69932-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="69932-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69932-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69932-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69932-116">Not supported.</span></span>|
|<span data-ttu-id="69932-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="69932-117">Application</span></span>|<span data-ttu-id="69932-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="69932-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69932-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69932-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="69932-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="69932-120">Request headers</span></span>
|<span data-ttu-id="69932-121">标头</span><span class="sxs-lookup"><span data-stu-id="69932-121">Header</span></span>|<span data-ttu-id="69932-122">值</span><span class="sxs-lookup"><span data-stu-id="69932-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69932-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69932-123">Authorization</span></span>|<span data-ttu-id="69932-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69932-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69932-125">Accept</span><span class="sxs-lookup"><span data-stu-id="69932-125">Accept</span></span>|<span data-ttu-id="69932-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69932-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69932-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="69932-127">Request body</span></span>
<span data-ttu-id="69932-128">在请求正文中，提供 deviceManagementTroubleshootingEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69932-128">In the request body, supply a JSON representation for the deviceManagementTroubleshootingEvent object.</span></span>

<span data-ttu-id="69932-129">下表显示创建 deviceManagementTroubleshootingEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="69932-129">The following table shows the properties that are required when you create the deviceManagementTroubleshootingEvent.</span></span>

|<span data-ttu-id="69932-130">属性</span><span class="sxs-lookup"><span data-stu-id="69932-130">Property</span></span>|<span data-ttu-id="69932-131">类型</span><span class="sxs-lookup"><span data-stu-id="69932-131">Type</span></span>|<span data-ttu-id="69932-132">说明</span><span class="sxs-lookup"><span data-stu-id="69932-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69932-133">id</span><span class="sxs-lookup"><span data-stu-id="69932-133">id</span></span>|<span data-ttu-id="69932-134">String</span><span class="sxs-lookup"><span data-stu-id="69932-134">String</span></span>|<span data-ttu-id="69932-135">对象的 UUID</span><span class="sxs-lookup"><span data-stu-id="69932-135">UUID for the object</span></span>|
|<span data-ttu-id="69932-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="69932-136">eventDateTime</span></span>|<span data-ttu-id="69932-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69932-137">DateTimeOffset</span></span>|<span data-ttu-id="69932-138">事件发生的时间。</span><span class="sxs-lookup"><span data-stu-id="69932-138">Time when the event occurred .</span></span>|
|<span data-ttu-id="69932-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="69932-139">correlationId</span></span>|<span data-ttu-id="69932-140">String</span><span class="sxs-lookup"><span data-stu-id="69932-140">String</span></span>|<span data-ttu-id="69932-141">用于跟踪服务中的故障的 ID。</span><span class="sxs-lookup"><span data-stu-id="69932-141">Id used for tracing the failure in the service.</span></span>|



## <a name="response"></a><span data-ttu-id="69932-142">响应</span><span class="sxs-lookup"><span data-stu-id="69932-142">Response</span></span>
<span data-ttu-id="69932-143">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="69932-143">If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69932-144">示例</span><span class="sxs-lookup"><span data-stu-id="69932-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="69932-145">请求</span><span class="sxs-lookup"><span data-stu-id="69932-145">Request</span></span>
<span data-ttu-id="69932-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69932-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value"
}
```

### <a name="response"></a><span data-ttu-id="69932-147">响应</span><span class="sxs-lookup"><span data-stu-id="69932-147">Response</span></span>
<span data-ttu-id="69932-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69932-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





