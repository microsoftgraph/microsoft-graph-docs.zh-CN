---
title: servicePrincipal：removePassword
description: 从 servicePrincipal 中删除密码
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: be45dacbb123c93d7670d3f01f9b7444e561300a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134097"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="46d8b-103">servicePrincipal：removePassword</span><span class="sxs-lookup"><span data-stu-id="46d8b-103">servicePrincipal: removePassword</span></span>

<span data-ttu-id="46d8b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46d8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46d8b-105">从 [servicePrincipal 对象中删除](../resources/serviceprincipal.md) 密码。</span><span class="sxs-lookup"><span data-stu-id="46d8b-105">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46d8b-106">权限</span><span class="sxs-lookup"><span data-stu-id="46d8b-106">Permissions</span></span>

<span data-ttu-id="46d8b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46d8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46d8b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="46d8b-109">Permission type</span></span>                        | <span data-ttu-id="46d8b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46d8b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="46d8b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46d8b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="46d8b-112">Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="46d8b-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="46d8b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46d8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46d8b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="46d8b-114">Not supported.</span></span> |
| <span data-ttu-id="46d8b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="46d8b-115">Application</span></span>                            | <span data-ttu-id="46d8b-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46d8b-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46d8b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46d8b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="46d8b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="46d8b-118">Request headers</span></span>

| <span data-ttu-id="46d8b-119">名称</span><span class="sxs-lookup"><span data-stu-id="46d8b-119">Name</span></span>           | <span data-ttu-id="46d8b-120">说明</span><span class="sxs-lookup"><span data-stu-id="46d8b-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="46d8b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="46d8b-121">Authorization</span></span>  | <span data-ttu-id="46d8b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46d8b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="46d8b-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="46d8b-124">Content-type</span></span>   | <span data-ttu-id="46d8b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="46d8b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46d8b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="46d8b-127">Request body</span></span>

| <span data-ttu-id="46d8b-128">属性</span><span class="sxs-lookup"><span data-stu-id="46d8b-128">Property</span></span>     | <span data-ttu-id="46d8b-129">类型</span><span class="sxs-lookup"><span data-stu-id="46d8b-129">Type</span></span>   |<span data-ttu-id="46d8b-130">说明</span><span class="sxs-lookup"><span data-stu-id="46d8b-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="46d8b-131">keyId</span><span class="sxs-lookup"><span data-stu-id="46d8b-131">keyId</span></span> | <span data-ttu-id="46d8b-132">GUID</span><span class="sxs-lookup"><span data-stu-id="46d8b-132">GUID</span></span> | <span data-ttu-id="46d8b-133">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="46d8b-133">The unique identifier for the password.</span></span> <span data-ttu-id="46d8b-134">必需。</span><span class="sxs-lookup"><span data-stu-id="46d8b-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="46d8b-135">响应</span><span class="sxs-lookup"><span data-stu-id="46d8b-135">Response</span></span>

<span data-ttu-id="46d8b-136">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="46d8b-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="46d8b-137">示例</span><span class="sxs-lookup"><span data-stu-id="46d8b-137">Examples</span></span>

<span data-ttu-id="46d8b-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="46d8b-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="46d8b-139">请求</span><span class="sxs-lookup"><span data-stu-id="46d8b-139">Request</span></span>

<span data-ttu-id="46d8b-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="46d8b-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46d8b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="46d8b-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_removepassword"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="javascript"></a>[<span data-ttu-id="46d8b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46d8b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46d8b-143">响应</span><span class="sxs-lookup"><span data-stu-id="46d8b-143">Response</span></span>

<span data-ttu-id="46d8b-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="46d8b-144">The following is an example of the response.</span></span>

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



