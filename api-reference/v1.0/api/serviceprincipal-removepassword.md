---
title: servicePrincipal： removePassword
description: 从 servicePrincipal 中删除密码
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 937feb0e414f1e3a6263bc2e54e440898431d130
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383922"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="50f28-103">servicePrincipal： removePassword</span><span class="sxs-lookup"><span data-stu-id="50f28-103">servicePrincipal: removePassword</span></span>

<span data-ttu-id="50f28-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50f28-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50f28-105">从[servicePrincipal](../resources/serviceprincipal.md)对象中删除密码。</span><span class="sxs-lookup"><span data-stu-id="50f28-105">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="50f28-106">权限</span><span class="sxs-lookup"><span data-stu-id="50f28-106">Permissions</span></span>

<span data-ttu-id="50f28-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50f28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50f28-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="50f28-109">Permission type</span></span>                        | <span data-ttu-id="50f28-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50f28-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="50f28-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50f28-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="50f28-112">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="50f28-112">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="50f28-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50f28-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50f28-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="50f28-114">Not supported.</span></span> |
| <span data-ttu-id="50f28-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="50f28-115">Application</span></span>                            | <span data-ttu-id="50f28-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="50f28-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50f28-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50f28-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="50f28-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="50f28-118">Request headers</span></span>

| <span data-ttu-id="50f28-119">名称</span><span class="sxs-lookup"><span data-stu-id="50f28-119">Name</span></span>           | <span data-ttu-id="50f28-120">说明</span><span class="sxs-lookup"><span data-stu-id="50f28-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="50f28-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50f28-121">Authorization</span></span>  | <span data-ttu-id="50f28-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50f28-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50f28-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="50f28-124">Content-type</span></span>   | <span data-ttu-id="50f28-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="50f28-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50f28-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="50f28-127">Request body</span></span>

| <span data-ttu-id="50f28-128">属性</span><span class="sxs-lookup"><span data-stu-id="50f28-128">Property</span></span>     | <span data-ttu-id="50f28-129">类型</span><span class="sxs-lookup"><span data-stu-id="50f28-129">Type</span></span>   |<span data-ttu-id="50f28-130">Description</span><span class="sxs-lookup"><span data-stu-id="50f28-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="50f28-131">keyId</span><span class="sxs-lookup"><span data-stu-id="50f28-131">keyId</span></span> | <span data-ttu-id="50f28-132">GUID</span><span class="sxs-lookup"><span data-stu-id="50f28-132">GUID</span></span> | <span data-ttu-id="50f28-133">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="50f28-133">The unique identifier for the password.</span></span> <span data-ttu-id="50f28-134">必需。</span><span class="sxs-lookup"><span data-stu-id="50f28-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="50f28-135">响应</span><span class="sxs-lookup"><span data-stu-id="50f28-135">Response</span></span>

<span data-ttu-id="50f28-136">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="50f28-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="50f28-137">示例</span><span class="sxs-lookup"><span data-stu-id="50f28-137">Examples</span></span>

<span data-ttu-id="50f28-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="50f28-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="50f28-139">请求</span><span class="sxs-lookup"><span data-stu-id="50f28-139">Request</span></span>

<span data-ttu-id="50f28-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="50f28-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="50f28-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="50f28-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_removepassword"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="c"></a>[<span data-ttu-id="50f28-142">C#</span><span class="sxs-lookup"><span data-stu-id="50f28-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-removepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50f28-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50f28-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50f28-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50f28-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-removepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50f28-145">Java</span><span class="sxs-lookup"><span data-stu-id="50f28-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-removepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50f28-146">响应</span><span class="sxs-lookup"><span data-stu-id="50f28-146">Response</span></span>

<span data-ttu-id="50f28-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="50f28-147">The following is an example of the response.</span></span>

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
  "description": "servicePrincipal: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
