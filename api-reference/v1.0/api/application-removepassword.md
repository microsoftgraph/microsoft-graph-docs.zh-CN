---
title: application： removePassword
description: 从应用程序中删除密码
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: cfe32e9743bbae164065416adfa1873431a1bb51
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787973"
---
# <a name="application-removepassword"></a><span data-ttu-id="6597e-103">application： removePassword</span><span class="sxs-lookup"><span data-stu-id="6597e-103">application: removePassword</span></span>

<span data-ttu-id="6597e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6597e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6597e-105">从应用程序中删除 [密码](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="6597e-105">Remove a password from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6597e-106">权限</span><span class="sxs-lookup"><span data-stu-id="6597e-106">Permissions</span></span>

<span data-ttu-id="6597e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6597e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6597e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6597e-109">Permission type</span></span>                        | <span data-ttu-id="6597e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6597e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6597e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6597e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6597e-112">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6597e-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="6597e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6597e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6597e-114">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6597e-114">Application.ReadWrite.All</span></span> |
| <span data-ttu-id="6597e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6597e-115">Application</span></span>                            | <span data-ttu-id="6597e-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6597e-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6597e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6597e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="6597e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6597e-118">Request headers</span></span>

| <span data-ttu-id="6597e-119">名称</span><span class="sxs-lookup"><span data-stu-id="6597e-119">Name</span></span>           | <span data-ttu-id="6597e-120">说明</span><span class="sxs-lookup"><span data-stu-id="6597e-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6597e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6597e-121">Authorization</span></span>  | <span data-ttu-id="6597e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6597e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6597e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6597e-124">Content-Type</span></span>   | <span data-ttu-id="6597e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6597e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6597e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6597e-127">Request body</span></span>

| <span data-ttu-id="6597e-128">属性</span><span class="sxs-lookup"><span data-stu-id="6597e-128">Property</span></span>  | <span data-ttu-id="6597e-129">类型</span><span class="sxs-lookup"><span data-stu-id="6597e-129">Type</span></span> | <span data-ttu-id="6597e-130">说明</span><span class="sxs-lookup"><span data-stu-id="6597e-130">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="6597e-131">keyId</span><span class="sxs-lookup"><span data-stu-id="6597e-131">keyId</span></span>     | <span data-ttu-id="6597e-132">GUID</span><span class="sxs-lookup"><span data-stu-id="6597e-132">GUID</span></span> | <span data-ttu-id="6597e-133">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6597e-133">The unique identifier for the password.</span></span> <span data-ttu-id="6597e-134">必需。</span><span class="sxs-lookup"><span data-stu-id="6597e-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6597e-135">响应</span><span class="sxs-lookup"><span data-stu-id="6597e-135">Response</span></span>

<span data-ttu-id="6597e-136">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6597e-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6597e-137">示例</span><span class="sxs-lookup"><span data-stu-id="6597e-137">Examples</span></span>

<span data-ttu-id="6597e-138">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6597e-138">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6597e-139">请求</span><span class="sxs-lookup"><span data-stu-id="6597e-139">Request</span></span>

<span data-ttu-id="6597e-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6597e-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6597e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="6597e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removepassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="c"></a>[<span data-ttu-id="6597e-142">C#</span><span class="sxs-lookup"><span data-stu-id="6597e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6597e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6597e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6597e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6597e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6597e-145">Java</span><span class="sxs-lookup"><span data-stu-id="6597e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6597e-146">响应</span><span class="sxs-lookup"><span data-stu-id="6597e-146">Response</span></span>

<span data-ttu-id="6597e-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6597e-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
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

