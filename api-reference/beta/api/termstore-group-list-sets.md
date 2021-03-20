---
title: 列表集
description: 获取 set 对象及其属性的列表。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 32c929f5156304e2a36aa64a5fcc8d97cee8468d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950444"
---
# <a name="list-sets"></a><span data-ttu-id="55e55-103">列表集</span><span class="sxs-lookup"><span data-stu-id="55e55-103">List sets</span></span>
<span data-ttu-id="55e55-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="55e55-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55e55-105">获取 set [对象及其](../resources/termstore-set.md) 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="55e55-105">Get a list of the [set](../resources/termstore-set.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="55e55-106">权限</span><span class="sxs-lookup"><span data-stu-id="55e55-106">Permissions</span></span>
<span data-ttu-id="55e55-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55e55-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="55e55-109">Permission type</span></span>|<span data-ttu-id="55e55-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55e55-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55e55-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55e55-111">Delegated (work or school account)</span></span> |<span data-ttu-id="55e55-112">TermStore.Read.All、TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55e55-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="55e55-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55e55-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55e55-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="55e55-114">Not supported.</span></span>    |
|<span data-ttu-id="55e55-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="55e55-115">Application</span></span> | <span data-ttu-id="55e55-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="55e55-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="55e55-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55e55-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups/{groupId}/sets
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55e55-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="55e55-118">Optional query parameters</span></span>
<span data-ttu-id="55e55-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="55e55-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="55e55-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="55e55-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="55e55-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="55e55-121">Request headers</span></span>
|<span data-ttu-id="55e55-122">名称</span><span class="sxs-lookup"><span data-stu-id="55e55-122">Name</span></span>|<span data-ttu-id="55e55-123">说明</span><span class="sxs-lookup"><span data-stu-id="55e55-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="55e55-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="55e55-124">Authorization</span></span>|<span data-ttu-id="55e55-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55e55-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="55e55-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="55e55-127">Request body</span></span>
<span data-ttu-id="55e55-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="55e55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55e55-129">响应</span><span class="sxs-lookup"><span data-stu-id="55e55-129">Response</span></span>

<span data-ttu-id="55e55-130">如果成功，此方法在响应正文中返回 响应代码 `200 OK` [和 set](../resources/termstore-set.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="55e55-130">If successful, this method returns a `200 OK` response code and a collection of [set](../resources/termstore-set.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55e55-131">示例</span><span class="sxs-lookup"><span data-stu-id="55e55-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55e55-132">请求</span><span class="sxs-lookup"><span data-stu-id="55e55-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="55e55-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="55e55-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_set_1"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets
```
# <a name="c"></a>[<span data-ttu-id="55e55-134">C#</span><span class="sxs-lookup"><span data-stu-id="55e55-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55e55-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55e55-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55e55-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55e55-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55e55-137">Java</span><span class="sxs-lookup"><span data-stu-id="55e55-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-set-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="55e55-138">响应</span><span class="sxs-lookup"><span data-stu-id="55e55-138">Response</span></span>

<span data-ttu-id="55e55-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="55e55-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


