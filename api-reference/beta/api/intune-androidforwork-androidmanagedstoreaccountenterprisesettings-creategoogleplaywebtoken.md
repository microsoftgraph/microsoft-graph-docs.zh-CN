---
title: createGooglePlayWebToken 操作
description: 生成嵌入组件中使用的 web 标记。
author: tfitzmac
ms.openlocfilehash: 206113b445d8b190e02b292dd661bc3c207de288
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338540"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="63b28-103">createGooglePlayWebToken 操作</span><span class="sxs-lookup"><span data-stu-id="63b28-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="63b28-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="63b28-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63b28-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63b28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63b28-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="63b28-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63b28-107">生成嵌入组件中使用的 web 标记。</span><span class="sxs-lookup"><span data-stu-id="63b28-107">Generates a web token that is used in an embeddable component.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63b28-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="63b28-108">Prerequisites</span></span>
<span data-ttu-id="63b28-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="63b28-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63b28-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="63b28-111">Permission type</span></span>|<span data-ttu-id="63b28-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63b28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63b28-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63b28-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63b28-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63b28-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63b28-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63b28-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63b28-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="63b28-116">Not supported.</span></span>|
|<span data-ttu-id="63b28-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="63b28-117">Application</span></span>|<span data-ttu-id="63b28-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="63b28-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63b28-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63b28-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="63b28-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="63b28-120">Request headers</span></span>
|<span data-ttu-id="63b28-121">标头</span><span class="sxs-lookup"><span data-stu-id="63b28-121">Header</span></span>|<span data-ttu-id="63b28-122">值</span><span class="sxs-lookup"><span data-stu-id="63b28-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63b28-123">授权</span><span class="sxs-lookup"><span data-stu-id="63b28-123">Authorization</span></span>|<span data-ttu-id="63b28-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="63b28-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63b28-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63b28-125">Accept</span></span>|<span data-ttu-id="63b28-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63b28-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63b28-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="63b28-127">Request body</span></span>
<span data-ttu-id="63b28-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63b28-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="63b28-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="63b28-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="63b28-130">属性</span><span class="sxs-lookup"><span data-stu-id="63b28-130">Property</span></span>|<span data-ttu-id="63b28-131">类型</span><span class="sxs-lookup"><span data-stu-id="63b28-131">Type</span></span>|<span data-ttu-id="63b28-132">说明</span><span class="sxs-lookup"><span data-stu-id="63b28-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63b28-133">parentUri</span><span class="sxs-lookup"><span data-stu-id="63b28-133">parentUri</span></span>|<span data-ttu-id="63b28-134">字符串</span><span class="sxs-lookup"><span data-stu-id="63b28-134">String</span></span>|<span data-ttu-id="63b28-135">承载组件页上的 https 路径。</span><span class="sxs-lookup"><span data-stu-id="63b28-135">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="63b28-136">响应</span><span class="sxs-lookup"><span data-stu-id="63b28-136">Response</span></span>
<span data-ttu-id="63b28-137">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和一个 String。</span><span class="sxs-lookup"><span data-stu-id="63b28-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63b28-138">示例</span><span class="sxs-lookup"><span data-stu-id="63b28-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="63b28-139">请求</span><span class="sxs-lookup"><span data-stu-id="63b28-139">Request</span></span>
<span data-ttu-id="63b28-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="63b28-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="63b28-141">响应</span><span class="sxs-lookup"><span data-stu-id="63b28-141">Response</span></span>
<span data-ttu-id="63b28-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63b28-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```





