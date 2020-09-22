---
title: List agreementAcceptances
description: 检索用户的 agreementAcceptance 对象列表。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d27b78dff3902b86c62239df6a996f682a86fa11
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017083"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="8007d-103">List agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="8007d-103">List agreementAcceptances</span></span>

<span data-ttu-id="8007d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8007d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8007d-105">检索用户的 [agreementAcceptance](../resources/agreementacceptance.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="8007d-105">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="8007d-106">权限</span><span class="sxs-lookup"><span data-stu-id="8007d-106">Permissions</span></span>
<span data-ttu-id="8007d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8007d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8007d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8007d-109">Permission type</span></span>                        | <span data-ttu-id="8007d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8007d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8007d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8007d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8007d-112">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="8007d-112">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="8007d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8007d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8007d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8007d-114">Not supported.</span></span> |
|<span data-ttu-id="8007d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8007d-115">Application</span></span>                            | <span data-ttu-id="8007d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8007d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8007d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8007d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="8007d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8007d-118">Request headers</span></span>
| <span data-ttu-id="8007d-119">名称</span><span class="sxs-lookup"><span data-stu-id="8007d-119">Name</span></span>      |<span data-ttu-id="8007d-120">说明</span><span class="sxs-lookup"><span data-stu-id="8007d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8007d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8007d-121">Authorization</span></span> | <span data-ttu-id="8007d-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="8007d-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8007d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8007d-123">Request body</span></span>
<span data-ttu-id="8007d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8007d-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8007d-125">响应</span><span class="sxs-lookup"><span data-stu-id="8007d-125">Response</span></span>
<span data-ttu-id="8007d-126">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [agreementAcceptance](../resources/agreementacceptance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8007d-126">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8007d-127">示例</span><span class="sxs-lookup"><span data-stu-id="8007d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8007d-128">请求</span><span class="sxs-lookup"><span data-stu-id="8007d-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8007d-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="8007d-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="c"></a>[<span data-ttu-id="8007d-130">C#</span><span class="sxs-lookup"><span data-stu-id="8007d-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8007d-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8007d-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8007d-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8007d-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8007d-133">响应</span><span class="sxs-lookup"><span data-stu-id="8007d-133">Response</span></span>
><span data-ttu-id="8007d-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8007d-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


