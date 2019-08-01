---
title: 列出 localizedNotificationMessages
description: 列出 localizedNotificationMessage 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0cafe0e84266d03ce4d5d52bf2d9e40af67a3e02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018125"
---
# <a name="list-localizednotificationmessages"></a><span data-ttu-id="a6f9f-103">列出 localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="a6f9f-103">List localizedNotificationMessages</span></span>

> <span data-ttu-id="a6f9f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6f9f-105">列出 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-105">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6f9f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a6f9f-106">Prerequisites</span></span>
<span data-ttu-id="a6f9f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6f9f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6f9f-109">Permission type</span></span>|<span data-ttu-id="a6f9f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a6f9f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6f9f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6f9f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6f9f-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6f9f-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a6f9f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6f9f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6f9f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-114">Not supported.</span></span>|
|<span data-ttu-id="a6f9f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6f9f-115">Application</span></span>|<span data-ttu-id="a6f9f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6f9f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6f9f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="a6f9f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6f9f-118">Request headers</span></span>
|<span data-ttu-id="a6f9f-119">标头</span><span class="sxs-lookup"><span data-stu-id="a6f9f-119">Header</span></span>|<span data-ttu-id="a6f9f-120">值</span><span class="sxs-lookup"><span data-stu-id="a6f9f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6f9f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6f9f-121">Authorization</span></span>|<span data-ttu-id="a6f9f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6f9f-123">接受</span><span class="sxs-lookup"><span data-stu-id="a6f9f-123">Accept</span></span>|<span data-ttu-id="a6f9f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a6f9f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6f9f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6f9f-125">Request body</span></span>
<span data-ttu-id="a6f9f-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6f9f-127">响应</span><span class="sxs-lookup"><span data-stu-id="a6f9f-127">Response</span></span>
<span data-ttu-id="a6f9f-128">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-128">If successful, this method returns a `200 OK` response code and a collection of [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6f9f-129">示例</span><span class="sxs-lookup"><span data-stu-id="a6f9f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6f9f-130">请求</span><span class="sxs-lookup"><span data-stu-id="a6f9f-130">Request</span></span>
<span data-ttu-id="a6f9f-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

### <a name="response"></a><span data-ttu-id="a6f9f-132">响应</span><span class="sxs-lookup"><span data-stu-id="a6f9f-132">Response</span></span>
<span data-ttu-id="a6f9f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a6f9f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.localizedNotificationMessage",
      "id": "7a777708-7708-7a77-0877-777a0877777a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "locale": "Locale value",
      "subject": "Subject value",
      "messageTemplate": "Message Template value",
      "isDefault": true
    }
  ]
}
```



