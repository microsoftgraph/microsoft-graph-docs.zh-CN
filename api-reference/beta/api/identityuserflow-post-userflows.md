---
title: 创建 userFlow
description: 使用此 API 创建新的 userFlow。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1cd660e4be738469351e3d1369d557774895ac58
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938556"
---
# <a name="create-userflow"></a><span data-ttu-id="9fee3-103">创建 userFlow</span><span class="sxs-lookup"><span data-stu-id="9fee3-103">Create userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fee3-104">创建新的[userFlow](../resources/identityuserflow.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9fee3-104">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fee3-105">权限</span><span class="sxs-lookup"><span data-stu-id="9fee3-105">Permissions</span></span>

<span data-ttu-id="9fee3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fee3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9fee3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fee3-108">Permission type</span></span>                        | <span data-ttu-id="9fee3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fee3-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9fee3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fee3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9fee3-111">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="9fee3-111">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="9fee3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fee3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fee3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9fee3-113">Not supported.</span></span> |
| <span data-ttu-id="9fee3-114">Application</span><span class="sxs-lookup"><span data-stu-id="9fee3-114">Application</span></span>                            | <span data-ttu-id="9fee3-115">IdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="9fee3-115">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fee3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fee3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="9fee3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fee3-117">Request headers</span></span>

| <span data-ttu-id="9fee3-118">名称</span><span class="sxs-lookup"><span data-stu-id="9fee3-118">Name</span></span>          | <span data-ttu-id="9fee3-119">说明</span><span class="sxs-lookup"><span data-stu-id="9fee3-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9fee3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fee3-120">Authorization</span></span> | <span data-ttu-id="9fee3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9fee3-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9fee3-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="9fee3-123">Content-type</span></span> | <span data-ttu-id="9fee3-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9fee3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fee3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fee3-126">Request body</span></span>

<span data-ttu-id="9fee3-127">在请求正文中，提供[userFlow](../resources/identityuserflow.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9fee3-127">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9fee3-128">响应</span><span class="sxs-lookup"><span data-stu-id="9fee3-128">Response</span></span>

<span data-ttu-id="9fee3-129">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[userFlow](../resources/identityuserflow.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9fee3-129">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9fee3-130">示例</span><span class="sxs-lookup"><span data-stu-id="9fee3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9fee3-131">请求</span><span class="sxs-lookup"><span data-stu-id="9fee3-131">Request</span></span>

<span data-ttu-id="9fee3-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9fee3-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9fee3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fee3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_identitycontainer"
}-->

```http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-type: application/json

{
  "userFlowType": "signUpOrSignIn",
  "userFlowTypeVersion": 1
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9fee3-134">C#</span><span class="sxs-lookup"><span data-stu-id="9fee3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fee3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fee3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9fee3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fee3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9fee3-137">响应</span><span class="sxs-lookup"><span data-stu-id="9fee3-137">Response</span></span>

<span data-ttu-id="9fee3-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9fee3-138">The following is an example of the response.</span></span>

> <span data-ttu-id="9fee3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9fee3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
