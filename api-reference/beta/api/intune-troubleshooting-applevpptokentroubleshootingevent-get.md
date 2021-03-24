---
title: 获取 appleVppTokenTroubleshootingEvent
description: 读取 appleVppTokenTroubleshootingEvent 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a24bf61294673d741bf9d448ed300fcac496d6fc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123369"
---
# <a name="get-applevpptokentroubleshootingevent"></a><span data-ttu-id="8ed31-103">获取 appleVppTokenTroubleshootingEvent</span><span class="sxs-lookup"><span data-stu-id="8ed31-103">Get appleVppTokenTroubleshootingEvent</span></span>

<span data-ttu-id="8ed31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ed31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ed31-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ed31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ed31-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ed31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ed31-107">读取 [appleVppTokenTroubleshootingEvent 对象的属性和](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="8ed31-107">Read properties and relationships of the [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ed31-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ed31-108">Prerequisites</span></span>
<span data-ttu-id="8ed31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ed31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ed31-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ed31-111">Permission type</span></span>|<span data-ttu-id="8ed31-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ed31-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ed31-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ed31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ed31-114">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed31-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8ed31-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ed31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ed31-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ed31-116">Not supported.</span></span>|
|<span data-ttu-id="8ed31-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ed31-117">Application</span></span>|<span data-ttu-id="8ed31-118">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed31-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ed31-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ed31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ed31-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8ed31-120">Optional query parameters</span></span>
<span data-ttu-id="8ed31-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8ed31-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ed31-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ed31-122">Request headers</span></span>
|<span data-ttu-id="8ed31-123">标头</span><span class="sxs-lookup"><span data-stu-id="8ed31-123">Header</span></span>|<span data-ttu-id="8ed31-124">值</span><span class="sxs-lookup"><span data-stu-id="8ed31-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ed31-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ed31-125">Authorization</span></span>|<span data-ttu-id="8ed31-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8ed31-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ed31-127">接受</span><span class="sxs-lookup"><span data-stu-id="8ed31-127">Accept</span></span>|<span data-ttu-id="8ed31-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8ed31-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ed31-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ed31-129">Request body</span></span>
<span data-ttu-id="8ed31-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8ed31-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ed31-131">响应</span><span class="sxs-lookup"><span data-stu-id="8ed31-131">Response</span></span>
<span data-ttu-id="8ed31-132">如果成功，此方法在响应正文 `200 OK` 中返回 响应代码和 [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ed31-132">If successful, this method returns a `200 OK` response code and [appleVppTokenTroubleshootingEvent](../resources/intune-troubleshooting-applevpptokentroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ed31-133">示例</span><span class="sxs-lookup"><span data-stu-id="8ed31-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ed31-134">请求</span><span class="sxs-lookup"><span data-stu-id="8ed31-134">Request</span></span>
<span data-ttu-id="8ed31-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ed31-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="8ed31-136">响应</span><span class="sxs-lookup"><span data-stu-id="8ed31-136">Response</span></span>
<span data-ttu-id="8ed31-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ed31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




