---
title: 列出 appleVppTokenTroubleshootingEvents
description: 列出 appleVppTokenTroubleshootingEvent 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e4a5d2022ff289f4bfb7be6690801e0f162071b1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526669"
---
# <a name="list-applevpptokentroubleshootingevents"></a><span data-ttu-id="11180-103">列出 appleVppTokenTroubleshootingEvents</span><span class="sxs-lookup"><span data-stu-id="11180-103">List appleVppTokenTroubleshootingEvents</span></span>

> <span data-ttu-id="11180-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11180-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11180-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11180-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11180-106">列出[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="11180-106">List properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11180-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="11180-107">Prerequisites</span></span>
<span data-ttu-id="11180-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11180-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11180-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11180-110">Permission type</span></span>|<span data-ttu-id="11180-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="11180-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11180-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11180-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11180-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="11180-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="11180-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11180-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11180-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="11180-115">Not supported.</span></span>|
|<span data-ttu-id="11180-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="11180-116">Application</span></span>|<span data-ttu-id="11180-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="11180-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11180-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11180-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="11180-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="11180-119">Request headers</span></span>
|<span data-ttu-id="11180-120">标头</span><span class="sxs-lookup"><span data-stu-id="11180-120">Header</span></span>|<span data-ttu-id="11180-121">值</span><span class="sxs-lookup"><span data-stu-id="11180-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11180-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11180-122">Authorization</span></span>|<span data-ttu-id="11180-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="11180-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11180-124">接受</span><span class="sxs-lookup"><span data-stu-id="11180-124">Accept</span></span>|<span data-ttu-id="11180-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11180-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11180-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="11180-126">Request body</span></span>
<span data-ttu-id="11180-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="11180-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11180-128">响应</span><span class="sxs-lookup"><span data-stu-id="11180-128">Response</span></span>
<span data-ttu-id="11180-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="11180-129">If successful, this method returns a `200 OK` response code and a collection of [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11180-130">示例</span><span class="sxs-lookup"><span data-stu-id="11180-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="11180-131">请求</span><span class="sxs-lookup"><span data-stu-id="11180-131">Request</span></span>
<span data-ttu-id="11180-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="11180-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="11180-133">响应</span><span class="sxs-lookup"><span data-stu-id="11180-133">Response</span></span>
<span data-ttu-id="11180-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="11180-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1071

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleVppTokenTroubleshootingEvent",
      "id": "09295f26-5f26-0929-265f-2909265f2909",
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
      ],
      "tokenId": "Token Id value"
    }
  ]
}
```



