---
title: 'synchronizationJob: validateCredentials'
description: 验证凭据在租户中是否有效。
localization_priority: Normal
ms.openlocfilehash: b533305f622ddb5249fb64727979cafb6fbbc56a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638002"
---
# <a name="synchronizationjob-validatecredentials"></a><span data-ttu-id="2f15f-103">synchronizationJob: validateCredentials</span><span class="sxs-lookup"><span data-stu-id="2f15f-103">synchronizationJob: validateCredentials</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f15f-104">验证凭据在租户中是否有效。</span><span class="sxs-lookup"><span data-stu-id="2f15f-104">Validate that the credentials are valid in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f15f-105">权限</span><span class="sxs-lookup"><span data-stu-id="2f15f-105">Permissions</span></span>
<span data-ttu-id="2f15f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f15f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f15f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f15f-108">Permission type</span></span>                        | <span data-ttu-id="2f15f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f15f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f15f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f15f-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="2f15f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f15f-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2f15f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f15f-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2f15f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f15f-113">Not supported.</span></span> |
|<span data-ttu-id="2f15f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f15f-114">Application</span></span>                            |<span data-ttu-id="2f15f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f15f-115">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="2f15f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f15f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials

```
## <a name="request-headers"></a><span data-ttu-id="2f15f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f15f-117">Request headers</span></span>
| <span data-ttu-id="2f15f-118">名称</span><span class="sxs-lookup"><span data-stu-id="2f15f-118">Name</span></span>       | <span data-ttu-id="2f15f-119">说明</span><span class="sxs-lookup"><span data-stu-id="2f15f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2f15f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f15f-120">Authorization</span></span>  | <span data-ttu-id="2f15f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2f15f-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f15f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f15f-122">Request body</span></span>
<span data-ttu-id="2f15f-123">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2f15f-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f15f-124">参数</span><span class="sxs-lookup"><span data-stu-id="2f15f-124">Parameter</span></span>    | <span data-ttu-id="2f15f-125">类型</span><span class="sxs-lookup"><span data-stu-id="2f15f-125">Type</span></span>   |<span data-ttu-id="2f15f-126">说明</span><span class="sxs-lookup"><span data-stu-id="2f15f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f15f-127">useSavedCredentials</span><span class="sxs-lookup"><span data-stu-id="2f15f-127">useSavedCredentials</span></span>|<span data-ttu-id="2f15f-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f15f-128">Boolean</span></span>|<span data-ttu-id="2f15f-129">时`true`, 将`credentials`忽略该参数, 而改为验证以前保存的凭据 (如果有)。</span><span class="sxs-lookup"><span data-stu-id="2f15f-129">When `true`, the `credentials` parameter will be ignored and the previously saved credentials (if any) will be validated instead.</span></span> |
|<span data-ttu-id="2f15f-130">凭据</span><span class="sxs-lookup"><span data-stu-id="2f15f-130">credentials</span></span>|<span data-ttu-id="2f15f-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="2f15f-131">[synchronizationSecretKeyStringValuePair](../resources/synchronization-secretkeystringvaluepair.md) collection</span></span>|<span data-ttu-id="2f15f-132">要验证的凭据。</span><span class="sxs-lookup"><span data-stu-id="2f15f-132">Credentials to validate.</span></span> <span data-ttu-id="2f15f-133">当`useSavedCredentials`参数为`true`时忽略。</span><span class="sxs-lookup"><span data-stu-id="2f15f-133">Ignored when the `useSavedCredentials` parameter is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="2f15f-134">响应</span><span class="sxs-lookup"><span data-stu-id="2f15f-134">Response</span></span>
<span data-ttu-id="2f15f-135">如果验证成功, 此方法将`204, No Content`返回响应代码。</span><span class="sxs-lookup"><span data-stu-id="2f15f-135">If validation is successful, this method returns a `204, No Content` response code.</span></span> <span data-ttu-id="2f15f-136">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2f15f-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f15f-137">示例</span><span class="sxs-lookup"><span data-stu-id="2f15f-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2f15f-138">请求</span><span class="sxs-lookup"><span data-stu-id="2f15f-138">Request</span></span>
<span data-ttu-id="2f15f-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f15f-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2f15f-140">响应</span><span class="sxs-lookup"><span data-stu-id="2f15f-140">Response</span></span>
<span data-ttu-id="2f15f-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2f15f-141">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2f15f-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="2f15f-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2f15f-143">语言</span><span class="sxs-lookup"><span data-stu-id="2f15f-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f15f-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="2f15f-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationjob_validatecredentials-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationjob-validatecredentials.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
