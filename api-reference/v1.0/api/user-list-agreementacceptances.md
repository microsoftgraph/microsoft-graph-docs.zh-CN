---
title: List agreementAcceptances
description: 检索用户 agreementAcceptance 对象的列表。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d922160488b3a87fcf8fbf57d42acdba12b87701
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948658"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="4ef9a-103">List agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="4ef9a-103">List agreementAcceptances</span></span>

<span data-ttu-id="4ef9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ef9a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ef9a-105">检索用户 [agreementAcceptance 对象](../resources/agreementacceptance.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="4ef9a-105">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ef9a-106">权限</span><span class="sxs-lookup"><span data-stu-id="4ef9a-106">Permissions</span></span>
<span data-ttu-id="4ef9a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ef9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ef9a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ef9a-109">Permission type</span></span>                        | <span data-ttu-id="4ef9a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ef9a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ef9a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ef9a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ef9a-112">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="4ef9a-112">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="4ef9a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ef9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ef9a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ef9a-114">Not supported.</span></span> |
|<span data-ttu-id="4ef9a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ef9a-115">Application</span></span>                            | <span data-ttu-id="4ef9a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ef9a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ef9a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ef9a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/agreementAcceptances
GET /users/{id | userPrincipalName}/agreementAcceptances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ef9a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ef9a-118">Optional query parameters</span></span>
<span data-ttu-id="4ef9a-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4ef9a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ef9a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ef9a-120">Request headers</span></span>
| <span data-ttu-id="4ef9a-121">名称</span><span class="sxs-lookup"><span data-stu-id="4ef9a-121">Name</span></span>      |<span data-ttu-id="4ef9a-122">说明</span><span class="sxs-lookup"><span data-stu-id="4ef9a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4ef9a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ef9a-123">Authorization</span></span> | <span data-ttu-id="4ef9a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ef9a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ef9a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ef9a-126">Request body</span></span>
<span data-ttu-id="4ef9a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ef9a-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4ef9a-128">响应</span><span class="sxs-lookup"><span data-stu-id="4ef9a-128">Response</span></span>
<span data-ttu-id="4ef9a-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [agreementAcceptance](../resources/agreementacceptance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4ef9a-129">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ef9a-130">示例</span><span class="sxs-lookup"><span data-stu-id="4ef9a-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="4ef9a-131">请求</span><span class="sxs-lookup"><span data-stu-id="4ef9a-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4ef9a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ef9a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/agreementAcceptances

GET https://graph.microsoft.com/v1.0/users/f2f4f8e9-c99d-4c73-b990-34f81fbf7fcf/agreementAcceptances
```
# <a name="c"></a>[<span data-ttu-id="4ef9a-133">C#</span><span class="sxs-lookup"><span data-stu-id="4ef9a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ef9a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ef9a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ef9a-135">Java</span><span class="sxs-lookup"><span data-stu-id="4ef9a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreementacceptances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4ef9a-136">响应</span><span class="sxs-lookup"><span data-stu-id="4ef9a-136">Response</span></span>
><span data-ttu-id="4ef9a-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ef9a-137">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
      "agreementId": "093b947f-8363-4979-a47d-4c52b33ee1be",
      "userId": "f2f4f8e9-c99d-4c73-b990-34f81fbf7fcf",
      "agreementFileId": "f2f4f8e9-c99d-4c73-b990-34f81fbf7fcf",
      "recordedDateTime": "2021-03-10T00:39:56.0523527Z",
      "userDisplayName": "Test_User",
      "userPrincipalName": "Test_User@TestTenant.onmicrosoft.com"
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
