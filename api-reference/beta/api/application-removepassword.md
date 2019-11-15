---
title: 应用程序： removePassword
description: 删除应用程序中的密码
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6a83c1e128d319f76a4e52fad91a59193811b390
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37994950"
---
# <a name="application-removepassword"></a><span data-ttu-id="1b23d-103">应用程序： removePassword</span><span class="sxs-lookup"><span data-stu-id="1b23d-103">application: removePassword</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b23d-104">从[应用程序](../resources/application.md)中删除密码。</span><span class="sxs-lookup"><span data-stu-id="1b23d-104">Removes a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1b23d-105">权限</span><span class="sxs-lookup"><span data-stu-id="1b23d-105">Permissions</span></span>

<span data-ttu-id="1b23d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b23d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b23d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b23d-108">Permission type</span></span>                        | <span data-ttu-id="1b23d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b23d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1b23d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b23d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b23d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b23d-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1b23d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b23d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b23d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b23d-113">Not supported.</span></span> |
| <span data-ttu-id="1b23d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b23d-114">Application</span></span>                            | <span data-ttu-id="1b23d-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1b23d-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b23d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b23d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="1b23d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b23d-117">Request headers</span></span>

| <span data-ttu-id="1b23d-118">名称</span><span class="sxs-lookup"><span data-stu-id="1b23d-118">Name</span></span>           | <span data-ttu-id="1b23d-119">说明</span><span class="sxs-lookup"><span data-stu-id="1b23d-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="1b23d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b23d-120">Authorization</span></span>  | <span data-ttu-id="1b23d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b23d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1b23d-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="1b23d-123">Content-type</span></span>   | <span data-ttu-id="1b23d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1b23d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b23d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b23d-126">Request body</span></span>

| <span data-ttu-id="1b23d-127">属性</span><span class="sxs-lookup"><span data-stu-id="1b23d-127">Property</span></span>  | <span data-ttu-id="1b23d-128">类型</span><span class="sxs-lookup"><span data-stu-id="1b23d-128">Type</span></span> | <span data-ttu-id="1b23d-129">说明</span><span class="sxs-lookup"><span data-stu-id="1b23d-129">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="1b23d-130">keyId</span><span class="sxs-lookup"><span data-stu-id="1b23d-130">keyId</span></span>     | <span data-ttu-id="1b23d-131">GUID</span><span class="sxs-lookup"><span data-stu-id="1b23d-131">GUID</span></span> | <span data-ttu-id="1b23d-132">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1b23d-132">The unique identifier for the password.</span></span> <span data-ttu-id="1b23d-133">必需。</span><span class="sxs-lookup"><span data-stu-id="1b23d-133">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1b23d-134">响应</span><span class="sxs-lookup"><span data-stu-id="1b23d-134">Response</span></span>

<span data-ttu-id="1b23d-135">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1b23d-135">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1b23d-136">示例</span><span class="sxs-lookup"><span data-stu-id="1b23d-136">Examples</span></span>

<span data-ttu-id="1b23d-137">下面的示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1b23d-137">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1b23d-138">请求</span><span class="sxs-lookup"><span data-stu-id="1b23d-138">Request</span></span>

<span data-ttu-id="1b23d-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b23d-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b23d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b23d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removepassword"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b23d-141">C#</span><span class="sxs-lookup"><span data-stu-id="1b23d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b23d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b23d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b23d-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b23d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b23d-144">响应</span><span class="sxs-lookup"><span data-stu-id="1b23d-144">Response</span></span>

<span data-ttu-id="1b23d-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b23d-145">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
