---
title: 列出 deviceManagementTroubleshootingEvents
description: 列出 deviceManagementTroubleshootingEvent 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37ffbb1d049f3a675c115e15a1784baf200866ed
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792599"
---
# <a name="list-devicemanagementtroubleshootingevents"></a><span data-ttu-id="772a8-103">列出 deviceManagementTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="772a8-103">List deviceManagementTroubleshootingEvents</span></span>

> <span data-ttu-id="772a8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="772a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="772a8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="772a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="772a8-106">列出 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="772a8-106">List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="772a8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="772a8-107">Prerequisites</span></span>
<span data-ttu-id="772a8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="772a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="772a8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="772a8-110">Permission type</span></span>|<span data-ttu-id="772a8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="772a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="772a8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="772a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="772a8-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="772a8-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="772a8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="772a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="772a8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="772a8-115">Not supported.</span></span>|
|<span data-ttu-id="772a8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="772a8-116">Application</span></span>|<span data-ttu-id="772a8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="772a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="772a8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="772a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="772a8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="772a8-119">Request headers</span></span>
|<span data-ttu-id="772a8-120">标头</span><span class="sxs-lookup"><span data-stu-id="772a8-120">Header</span></span>|<span data-ttu-id="772a8-121">值</span><span class="sxs-lookup"><span data-stu-id="772a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="772a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="772a8-122">Authorization</span></span>|<span data-ttu-id="772a8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="772a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="772a8-124">接受</span><span class="sxs-lookup"><span data-stu-id="772a8-124">Accept</span></span>|<span data-ttu-id="772a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="772a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="772a8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="772a8-126">Request body</span></span>
<span data-ttu-id="772a8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="772a8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="772a8-128">响应</span><span class="sxs-lookup"><span data-stu-id="772a8-128">Response</span></span>
<span data-ttu-id="772a8-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="772a8-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="772a8-130">示例</span><span class="sxs-lookup"><span data-stu-id="772a8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="772a8-131">请求</span><span class="sxs-lookup"><span data-stu-id="772a8-131">Request</span></span>
<span data-ttu-id="772a8-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="772a8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="772a8-133">响应</span><span class="sxs-lookup"><span data-stu-id="772a8-133">Response</span></span>
<span data-ttu-id="772a8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="772a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1038

{
  "value": [
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
  ]
}
```



