---
title: 创建 authenticationContextClassReference
description: 创建新的 authenticationContextClassReference。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4646e8a388800587c0aa73a736d591dc6b97c6fb
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663938"
---
# <a name="create-authenticationcontextclassreference"></a><span data-ttu-id="60cdd-103">创建 authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="60cdd-103">Create authenticationContextClassReference</span></span>

<span data-ttu-id="60cdd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60cdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60cdd-105">创建新的 [authenticationContextClassReference](../resources/authenticationContextClassReference.md)。</span><span class="sxs-lookup"><span data-stu-id="60cdd-105">Create a new [authenticationContextClassReference](../resources/authenticationContextClassReference.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="60cdd-106">权限</span><span class="sxs-lookup"><span data-stu-id="60cdd-106">Permissions</span></span>

<span data-ttu-id="60cdd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60cdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60cdd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="60cdd-109">Permission type</span></span>                        | <span data-ttu-id="60cdd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60cdd-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="60cdd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60cdd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="60cdd-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="60cdd-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="60cdd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60cdd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60cdd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="60cdd-114">Not supported.</span></span> |
|<span data-ttu-id="60cdd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="60cdd-115">Application</span></span>                            | <span data-ttu-id="60cdd-116">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="60cdd-116">Policy.ReadWrite.ConditionalAccess</span></span> |

> [!NOTE]
> <span data-ttu-id="60cdd-117">此 API 有 [一个与](/graph/known-issues#permissions) 权限相关的已知问题。</span><span class="sxs-lookup"><span data-stu-id="60cdd-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="60cdd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60cdd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/conditionalAccess/authenticationContextClassReferences
```

## <a name="request-headers"></a><span data-ttu-id="60cdd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="60cdd-119">Request headers</span></span>

| <span data-ttu-id="60cdd-120">名称</span><span class="sxs-lookup"><span data-stu-id="60cdd-120">Name</span></span>          | <span data-ttu-id="60cdd-121">说明</span><span class="sxs-lookup"><span data-stu-id="60cdd-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="60cdd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60cdd-122">Authorization</span></span> | <span data-ttu-id="60cdd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="60cdd-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="60cdd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60cdd-125">Content-Type</span></span>  | <span data-ttu-id="60cdd-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="60cdd-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60cdd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="60cdd-128">Request body</span></span>

<span data-ttu-id="60cdd-129">在请求正文中，提供 [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60cdd-129">In the request body, supply a JSON representation of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="60cdd-130">响应</span><span class="sxs-lookup"><span data-stu-id="60cdd-130">Response</span></span>

<span data-ttu-id="60cdd-131">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60cdd-131">If successful, this method returns a `201 Created` response code and a new [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60cdd-132">示例</span><span class="sxs-lookup"><span data-stu-id="60cdd-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60cdd-133">请求</span><span class="sxs-lookup"><span data-stu-id="60cdd-133">Request</span></span>
<span data-ttu-id="60cdd-134">以下示例显示创建可供应用使用的新 authenticationcontextclassreference。</span><span class="sxs-lookup"><span data-stu-id="60cdd-134">The following example shows creating a new authenticationcontextclassreference that is available for apps to use.</span></span>




# <a name="http"></a>[<span data-ttu-id="60cdd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="60cdd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_authenticationcontextclassreference"
}-->

```http
POST https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
Content-type: application/json

{
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```
# <a name="c"></a>[<span data-ttu-id="60cdd-136">C#</span><span class="sxs-lookup"><span data-stu-id="60cdd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-authenticationcontextclassreference-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60cdd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60cdd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-authenticationcontextclassreference-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60cdd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60cdd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-authenticationcontextclassreference-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60cdd-139">Java</span><span class="sxs-lookup"><span data-stu-id="60cdd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-authenticationcontextclassreference-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="60cdd-140">响应</span><span class="sxs-lookup"><span data-stu-id="60cdd-140">Response</span></span>

<span data-ttu-id="60cdd-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="60cdd-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReference/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": true
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
