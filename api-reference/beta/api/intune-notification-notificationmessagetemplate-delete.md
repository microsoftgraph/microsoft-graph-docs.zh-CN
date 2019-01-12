---
title: 删除 notificationMessageTemplate
description: 删除 notificationMessageTemplate。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2fdd00ad49d335905a8fa3e68489964c9b9c8010
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940881"
---
# <a name="delete-notificationmessagetemplate"></a><span data-ttu-id="9d382-103">删除 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="9d382-103">Delete notificationMessageTemplate</span></span>

> <span data-ttu-id="9d382-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9d382-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d382-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d382-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d382-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9d382-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d382-107">删除 [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="9d382-107">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d382-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9d382-108">Prerequisites</span></span>
<span data-ttu-id="9d382-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9d382-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d382-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d382-111">Permission type</span></span>|<span data-ttu-id="9d382-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9d382-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d382-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d382-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d382-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d382-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9d382-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d382-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d382-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d382-116">Not supported.</span></span>|
|<span data-ttu-id="9d382-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d382-117">Application</span></span>|<span data-ttu-id="9d382-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d382-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d382-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d382-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

## <a name="request-headers"></a><span data-ttu-id="9d382-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d382-120">Request headers</span></span>
|<span data-ttu-id="9d382-121">标头</span><span class="sxs-lookup"><span data-stu-id="9d382-121">Header</span></span>|<span data-ttu-id="9d382-122">值</span><span class="sxs-lookup"><span data-stu-id="9d382-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d382-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d382-123">Authorization</span></span>|<span data-ttu-id="9d382-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9d382-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d382-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d382-125">Accept</span></span>|<span data-ttu-id="9d382-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d382-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d382-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d382-127">Request body</span></span>
<span data-ttu-id="9d382-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9d382-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d382-129">响应</span><span class="sxs-lookup"><span data-stu-id="9d382-129">Response</span></span>
<span data-ttu-id="9d382-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9d382-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9d382-131">示例</span><span class="sxs-lookup"><span data-stu-id="9d382-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d382-132">请求</span><span class="sxs-lookup"><span data-stu-id="9d382-132">Request</span></span>
<span data-ttu-id="9d382-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d382-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}
```

### <a name="response"></a><span data-ttu-id="9d382-134">响应</span><span class="sxs-lookup"><span data-stu-id="9d382-134">Response</span></span>
<span data-ttu-id="9d382-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9d382-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





