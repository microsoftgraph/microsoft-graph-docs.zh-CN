---
title: uploadDepToken 操作
description: 上载新的设备注册程序令牌
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e146ebe7d25c428c3451830eb7fa223096fff8af
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886581"
---
# <a name="uploaddeptoken-action"></a><span data-ttu-id="55492-103">uploadDepToken 操作</span><span class="sxs-lookup"><span data-stu-id="55492-103">uploadDepToken action</span></span>

> <span data-ttu-id="55492-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="55492-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55492-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="55492-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55492-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="55492-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55492-107">上载新的设备注册程序令牌</span><span class="sxs-lookup"><span data-stu-id="55492-107">Uploads a new Device Enrollment Program token</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55492-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="55492-108">Prerequisites</span></span>
<span data-ttu-id="55492-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="55492-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55492-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="55492-111">Permission type</span></span>|<span data-ttu-id="55492-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="55492-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55492-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55492-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55492-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55492-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="55492-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55492-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55492-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="55492-116">Not supported.</span></span>|
|<span data-ttu-id="55492-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="55492-117">Application</span></span>|<span data-ttu-id="55492-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="55492-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55492-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55492-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken
```

## <a name="request-headers"></a><span data-ttu-id="55492-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="55492-120">Request headers</span></span>
|<span data-ttu-id="55492-121">标头</span><span class="sxs-lookup"><span data-stu-id="55492-121">Header</span></span>|<span data-ttu-id="55492-122">值</span><span class="sxs-lookup"><span data-stu-id="55492-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55492-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55492-123">Authorization</span></span>|<span data-ttu-id="55492-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="55492-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55492-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55492-125">Accept</span></span>|<span data-ttu-id="55492-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55492-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55492-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="55492-127">Request body</span></span>
<span data-ttu-id="55492-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55492-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="55492-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="55492-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="55492-130">属性</span><span class="sxs-lookup"><span data-stu-id="55492-130">Property</span></span>|<span data-ttu-id="55492-131">类型</span><span class="sxs-lookup"><span data-stu-id="55492-131">Type</span></span>|<span data-ttu-id="55492-132">Description</span><span class="sxs-lookup"><span data-stu-id="55492-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55492-133">appleId</span><span class="sxs-lookup"><span data-stu-id="55492-133">appleId</span></span>|<span data-ttu-id="55492-134">String</span><span class="sxs-lookup"><span data-stu-id="55492-134">String</span></span>|<span data-ttu-id="55492-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="55492-135">Not yet documented</span></span>|
|<span data-ttu-id="55492-136">depToken</span><span class="sxs-lookup"><span data-stu-id="55492-136">depToken</span></span>|<span data-ttu-id="55492-137">字符串</span><span class="sxs-lookup"><span data-stu-id="55492-137">String</span></span>|<span data-ttu-id="55492-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="55492-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="55492-139">响应</span><span class="sxs-lookup"><span data-stu-id="55492-139">Response</span></span>
<span data-ttu-id="55492-140">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="55492-140">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="55492-141">示例</span><span class="sxs-lookup"><span data-stu-id="55492-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="55492-142">请求</span><span class="sxs-lookup"><span data-stu-id="55492-142">Request</span></span>
<span data-ttu-id="55492-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55492-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/uploadDepToken

Content-type: application/json
Content-length: 69

{
  "appleId": "Apple Id value",
  "depToken": "Dep Token value"
}
```

### <a name="response"></a><span data-ttu-id="55492-144">响应</span><span class="sxs-lookup"><span data-stu-id="55492-144">Response</span></span>
<span data-ttu-id="55492-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="55492-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





