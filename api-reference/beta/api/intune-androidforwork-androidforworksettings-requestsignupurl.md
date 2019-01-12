---
title: requestSignupUrl 操作
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 901d0bb67fa5992aa0931afc70660c22cd5ffeca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980039"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="f867c-103">requestSignupUrl 操作</span><span class="sxs-lookup"><span data-stu-id="f867c-103">requestSignupUrl action</span></span>

> <span data-ttu-id="f867c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f867c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f867c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f867c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f867c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f867c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f867c-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f867c-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f867c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f867c-108">Prerequisites</span></span>
<span data-ttu-id="f867c-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f867c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f867c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f867c-111">Permission type</span></span>|<span data-ttu-id="f867c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f867c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f867c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f867c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f867c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f867c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f867c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f867c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f867c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f867c-116">Not supported.</span></span>|
|<span data-ttu-id="f867c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f867c-117">Application</span></span>|<span data-ttu-id="f867c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f867c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f867c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f867c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="f867c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f867c-120">Request headers</span></span>
|<span data-ttu-id="f867c-121">标头</span><span class="sxs-lookup"><span data-stu-id="f867c-121">Header</span></span>|<span data-ttu-id="f867c-122">值</span><span class="sxs-lookup"><span data-stu-id="f867c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f867c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f867c-123">Authorization</span></span>|<span data-ttu-id="f867c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f867c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f867c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f867c-125">Accept</span></span>|<span data-ttu-id="f867c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f867c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f867c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f867c-127">Request body</span></span>
<span data-ttu-id="f867c-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f867c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f867c-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f867c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f867c-130">属性</span><span class="sxs-lookup"><span data-stu-id="f867c-130">Property</span></span>|<span data-ttu-id="f867c-131">类型</span><span class="sxs-lookup"><span data-stu-id="f867c-131">Type</span></span>|<span data-ttu-id="f867c-132">说明</span><span class="sxs-lookup"><span data-stu-id="f867c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f867c-133">hostName</span><span class="sxs-lookup"><span data-stu-id="f867c-133">hostName</span></span>|<span data-ttu-id="f867c-134">String</span><span class="sxs-lookup"><span data-stu-id="f867c-134">String</span></span>|<span data-ttu-id="f867c-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f867c-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="f867c-136">响应</span><span class="sxs-lookup"><span data-stu-id="f867c-136">Response</span></span>
<span data-ttu-id="f867c-137">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="f867c-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f867c-138">示例</span><span class="sxs-lookup"><span data-stu-id="f867c-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="f867c-139">请求</span><span class="sxs-lookup"><span data-stu-id="f867c-139">Request</span></span>
<span data-ttu-id="f867c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f867c-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="f867c-141">响应</span><span class="sxs-lookup"><span data-stu-id="f867c-141">Response</span></span>
<span data-ttu-id="f867c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f867c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```





