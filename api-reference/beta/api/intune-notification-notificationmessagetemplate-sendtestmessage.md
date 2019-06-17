---
title: sendTestMessage 操作
description: 使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea60b10ae0ca699d0f60165f1613dddcf588e23d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963497"
---
# <a name="sendtestmessage-action"></a><span data-ttu-id="2ce59-103">sendTestMessage 操作</span><span class="sxs-lookup"><span data-stu-id="2ce59-103">sendTestMessage action</span></span>

> <span data-ttu-id="2ce59-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2ce59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ce59-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ce59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ce59-106">使用默认区域设置中指定的 notificationMessageTemplate 发送测试消息</span><span class="sxs-lookup"><span data-stu-id="2ce59-106">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ce59-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ce59-107">Prerequisites</span></span>
<span data-ttu-id="2ce59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ce59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ce59-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ce59-110">Permission type</span></span>|<span data-ttu-id="2ce59-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ce59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ce59-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ce59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ce59-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ce59-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2ce59-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ce59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ce59-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ce59-115">Not supported.</span></span>|
|<span data-ttu-id="2ce59-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ce59-116">Application</span></span>|<span data-ttu-id="2ce59-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ce59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ce59-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ce59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

## <a name="request-headers"></a><span data-ttu-id="2ce59-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ce59-119">Request headers</span></span>
|<span data-ttu-id="2ce59-120">标头</span><span class="sxs-lookup"><span data-stu-id="2ce59-120">Header</span></span>|<span data-ttu-id="2ce59-121">值</span><span class="sxs-lookup"><span data-stu-id="2ce59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ce59-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ce59-122">Authorization</span></span>|<span data-ttu-id="2ce59-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ce59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ce59-124">接受</span><span class="sxs-lookup"><span data-stu-id="2ce59-124">Accept</span></span>|<span data-ttu-id="2ce59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ce59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ce59-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ce59-126">Request body</span></span>
<span data-ttu-id="2ce59-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ce59-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ce59-128">响应</span><span class="sxs-lookup"><span data-stu-id="2ce59-128">Response</span></span>
<span data-ttu-id="2ce59-129">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2ce59-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ce59-130">示例</span><span class="sxs-lookup"><span data-stu-id="2ce59-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ce59-131">请求</span><span class="sxs-lookup"><span data-stu-id="2ce59-131">Request</span></span>
<span data-ttu-id="2ce59-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ce59-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/sendTestMessage
```

### <a name="response"></a><span data-ttu-id="2ce59-133">响应</span><span class="sxs-lookup"><span data-stu-id="2ce59-133">Response</span></span>
<span data-ttu-id="2ce59-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ce59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





