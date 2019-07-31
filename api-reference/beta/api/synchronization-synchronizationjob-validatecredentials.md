---
title: 'synchronizationJob: validateCredentials'
description: 验证凭据在租户中是否有效。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c12f2d810841fb3f168e1196d466f6162ad4e1a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982697"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="7a08b-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="7a08b-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a08b-104">验证凭据在租户中是否有效。</span><span class="sxs-lookup"><span data-stu-id="7a08b-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a08b-105">权限</span><span class="sxs-lookup"><span data-stu-id="7a08b-105">Permissions</span></span>
<span data-ttu-id="7a08b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a08b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a08b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a08b-108">Permission type</span></span>                        | <span data-ttu-id="7a08b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a08b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a08b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a08b-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="7a08b-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a08b-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7a08b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a08b-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7a08b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a08b-113">Not supported.</span></span> |
|<span data-ttu-id="7a08b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a08b-114">Application</span></span>                            |<span data-ttu-id="7a08b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a08b-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="7a08b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a08b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="7a08b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a08b-117">Request headers</span></span>
| <span data-ttu-id="7a08b-118">名称</span><span class="sxs-lookup"><span data-stu-id="7a08b-118">Name</span></span>       | <span data-ttu-id="7a08b-119">说明</span><span class="sxs-lookup"><span data-stu-id="7a08b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7a08b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a08b-120">Authorization</span></span>  | <span data-ttu-id="7a08b-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7a08b-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a08b-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a08b-122">Request body</span></span>
<span data-ttu-id="7a08b-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7a08b-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7a08b-124">参数</span><span class="sxs-lookup"><span data-stu-id="7a08b-124">Parameter</span></span>    | <span data-ttu-id="7a08b-125">类型</span><span class="sxs-lookup"><span data-stu-id="7a08b-125">Type</span></span>   |<span data-ttu-id="7a08b-126">说明</span><span class="sxs-lookup"><span data-stu-id="7a08b-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a08b-127">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="7a08b-127">useSavedCredentials</span></span>|<span data-ttu-id="7a08b-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a08b-128">Boolean</span></span>|<span data-ttu-id="7a08b-129">时`true`, 将`credentials`忽略该参数, 而改为验证以前保存的凭据 (如果有)。</span><span class="sxs-lookup"><span data-stu-id="7a08b-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="7a08b-130">凭据</span><span class="sxs-lookup"><span data-stu-id="7a08b-130">credentials</span></span>|<span data-ttu-id="7a08b-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="7a08b-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="7a08b-132">要验证的凭据。</span><span class="sxs-lookup"><span data-stu-id="7a08b-132">Credentials to validate.</span></span> <span data-ttu-id="7a08b-133">当`useSavedCredentials`参数为`true`时忽略。</span><span class="sxs-lookup"><span data-stu-id="7a08b-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="7a08b-134">响应</span><span class="sxs-lookup"><span data-stu-id="7a08b-134">Response</span></span>
<span data-ttu-id="7a08b-135">如果验证成功, 此方法将`204, No Content`返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="7a08b-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="7a08b-136">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7a08b-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a08b-137">示例</span><span class="sxs-lookup"><span data-stu-id="7a08b-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7a08b-138">请求</span><span class="sxs-lookup"><span data-stu-id="7a08b-138">Request</span></span>
<span data-ttu-id="7a08b-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7a08b-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a08b-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7a08b-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a08b-141">C#</span><span class="sxs-lookup"><span data-stu-id="7a08b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationjob-validatecredentials-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a08b-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a08b-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationjob-validatecredentials-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a08b-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="7a08b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationjob-validatecredentials-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a08b-144">Java</span><span class="sxs-lookup"><span data-stu-id="7a08b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationjob-validatecredentials-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7a08b-145">响应</span><span class="sxs-lookup"><span data-stu-id="7a08b-145">Response</span></span>
<span data-ttu-id="7a08b-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7a08b-146">The following is an example of the response.</span></span> 
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
