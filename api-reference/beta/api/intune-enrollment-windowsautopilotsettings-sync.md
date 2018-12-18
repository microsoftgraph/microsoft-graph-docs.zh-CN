---
title: sync 操作
description: 尚未记录
author: tfitzmac
ms.openlocfilehash: fd6814c99b188e6c0e8859d7035a533ce6d0b0e3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332576"
---
# <a name="sync-action"></a><span data-ttu-id="91eee-103">sync 操作</span><span class="sxs-lookup"><span data-stu-id="91eee-103">sync action</span></span>

> <span data-ttu-id="91eee-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="91eee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91eee-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="91eee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91eee-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="91eee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91eee-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="91eee-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91eee-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="91eee-108">Prerequisites</span></span>
<span data-ttu-id="91eee-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="91eee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91eee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="91eee-111">Permission type</span></span>|<span data-ttu-id="91eee-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="91eee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91eee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91eee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91eee-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91eee-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="91eee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91eee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91eee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="91eee-116">Not supported.</span></span>|
|<span data-ttu-id="91eee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="91eee-117">Application</span></span>|<span data-ttu-id="91eee-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="91eee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91eee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91eee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotSettings/sync
```

## <a name="request-headers"></a><span data-ttu-id="91eee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="91eee-120">Request headers</span></span>
|<span data-ttu-id="91eee-121">标头</span><span class="sxs-lookup"><span data-stu-id="91eee-121">Header</span></span>|<span data-ttu-id="91eee-122">值</span><span class="sxs-lookup"><span data-stu-id="91eee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91eee-123">授权</span><span class="sxs-lookup"><span data-stu-id="91eee-123">Authorization</span></span>|<span data-ttu-id="91eee-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="91eee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91eee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="91eee-125">Accept</span></span>|<span data-ttu-id="91eee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91eee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91eee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="91eee-127">Request body</span></span>
<span data-ttu-id="91eee-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91eee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91eee-129">响应</span><span class="sxs-lookup"><span data-stu-id="91eee-129">Response</span></span>
<span data-ttu-id="91eee-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="91eee-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="91eee-131">示例</span><span class="sxs-lookup"><span data-stu-id="91eee-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="91eee-132">请求</span><span class="sxs-lookup"><span data-stu-id="91eee-132">Request</span></span>
<span data-ttu-id="91eee-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91eee-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings/sync
```

### <a name="response"></a><span data-ttu-id="91eee-134">响应</span><span class="sxs-lookup"><span data-stu-id="91eee-134">Response</span></span>
<span data-ttu-id="91eee-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91eee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





