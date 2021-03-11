---
title: List agreementAcceptances
description: 检索用户 agreementAcceptance 对象的列表。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: b0bc9630d503847832b8fb3ab73e8064fa90c96c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720058"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="1f2b3-103">List agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="1f2b3-103">List agreementAcceptances</span></span>

<span data-ttu-id="1f2b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f2b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f2b3-105">检索用户 [agreementAcceptance](../resources/agreementacceptance.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1f2b3-105">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1f2b3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="1f2b3-106">Permissions</span></span>
<span data-ttu-id="1f2b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f2b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f2b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f2b3-109">Permission type</span></span>                        | <span data-ttu-id="1f2b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f2b3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f2b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f2b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f2b3-112">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="1f2b3-112">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="1f2b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f2b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f2b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f2b3-114">Not supported.</span></span> |
|<span data-ttu-id="1f2b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f2b3-115">Application</span></span>                            | <span data-ttu-id="1f2b3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f2b3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f2b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f2b3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="1f2b3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f2b3-118">Request headers</span></span>
| <span data-ttu-id="1f2b3-119">名称</span><span class="sxs-lookup"><span data-stu-id="1f2b3-119">Name</span></span>      |<span data-ttu-id="1f2b3-120">说明</span><span class="sxs-lookup"><span data-stu-id="1f2b3-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1f2b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f2b3-121">Authorization</span></span> | <span data-ttu-id="1f2b3-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="1f2b3-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f2b3-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f2b3-123">Request body</span></span>
<span data-ttu-id="1f2b3-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f2b3-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1f2b3-125">响应</span><span class="sxs-lookup"><span data-stu-id="1f2b3-125">Response</span></span>
<span data-ttu-id="1f2b3-126">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [agreementAcceptance](../resources/agreementacceptance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1f2b3-126">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1f2b3-127">示例</span><span class="sxs-lookup"><span data-stu-id="1f2b3-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1f2b3-128">请求</span><span class="sxs-lookup"><span data-stu-id="1f2b3-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1f2b3-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f2b3-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="c"></a>[<span data-ttu-id="1f2b3-130">C#</span><span class="sxs-lookup"><span data-stu-id="1f2b3-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f2b3-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f2b3-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f2b3-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f2b3-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f2b3-133">Java</span><span class="sxs-lookup"><span data-stu-id="1f2b3-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreementacceptances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1f2b3-134">响应</span><span class="sxs-lookup"><span data-stu-id="1f2b3-134">Response</span></span>
><span data-ttu-id="1f2b3-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1f2b3-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
