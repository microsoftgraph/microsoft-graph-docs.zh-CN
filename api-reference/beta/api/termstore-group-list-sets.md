---
title: 列表集
description: 获取 set 对象及其属性的列表。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: f4d35decdae3303576565e2844206c7bfe16cf23
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330264"
---
# <a name="list-sets"></a><span data-ttu-id="f9775-103">列表集</span><span class="sxs-lookup"><span data-stu-id="f9775-103">List sets</span></span>
<span data-ttu-id="f9775-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="f9775-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9775-105">获取 [set](../resources/termstore-set.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="f9775-105">Get a list of the [set](../resources/termstore-set.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9775-106">权限</span><span class="sxs-lookup"><span data-stu-id="f9775-106">Permissions</span></span>
<span data-ttu-id="f9775-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9775-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9775-109">Permission type</span></span>|<span data-ttu-id="f9775-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9775-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9775-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9775-111">Delegated (work or school account)</span></span> |<span data-ttu-id="f9775-112">TermStore、TermStore 和所有</span><span class="sxs-lookup"><span data-stu-id="f9775-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="f9775-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9775-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9775-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9775-114">Not supported.</span></span>    |
|<span data-ttu-id="f9775-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9775-115">Application</span></span> | <span data-ttu-id="f9775-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9775-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9775-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9775-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}/sets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9775-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f9775-118">Optional query parameters</span></span>
<span data-ttu-id="f9775-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f9775-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f9775-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f9775-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9775-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9775-121">Request headers</span></span>
|<span data-ttu-id="f9775-122">名称</span><span class="sxs-lookup"><span data-stu-id="f9775-122">Name</span></span>|<span data-ttu-id="f9775-123">说明</span><span class="sxs-lookup"><span data-stu-id="f9775-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f9775-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9775-124">Authorization</span></span>|<span data-ttu-id="f9775-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9775-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9775-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9775-127">Request body</span></span>
<span data-ttu-id="f9775-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9775-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9775-129">响应</span><span class="sxs-lookup"><span data-stu-id="f9775-129">Response</span></span>

<span data-ttu-id="f9775-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [set](../resources/termstore-set.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f9775-130">If successful, this method returns a `200 OK` response code and a collection of [set](../resources/termstore-set.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9775-131">示例</span><span class="sxs-lookup"><span data-stu-id="f9775-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9775-132">请求</span><span class="sxs-lookup"><span data-stu-id="f9775-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f9775-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9775-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_set"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets
```
# <a name="c"></a>[<span data-ttu-id="f9775-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9775-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9775-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9775-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9775-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9775-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f9775-137">响应</span><span class="sxs-lookup"><span data-stu-id="f9775-137">Response</span></span>

<span data-ttu-id="f9775-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f9775-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.set)"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "3607e9f9-e9f9-3607-f9e9-0736f9e90736",
      "description": "Starting term Set",    
      "localizedNames" : [
        {
          "languageTag" : "en-US",
          "name" : "Department"
        }
      ]
    }
  ]
}
```

[microsoft.graph.termStore.set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/List termstore-set",
  "suppressions": [
  ]
}
-->
