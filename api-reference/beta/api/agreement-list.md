---
title: 列出协议
description: 检索协议对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 8d636cab5663633ba78e76057dc9ba3d555fbdc4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942887"
---
# <a name="list-agreements"></a><span data-ttu-id="c8a16-103">列出协议</span><span class="sxs-lookup"><span data-stu-id="c8a16-103">List agreements</span></span>

<span data-ttu-id="c8a16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8a16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8a16-105">检索协议 [对象](../resources/agreement.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="c8a16-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8a16-106">权限</span><span class="sxs-lookup"><span data-stu-id="c8a16-106">Permissions</span></span>
<span data-ttu-id="c8a16-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8a16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8a16-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8a16-109">Permission type</span></span>                        | <span data-ttu-id="c8a16-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8a16-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8a16-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8a16-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8a16-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8a16-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="c8a16-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8a16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8a16-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8a16-114">Not supported.</span></span> |
|<span data-ttu-id="c8a16-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8a16-115">Application</span></span>                            | <span data-ttu-id="c8a16-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8a16-116">Not supported.</span></span> |

<span data-ttu-id="c8a16-117">代表用户进行呼叫时，用户需要属于以下目录角色之一。</span><span class="sxs-lookup"><span data-stu-id="c8a16-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="c8a16-118">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="c8a16-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="c8a16-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="c8a16-119">Global Administrator</span></span>
+ <span data-ttu-id="c8a16-120">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="c8a16-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="c8a16-121">安全管理员</span><span class="sxs-lookup"><span data-stu-id="c8a16-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c8a16-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8a16-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="c8a16-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8a16-123">Request headers</span></span>
| <span data-ttu-id="c8a16-124">名称</span><span class="sxs-lookup"><span data-stu-id="c8a16-124">Name</span></span>         | <span data-ttu-id="c8a16-125">类型</span><span class="sxs-lookup"><span data-stu-id="c8a16-125">Type</span></span>        | <span data-ttu-id="c8a16-126">说明</span><span class="sxs-lookup"><span data-stu-id="c8a16-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c8a16-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8a16-127">Authorization</span></span> | <span data-ttu-id="c8a16-128">string</span><span class="sxs-lookup"><span data-stu-id="c8a16-128">string</span></span> | <span data-ttu-id="c8a16-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8a16-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8a16-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8a16-131">Request body</span></span>
<span data-ttu-id="c8a16-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c8a16-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c8a16-133">响应</span><span class="sxs-lookup"><span data-stu-id="c8a16-133">Response</span></span>
<span data-ttu-id="c8a16-134">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码 [和 agreement](../resources/agreement.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c8a16-134">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8a16-135">示例</span><span class="sxs-lookup"><span data-stu-id="c8a16-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8a16-136">请求</span><span class="sxs-lookup"><span data-stu-id="c8a16-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c8a16-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8a16-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
```
# <a name="c"></a>[<span data-ttu-id="c8a16-138">C#</span><span class="sxs-lookup"><span data-stu-id="c8a16-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8a16-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8a16-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8a16-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8a16-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8a16-141">Java</span><span class="sxs-lookup"><span data-stu-id="c8a16-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c8a16-142">响应</span><span class="sxs-lookup"><span data-stu-id="c8a16-142">Response</span></span>
><span data-ttu-id="c8a16-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c8a16-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
