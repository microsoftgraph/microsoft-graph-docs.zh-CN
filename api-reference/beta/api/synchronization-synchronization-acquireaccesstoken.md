---
title: 同步： acquireAccessToken
description: 获取 OAuth 访问令牌以授权 Azure AD 预配服务将用户预配到应用程序
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e507fd975a71bfd6a9b8dd0809d0041a7e07493b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975875"
---
# <a name="acquireaccesstoken"></a><span data-ttu-id="11c3a-103">acquireAccessToken</span><span class="sxs-lookup"><span data-stu-id="11c3a-103">acquireAccessToken</span></span>
<span data-ttu-id="11c3a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11c3a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11c3a-105">获取 OAuth 访问令牌以授权 Azure AD 预配服务将用户预配到应用程序中。</span><span class="sxs-lookup"><span data-stu-id="11c3a-105">Acquire an OAuth Access token to authorize the Azure AD provisioning service to provision users into an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="11c3a-106">权限</span><span class="sxs-lookup"><span data-stu-id="11c3a-106">Permissions</span></span>
<span data-ttu-id="11c3a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11c3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11c3a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="11c3a-109">Permission type</span></span>|<span data-ttu-id="11c3a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="11c3a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11c3a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11c3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11c3a-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11c3a-112">Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="11c3a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11c3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11c3a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="11c3a-114">Not supported.</span></span>|
|<span data-ttu-id="11c3a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="11c3a-115">Application</span></span>|<span data-ttu-id="11c3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="11c3a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11c3a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11c3a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /applications/{applicationsId}/synchronization/acquireAccessToken
POST /servicePrincipals/{servicePrincipalsId}/synchronization/acquireAccessToken
```

## <a name="request-headers"></a><span data-ttu-id="11c3a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="11c3a-118">Request headers</span></span>
|<span data-ttu-id="11c3a-119">名称</span><span class="sxs-lookup"><span data-stu-id="11c3a-119">Name</span></span>|<span data-ttu-id="11c3a-120">说明</span><span class="sxs-lookup"><span data-stu-id="11c3a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="11c3a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11c3a-121">Authorization</span></span>|<span data-ttu-id="11c3a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11c3a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="11c3a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11c3a-124">Content-Type</span></span>|<span data-ttu-id="11c3a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="11c3a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11c3a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="11c3a-127">Request body</span></span>
<span data-ttu-id="11c3a-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11c3a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="11c3a-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="11c3a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="11c3a-130">参数</span><span class="sxs-lookup"><span data-stu-id="11c3a-130">Parameter</span></span>|<span data-ttu-id="11c3a-131">类型</span><span class="sxs-lookup"><span data-stu-id="11c3a-131">Type</span></span>|<span data-ttu-id="11c3a-132">说明</span><span class="sxs-lookup"><span data-stu-id="11c3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11c3a-133">凭据</span><span class="sxs-lookup"><span data-stu-id="11c3a-133">credentials</span></span>|<span data-ttu-id="11c3a-134">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="11c3a-134">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="11c3a-135">表示单个机密值。</span><span class="sxs-lookup"><span data-stu-id="11c3a-135">Represents a single secret value.</span></span>|



## <a name="response"></a><span data-ttu-id="11c3a-136">响应</span><span class="sxs-lookup"><span data-stu-id="11c3a-136">Response</span></span>

<span data-ttu-id="11c3a-137">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="11c3a-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="11c3a-138">示例</span><span class="sxs-lookup"><span data-stu-id="11c3a-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11c3a-139">请求</span><span class="sxs-lookup"><span data-stu-id="11c3a-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="11c3a-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="11c3a-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronization_acquireaccesstoken"
}
-->
``` http
POST https://graph.microsoft.com/beta/applications/{applicationsId}/synchronization/acquireAccessToken
Content-Type: application/json
Content-length: 123

{
  "credentials": [
    {
      "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="11c3a-141">C#</span><span class="sxs-lookup"><span data-stu-id="11c3a-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronization-acquireaccesstoken-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11c3a-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11c3a-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronization-acquireaccesstoken-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11c3a-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11c3a-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronization-acquireaccesstoken-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11c3a-144">Java</span><span class="sxs-lookup"><span data-stu-id="11c3a-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronization-acquireaccesstoken-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="11c3a-145">响应</span><span class="sxs-lookup"><span data-stu-id="11c3a-145">Response</span></span>
<span data-ttu-id="11c3a-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="11c3a-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


