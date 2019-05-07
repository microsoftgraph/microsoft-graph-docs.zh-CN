---
title: 列出协议
description: 检索协议对象的列表。
localization_priority: Normal
ms.openlocfilehash: 3d0594f37a3d88f7ff1ba9ea543e3b2d21ebc63a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636623"
---
# <a name="list-agreements"></a><span data-ttu-id="4fd6c-103">列出协议</span><span class="sxs-lookup"><span data-stu-id="4fd6c-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fd6c-104">检索[协议](../resources/agreement.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4fd6c-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="4fd6c-105">权限</span><span class="sxs-lookup"><span data-stu-id="4fd6c-105">Permissions</span></span>
<span data-ttu-id="4fd6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fd6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fd6c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fd6c-108">Permission type</span></span>                        | <span data-ttu-id="4fd6c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fd6c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fd6c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fd6c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fd6c-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fd6c-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="4fd6c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fd6c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fd6c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fd6c-113">Not supported.</span></span> |
|<span data-ttu-id="4fd6c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fd6c-114">Application</span></span>                            | <span data-ttu-id="4fd6c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fd6c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4fd6c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fd6c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="4fd6c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fd6c-117">Request headers</span></span>
| <span data-ttu-id="4fd6c-118">名称</span><span class="sxs-lookup"><span data-stu-id="4fd6c-118">Name</span></span>         | <span data-ttu-id="4fd6c-119">类型</span><span class="sxs-lookup"><span data-stu-id="4fd6c-119">Type</span></span>        | <span data-ttu-id="4fd6c-120">说明</span><span class="sxs-lookup"><span data-stu-id="4fd6c-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4fd6c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fd6c-121">Authorization</span></span> | <span data-ttu-id="4fd6c-122">string</span><span class="sxs-lookup"><span data-stu-id="4fd6c-122">string</span></span> | <span data-ttu-id="4fd6c-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="4fd6c-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fd6c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fd6c-125">Request body</span></span>
<span data-ttu-id="4fd6c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4fd6c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4fd6c-127">响应</span><span class="sxs-lookup"><span data-stu-id="4fd6c-127">Response</span></span>
<span data-ttu-id="4fd6c-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[协议](../resources/agreement.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4fd6c-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4fd6c-129">示例</span><span class="sxs-lookup"><span data-stu-id="4fd6c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4fd6c-130">请求</span><span class="sxs-lookup"><span data-stu-id="4fd6c-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="4fd6c-131">响应</span><span class="sxs-lookup"><span data-stu-id="4fd6c-131">Response</span></span>
><span data-ttu-id="4fd6c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4fd6c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4fd6c-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4fd6c-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4fd6c-135">语言</span><span class="sxs-lookup"><span data-stu-id="4fd6c-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_agreements-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4fd6c-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="4fd6c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_agreements-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/agreement-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/agreement-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
