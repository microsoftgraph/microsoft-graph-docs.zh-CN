---
title: sync 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8075d8ff03e37f8a6ba33913c30caf4e09fd842
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943030"
---
# <a name="sync-action"></a><span data-ttu-id="bbfb6-103">sync 操作</span><span class="sxs-lookup"><span data-stu-id="bbfb6-103">sync action</span></span>

> <span data-ttu-id="bbfb6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbfb6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bbfb6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbfb6-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="bbfb6-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbfb6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbfb6-108">Prerequisites</span></span>
<span data-ttu-id="bbfb6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bbfb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbfb6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbfb6-111">Permission type</span></span>|<span data-ttu-id="bbfb6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bbfb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbfb6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbfb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bbfb6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbfb6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bbfb6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbfb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbfb6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-116">Not supported.</span></span>|
|<span data-ttu-id="bbfb6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbfb6-117">Application</span></span>|<span data-ttu-id="bbfb6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbfb6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbfb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="bbfb6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbfb6-120">Request headers</span></span>
|<span data-ttu-id="bbfb6-121">标头</span><span class="sxs-lookup"><span data-stu-id="bbfb6-121">Header</span></span>|<span data-ttu-id="bbfb6-122">值</span><span class="sxs-lookup"><span data-stu-id="bbfb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbfb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbfb6-123">Authorization</span></span>|<span data-ttu-id="bbfb6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbfb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bbfb6-125">Accept</span></span>|<span data-ttu-id="bbfb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bbfb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbfb6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbfb6-127">Request body</span></span>
<span data-ttu-id="bbfb6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbfb6-129">响应</span><span class="sxs-lookup"><span data-stu-id="bbfb6-129">Response</span></span>
<span data-ttu-id="bbfb6-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bbfb6-131">示例</span><span class="sxs-lookup"><span data-stu-id="bbfb6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbfb6-132">请求</span><span class="sxs-lookup"><span data-stu-id="bbfb6-132">Request</span></span>
<span data-ttu-id="bbfb6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="bbfb6-134">响应</span><span class="sxs-lookup"><span data-stu-id="bbfb6-134">Response</span></span>
<span data-ttu-id="bbfb6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbfb6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





