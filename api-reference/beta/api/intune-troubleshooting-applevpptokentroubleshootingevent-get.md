---
title: 获取 appleVppTokenTroubleshootingEvent
description: 读取 appleVppTokenTroubleshootingEvent 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15244742bd9343777bc397246000586747b06ba9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980314"
---
# <a name="get-applevpptokentroubleshootingevent"></a><span data-ttu-id="9601e-103">获取 appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="9601e-103">Get appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="9601e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9601e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9601e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9601e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9601e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9601e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9601e-107">读取 [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9601e-107">Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9601e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9601e-108">Prerequisites</span></span>
<span data-ttu-id="9601e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9601e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9601e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9601e-111">Permission type</span></span>|<span data-ttu-id="9601e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9601e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9601e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9601e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9601e-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9601e-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9601e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9601e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9601e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9601e-116">Not supported.</span></span>|
|<span data-ttu-id="9601e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9601e-117">Application</span></span>|<span data-ttu-id="9601e-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9601e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9601e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9601e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9601e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9601e-120">Optional query parameters</span></span>
<span data-ttu-id="9601e-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9601e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9601e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9601e-122">Request headers</span></span>
|<span data-ttu-id="9601e-123">标头</span><span class="sxs-lookup"><span data-stu-id="9601e-123">Header</span></span>|<span data-ttu-id="9601e-124">值</span><span class="sxs-lookup"><span data-stu-id="9601e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9601e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9601e-125">Authorization</span></span>|<span data-ttu-id="9601e-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9601e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9601e-127">接受</span><span class="sxs-lookup"><span data-stu-id="9601e-127">Accept</span></span>|<span data-ttu-id="9601e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9601e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9601e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9601e-129">Request body</span></span>
<span data-ttu-id="9601e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9601e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9601e-131">响应</span><span class="sxs-lookup"><span data-stu-id="9601e-131">Response</span></span>
<span data-ttu-id="9601e-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9601e-132">If successful, this method returns a `200 OK` response code and [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9601e-133">示例</span><span class="sxs-lookup"><span data-stu-id="9601e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9601e-134">请求</span><span class="sxs-lookup"><span data-stu-id="9601e-134">Request</span></span>
<span data-ttu-id="9601e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9601e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="9601e-136">响应</span><span class="sxs-lookup"><span data-stu-id="9601e-136">Response</span></span>
<span data-ttu-id="9601e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9601e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1003

{
  "value": {
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
}
```






