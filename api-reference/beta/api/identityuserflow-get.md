---
title: 获取 userFlow
description: 检索 userflow 对象的属性和关系。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce54eb6ea71cf1396a8aedcde9478737f75d2c21
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446441"
---
# <a name="get-userflow"></a><span data-ttu-id="01f0f-103">获取 userFlow</span><span class="sxs-lookup"><span data-stu-id="01f0f-103">Get userFlow</span></span>

<span data-ttu-id="01f0f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="01f0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01f0f-105">检索[userFlow](../resources/identityuserflow.md)对象的属性和关联。</span><span class="sxs-lookup"><span data-stu-id="01f0f-105">Retrieve the properties and associations for an [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="01f0f-106">权限</span><span class="sxs-lookup"><span data-stu-id="01f0f-106">Permissions</span></span>

<span data-ttu-id="01f0f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01f0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="01f0f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="01f0f-109">Permission type</span></span>                        | <span data-ttu-id="01f0f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01f0f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="01f0f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01f0f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="01f0f-112">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="01f0f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="01f0f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01f0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01f0f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="01f0f-114">Not supported.</span></span> |
| <span data-ttu-id="01f0f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="01f0f-115">Application</span></span>                            | <span data-ttu-id="01f0f-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="01f0f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01f0f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01f0f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="01f0f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="01f0f-118">Request headers</span></span>

| <span data-ttu-id="01f0f-119">名称</span><span class="sxs-lookup"><span data-stu-id="01f0f-119">Name</span></span>      |<span data-ttu-id="01f0f-120">说明</span><span class="sxs-lookup"><span data-stu-id="01f0f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01f0f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f0f-121">Authorization</span></span> | <span data-ttu-id="01f0f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01f0f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01f0f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="01f0f-124">Content-type</span></span> | <span data-ttu-id="01f0f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="01f0f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01f0f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="01f0f-127">Request body</span></span>

<span data-ttu-id="01f0f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01f0f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01f0f-129">响应</span><span class="sxs-lookup"><span data-stu-id="01f0f-129">Response</span></span>

<span data-ttu-id="01f0f-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[userFlow](../resources/identityuserflow.md)对象。</span><span class="sxs-lookup"><span data-stu-id="01f0f-130">If successful, this method returns a `200 OK` response code and the requested [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01f0f-131">示例</span><span class="sxs-lookup"><span data-stu-id="01f0f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01f0f-132">请求</span><span class="sxs-lookup"><span data-stu-id="01f0f-132">Request</span></span>

<span data-ttu-id="01f0f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="01f0f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="01f0f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="01f0f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows/B2C_1_Pol1
```
# <a name="c"></a>[<span data-ttu-id="01f0f-135">C#</span><span class="sxs-lookup"><span data-stu-id="01f0f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01f0f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01f0f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01f0f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01f0f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01f0f-138">响应</span><span class="sxs-lookup"><span data-stu-id="01f0f-138">Response</span></span>

<span data-ttu-id="01f0f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="01f0f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="01f0f-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="01f0f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 200 OK
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
  "description": "Get UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
   "suppressions": [
    "Error: get_identityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
