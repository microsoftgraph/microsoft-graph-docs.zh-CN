---
title: 创建 userFlow
description: 使用此 API 创建新的 userFlow。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3ed41278c913361f22d8df3f2ac34ce50c69d2ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435299"
---
# <a name="create-userflow"></a><span data-ttu-id="6b2bf-103">创建 userFlow</span><span class="sxs-lookup"><span data-stu-id="6b2bf-103">Create userFlow</span></span>

<span data-ttu-id="6b2bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b2bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b2bf-105">创建新的 [userFlow](../resources/identityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b2bf-105">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b2bf-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6b2bf-106">Permissions</span></span>

<span data-ttu-id="6b2bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b2bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b2bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b2bf-109">Permission type</span></span>                        | <span data-ttu-id="6b2bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b2bf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6b2bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b2bf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b2bf-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b2bf-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="6b2bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b2bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b2bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b2bf-114">Not supported.</span></span> |
| <span data-ttu-id="6b2bf-115">Application</span><span class="sxs-lookup"><span data-stu-id="6b2bf-115">Application</span></span>                            | <span data-ttu-id="6b2bf-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b2bf-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b2bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b2bf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="6b2bf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b2bf-118">Request headers</span></span>

| <span data-ttu-id="6b2bf-119">名称</span><span class="sxs-lookup"><span data-stu-id="6b2bf-119">Name</span></span>          | <span data-ttu-id="6b2bf-120">说明</span><span class="sxs-lookup"><span data-stu-id="6b2bf-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6b2bf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b2bf-121">Authorization</span></span> | <span data-ttu-id="6b2bf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b2bf-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="6b2bf-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="6b2bf-124">Content-type</span></span> | <span data-ttu-id="6b2bf-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6b2bf-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b2bf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b2bf-127">Request body</span></span>

<span data-ttu-id="6b2bf-128">在请求正文中，提供 [userFlow](../resources/identityuserflow.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b2bf-128">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6b2bf-129">响应</span><span class="sxs-lookup"><span data-stu-id="6b2bf-129">Response</span></span>

<span data-ttu-id="6b2bf-130">如果成功，此方法在响应正文中返回响应 `201 Created` 代码和新 [userFlow](../resources/identityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b2bf-130">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b2bf-131">示例</span><span class="sxs-lookup"><span data-stu-id="6b2bf-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6b2bf-132">请求</span><span class="sxs-lookup"><span data-stu-id="6b2bf-132">Request</span></span>

<span data-ttu-id="6b2bf-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b2bf-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b2bf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b2bf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_identitycontainer"
}-->

```http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-type: application/json

{
  "id": "Pol1",
  "userFlowType": "signUpOrSignIn",
  "userFlowTypeVersion": 1
}
```
# <a name="c"></a>[<span data-ttu-id="6b2bf-135">C#</span><span class="sxs-lookup"><span data-stu-id="6b2bf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b2bf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b2bf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b2bf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b2bf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b2bf-138">Java</span><span class="sxs-lookup"><span data-stu-id="6b2bf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflow-from-identitycontainer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6b2bf-139">响应</span><span class="sxs-lookup"><span data-stu-id="6b2bf-139">Response</span></span>

<span data-ttu-id="6b2bf-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6b2bf-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6b2bf-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6b2bf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "B2C_1_Pol1",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_identityuserflow_from_identitycontainer/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


