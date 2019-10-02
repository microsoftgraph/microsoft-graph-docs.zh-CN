---
title: 获取 deviceManagementTroubleshootingEvent
description: 读取 deviceManagementTroubleshootingEvent 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e53af3190d9c1282dbd7eb90908495c3d807906
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361145"
---
# <a name="get-devicemanagementtroubleshootingevent"></a><span data-ttu-id="e76fc-103">获取 deviceManagementTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="e76fc-103">Get deviceManagementTroubleshootingEvent</span></span>

> <span data-ttu-id="e76fc-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e76fc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e76fc-105">读取 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e76fc-105">Read properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e76fc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e76fc-106">Prerequisites</span></span>
<span data-ttu-id="e76fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e76fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e76fc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e76fc-109">Permission type</span></span>|<span data-ttu-id="e76fc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e76fc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e76fc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e76fc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e76fc-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e76fc-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e76fc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e76fc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e76fc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e76fc-114">Not supported.</span></span>|
|<span data-ttu-id="e76fc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e76fc-115">Application</span></span>|<span data-ttu-id="e76fc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e76fc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e76fc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e76fc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e76fc-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e76fc-118">Optional query parameters</span></span>
<span data-ttu-id="e76fc-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e76fc-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e76fc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e76fc-120">Request headers</span></span>
|<span data-ttu-id="e76fc-121">标头</span><span class="sxs-lookup"><span data-stu-id="e76fc-121">Header</span></span>|<span data-ttu-id="e76fc-122">值</span><span class="sxs-lookup"><span data-stu-id="e76fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e76fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e76fc-123">Authorization</span></span>|<span data-ttu-id="e76fc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e76fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e76fc-125">接受</span><span class="sxs-lookup"><span data-stu-id="e76fc-125">Accept</span></span>|<span data-ttu-id="e76fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e76fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e76fc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e76fc-127">Request body</span></span>
<span data-ttu-id="e76fc-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e76fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e76fc-129">响应</span><span class="sxs-lookup"><span data-stu-id="e76fc-129">Response</span></span>
<span data-ttu-id="e76fc-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e76fc-130">If successful, this method returns a `200 OK` response code and [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e76fc-131">示例</span><span class="sxs-lookup"><span data-stu-id="e76fc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e76fc-132">请求</span><span class="sxs-lookup"><span data-stu-id="e76fc-132">Request</span></span>
<span data-ttu-id="e76fc-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e76fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="e76fc-134">响应</span><span class="sxs-lookup"><span data-stu-id="e76fc-134">Response</span></span>
<span data-ttu-id="e76fc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e76fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
    "id": "fb26dcee-dcee-fb26-eedc-26fbeedc26fb",
    "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
    "correlationId": "Correlation Id value"
  }
}
```




