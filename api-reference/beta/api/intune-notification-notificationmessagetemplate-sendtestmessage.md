---
title: sendTestMessage 操作
description: 使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fe44c931b6962766c9daba1db85dce0354c717d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147052"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="b1407-103">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="b1407-103">sendTestMessage action</span></span>

> <span data-ttu-id="b1407-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1407-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1407-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1407-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1407-106">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="b1407-106">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1407-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1407-107">Prerequisites</span></span>
<span data-ttu-id="b1407-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b1407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b1407-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1407-110">Permission type</span></span>|<span data-ttu-id="b1407-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1407-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1407-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1407-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1407-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1407-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b1407-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1407-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1407-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1407-115">Not supported.</span></span>|
|<span data-ttu-id="b1407-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1407-116">Application</span></span>|<span data-ttu-id="b1407-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1407-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1407-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1407-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="b1407-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1407-119">Request headers</span></span>
|<span data-ttu-id="b1407-120">标头</span><span class="sxs-lookup"><span data-stu-id="b1407-120">Header</span></span>|<span data-ttu-id="b1407-121">值</span><span class="sxs-lookup"><span data-stu-id="b1407-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1407-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1407-122">Authorization</span></span>|<span data-ttu-id="b1407-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1407-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1407-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b1407-124">Accept</span></span>|<span data-ttu-id="b1407-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1407-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1407-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1407-126">Request body</span></span>
<span data-ttu-id="b1407-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1407-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1407-128">响应</span><span class="sxs-lookup"><span data-stu-id="b1407-128">Response</span></span>
<span data-ttu-id="b1407-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b1407-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1407-130">示例</span><span class="sxs-lookup"><span data-stu-id="b1407-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1407-131">请求</span><span class="sxs-lookup"><span data-stu-id="b1407-131">Request</span></span>
<span data-ttu-id="b1407-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1407-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="b1407-133">响应</span><span class="sxs-lookup"><span data-stu-id="b1407-133">Response</span></span>
<span data-ttu-id="b1407-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1407-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




