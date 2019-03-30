---
title: sendTestMessage 操作
description: 使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01426ef13ae875af474b5ec57721d51adc288f71
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987725"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="7eeea-103">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="7eeea-103">sendTestMessage action</span></span>

> <span data-ttu-id="7eeea-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7eeea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7eeea-105">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="7eeea-105">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7eeea-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7eeea-106">Prerequisites</span></span>
<span data-ttu-id="7eeea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7eeea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eeea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7eeea-109">Permission type</span></span>|<span data-ttu-id="7eeea-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7eeea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7eeea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7eeea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7eeea-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eeea-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7eeea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7eeea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7eeea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7eeea-114">Not supported.</span></span>|
|<span data-ttu-id="7eeea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7eeea-115">Application</span></span>|<span data-ttu-id="7eeea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7eeea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7eeea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7eeea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="7eeea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7eeea-118">Request headers</span></span>
|<span data-ttu-id="7eeea-119">标头</span><span class="sxs-lookup"><span data-stu-id="7eeea-119">Header</span></span>|<span data-ttu-id="7eeea-120">值</span><span class="sxs-lookup"><span data-stu-id="7eeea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7eeea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7eeea-121">Authorization</span></span>|<span data-ttu-id="7eeea-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7eeea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7eeea-123">接受</span><span class="sxs-lookup"><span data-stu-id="7eeea-123">Accept</span></span>|<span data-ttu-id="7eeea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7eeea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7eeea-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7eeea-125">Request body</span></span>
<span data-ttu-id="7eeea-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7eeea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eeea-127">响应</span><span class="sxs-lookup"><span data-stu-id="7eeea-127">Response</span></span>
<span data-ttu-id="7eeea-128">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7eeea-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7eeea-129">示例</span><span class="sxs-lookup"><span data-stu-id="7eeea-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7eeea-130">请求</span><span class="sxs-lookup"><span data-stu-id="7eeea-130">Request</span></span>
<span data-ttu-id="7eeea-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7eeea-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="7eeea-132">响应</span><span class="sxs-lookup"><span data-stu-id="7eeea-132">Response</span></span>
<span data-ttu-id="7eeea-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7eeea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



