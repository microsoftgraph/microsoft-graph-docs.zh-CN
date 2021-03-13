---
title: synchronizationJob： validateCredentials
description: 验证凭据在租户中是否有效。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ce507c989ee842040787c77f772d6188d9444a03
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50773555"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="7576e-103">synchronizationJob： validateCredentials</span><span class="sxs-lookup"><span data-stu-id="7576e-103">synchronizationJob: validateCredentials</span></span>

<span data-ttu-id="7576e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7576e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7576e-105">验证凭据在租户中是否有效。</span><span class="sxs-lookup"><span data-stu-id="7576e-105">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="7576e-106">权限</span><span class="sxs-lookup"><span data-stu-id="7576e-106">Permissions</span></span>
<span data-ttu-id="7576e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7576e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7576e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7576e-109">Permission type</span></span>                        | <span data-ttu-id="7576e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7576e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7576e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7576e-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="7576e-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7576e-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7576e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7576e-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7576e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7576e-114">Not supported.</span></span> |
|<span data-ttu-id="7576e-115">Application</span><span class="sxs-lookup"><span data-stu-id="7576e-115">Application</span></span>                            |<span data-ttu-id="7576e-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7576e-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7576e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7576e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="7576e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7576e-118">Request headers</span></span>
| <span data-ttu-id="7576e-119">名称</span><span class="sxs-lookup"><span data-stu-id="7576e-119">Name</span></span>       | <span data-ttu-id="7576e-120">说明</span><span class="sxs-lookup"><span data-stu-id="7576e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7576e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7576e-121">Authorization</span></span>  | <span data-ttu-id="7576e-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7576e-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7576e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7576e-123">Request body</span></span>
<span data-ttu-id="7576e-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7576e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7576e-125">参数</span><span class="sxs-lookup"><span data-stu-id="7576e-125">Parameter</span></span>    | <span data-ttu-id="7576e-126">类型</span><span class="sxs-lookup"><span data-stu-id="7576e-126">Type</span></span>   |<span data-ttu-id="7576e-127">说明</span><span class="sxs-lookup"><span data-stu-id="7576e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7576e-128">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="7576e-128">useSavedCredentials</span></span>|<span data-ttu-id="7576e-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="7576e-129">Boolean</span></span>|<span data-ttu-id="7576e-130">When `true` ， the parameter will be ignored and the previously saved `credentials` credentials (if any) will be validated instead.</span><span class="sxs-lookup"><span data-stu-id="7576e-130">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="7576e-131">credentials</span><span class="sxs-lookup"><span data-stu-id="7576e-131">credentials</span></span>|<span data-ttu-id="7576e-132">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7576e-132">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="7576e-133">要验证的凭据。</span><span class="sxs-lookup"><span data-stu-id="7576e-133">Credentials to validate.</span></span> <span data-ttu-id="7576e-134">当参数为 时 `useSavedCredentials` 忽略 `true` 。</span><span class="sxs-lookup"><span data-stu-id="7576e-134">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="7576e-135">响应</span><span class="sxs-lookup"><span data-stu-id="7576e-135">Response</span></span>
<span data-ttu-id="7576e-136">如果验证成功，此方法将返回 响应 `204, No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="7576e-136">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="7576e-137">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7576e-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7576e-138">示例</span><span class="sxs-lookup"><span data-stu-id="7576e-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7576e-139">请求</span><span class="sxs-lookup"><span data-stu-id="7576e-139">Request</span></span>
<span data-ttu-id="7576e-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7576e-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7576e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="7576e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationjob_validatecredentials"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials
Content-type: application/json
Content-length: 218

{ 
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="7576e-142">C#</span><span class="sxs-lookup"><span data-stu-id="7576e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7576e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7576e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7576e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7576e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7576e-145">Java</span><span class="sxs-lookup"><span data-stu-id="7576e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-validatecredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7576e-146">响应</span><span class="sxs-lookup"><span data-stu-id="7576e-146">Response</span></span>
<span data-ttu-id="7576e-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7576e-147">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob: validateCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


