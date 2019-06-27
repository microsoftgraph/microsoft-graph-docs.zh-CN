---
title: List agreementAcceptances
description: 检索用户的 agreementAcceptance 对象列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8ca6788bec02713131aaa6006e4327b85e85eff0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270299"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="76f9a-103">List agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="76f9a-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76f9a-104">检索用户的[agreementAcceptance](../resources/agreementacceptance.md)对象列表。</span><span class="sxs-lookup"><span data-stu-id="76f9a-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="76f9a-105">权限</span><span class="sxs-lookup"><span data-stu-id="76f9a-105">Permissions</span></span>
<span data-ttu-id="76f9a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76f9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76f9a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="76f9a-108">Permission type</span></span>                        | <span data-ttu-id="76f9a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76f9a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="76f9a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76f9a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="76f9a-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="76f9a-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="76f9a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76f9a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76f9a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="76f9a-113">Not supported.</span></span> |
|<span data-ttu-id="76f9a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="76f9a-114">Application</span></span>                            | <span data-ttu-id="76f9a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="76f9a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76f9a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76f9a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="76f9a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="76f9a-117">Request headers</span></span>
| <span data-ttu-id="76f9a-118">名称</span><span class="sxs-lookup"><span data-stu-id="76f9a-118">Name</span></span>      |<span data-ttu-id="76f9a-119">说明</span><span class="sxs-lookup"><span data-stu-id="76f9a-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76f9a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="76f9a-120">Authorization</span></span> | <span data-ttu-id="76f9a-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="76f9a-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="76f9a-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="76f9a-122">Request body</span></span>
<span data-ttu-id="76f9a-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76f9a-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="76f9a-124">响应</span><span class="sxs-lookup"><span data-stu-id="76f9a-124">Response</span></span>
<span data-ttu-id="76f9a-125">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[agreementAcceptance](../resources/agreementacceptance.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="76f9a-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76f9a-126">示例</span><span class="sxs-lookup"><span data-stu-id="76f9a-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76f9a-127">请求</span><span class="sxs-lookup"><span data-stu-id="76f9a-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
##### <a name="response"></a><span data-ttu-id="76f9a-128">响应</span><span class="sxs-lookup"><span data-stu-id="76f9a-128">Response</span></span>
><span data-ttu-id="76f9a-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="76f9a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="76f9a-131">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="76f9a-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="76f9a-132">C#</span><span class="sxs-lookup"><span data-stu-id="76f9a-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_agreementacceptances-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76f9a-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="76f9a-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_agreementacceptances-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="76f9a-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="76f9a-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_agreementacceptances-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-agreementacceptances.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
