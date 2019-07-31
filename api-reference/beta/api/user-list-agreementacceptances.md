---
title: List agreementAcceptances
description: 检索用户的 agreementAcceptance 对象列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eb55aaaccd9fe5db3e7c8929c28e672a4c3fa87a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996460"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="ba970-103">List agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="ba970-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba970-104">检索用户的[agreementAcceptance](../resources/agreementacceptance.md)对象列表。</span><span class="sxs-lookup"><span data-stu-id="ba970-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ba970-105">权限</span><span class="sxs-lookup"><span data-stu-id="ba970-105">Permissions</span></span>
<span data-ttu-id="ba970-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba970-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba970-108">Permission type</span></span>                        | <span data-ttu-id="ba970-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba970-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba970-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba970-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba970-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="ba970-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="ba970-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba970-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba970-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba970-113">Not supported.</span></span> |
|<span data-ttu-id="ba970-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba970-114">Application</span></span>                            | <span data-ttu-id="ba970-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba970-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba970-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba970-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="ba970-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba970-117">Request headers</span></span>
| <span data-ttu-id="ba970-118">名称</span><span class="sxs-lookup"><span data-stu-id="ba970-118">Name</span></span>      |<span data-ttu-id="ba970-119">说明</span><span class="sxs-lookup"><span data-stu-id="ba970-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba970-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba970-120">Authorization</span></span> | <span data-ttu-id="ba970-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ba970-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba970-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba970-122">Request body</span></span>
<span data-ttu-id="ba970-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba970-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ba970-124">响应</span><span class="sxs-lookup"><span data-stu-id="ba970-124">Response</span></span>
<span data-ttu-id="ba970-125">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[agreementAcceptance](../resources/agreementacceptance.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ba970-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba970-126">示例</span><span class="sxs-lookup"><span data-stu-id="ba970-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba970-127">请求</span><span class="sxs-lookup"><span data-stu-id="ba970-127">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ba970-128">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ba970-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba970-129">C#</span><span class="sxs-lookup"><span data-stu-id="ba970-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba970-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="ba970-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba970-131">目标-C</span><span class="sxs-lookup"><span data-stu-id="ba970-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ba970-132">Java</span><span class="sxs-lookup"><span data-stu-id="ba970-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreementacceptances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ba970-133">响应</span><span class="sxs-lookup"><span data-stu-id="ba970-133">Response</span></span>
><span data-ttu-id="ba970-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba970-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
