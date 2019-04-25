---
title: 删除 localizedNotificationMessage
description: 删除 localizedNotificationMessage。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47df5ab32e3e80d4ab3666784a29c9d2b078a82d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561766"
---
# <a name="delete-localizednotificationmessage"></a><span data-ttu-id="76337-103">删除 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="76337-103">Delete localizedNotificationMessage</span></span>

> <span data-ttu-id="76337-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76337-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76337-105">删除 [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="76337-105">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76337-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="76337-106">Prerequisites</span></span>
<span data-ttu-id="76337-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76337-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="76337-109">Permission type</span></span>|<span data-ttu-id="76337-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="76337-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76337-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76337-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76337-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76337-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="76337-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76337-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76337-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="76337-114">Not supported.</span></span>|
|<span data-ttu-id="76337-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="76337-115">Application</span></span>|<span data-ttu-id="76337-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="76337-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76337-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76337-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="76337-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="76337-118">Request headers</span></span>
|<span data-ttu-id="76337-119">标头</span><span class="sxs-lookup"><span data-stu-id="76337-119">Header</span></span>|<span data-ttu-id="76337-120">值</span><span class="sxs-lookup"><span data-stu-id="76337-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76337-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="76337-121">Authorization</span></span>|<span data-ttu-id="76337-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76337-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76337-123">接受</span><span class="sxs-lookup"><span data-stu-id="76337-123">Accept</span></span>|<span data-ttu-id="76337-124">application/json</span><span class="sxs-lookup"><span data-stu-id="76337-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76337-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="76337-125">Request body</span></span>
<span data-ttu-id="76337-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76337-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76337-127">响应</span><span class="sxs-lookup"><span data-stu-id="76337-127">Response</span></span>
<span data-ttu-id="76337-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="76337-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76337-129">示例</span><span class="sxs-lookup"><span data-stu-id="76337-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="76337-130">请求</span><span class="sxs-lookup"><span data-stu-id="76337-130">Request</span></span>
<span data-ttu-id="76337-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76337-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

### <a name="response"></a><span data-ttu-id="76337-132">响应</span><span class="sxs-lookup"><span data-stu-id="76337-132">Response</span></span>
<span data-ttu-id="76337-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76337-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



