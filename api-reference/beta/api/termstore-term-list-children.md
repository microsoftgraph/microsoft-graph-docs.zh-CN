---
title: 列出子项
description: 从 "子导航" 属性中获取术语。
author: mohitpcad
ms.prod: Sharepoint
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 22ed47e1332dbe8ff5da8597f51d58017c10093f
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329919"
---
# <a name="list-children"></a><span data-ttu-id="7af22-103">列出子项</span><span class="sxs-lookup"><span data-stu-id="7af22-103">List children</span></span>
<span data-ttu-id="7af22-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="7af22-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7af22-105">使用 "子导航" 属性获取 [集] 或 [术语] 资源的第一级子级。</span><span class="sxs-lookup"><span data-stu-id="7af22-105">Get the first level children of a [set] or [term] resource using the children navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="7af22-106">权限</span><span class="sxs-lookup"><span data-stu-id="7af22-106">Permissions</span></span>
<span data-ttu-id="7af22-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7af22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7af22-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7af22-109">Permission type</span></span>|<span data-ttu-id="7af22-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7af22-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7af22-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7af22-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7af22-112">TermStore、TermStore 和所有</span><span class="sxs-lookup"><span data-stu-id="7af22-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="7af22-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7af22-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7af22-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7af22-114">Not supported.</span></span>    |
|<span data-ttu-id="7af22-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7af22-115">Application</span></span> | <span data-ttu-id="7af22-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7af22-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7af22-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7af22-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/children
GET /termStore/sets/{setId}/terms/{termId}/children
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7af22-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7af22-118">Optional query parameters</span></span>
<span data-ttu-id="7af22-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7af22-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7af22-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7af22-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7af22-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7af22-121">Request headers</span></span>
|<span data-ttu-id="7af22-122">名称</span><span class="sxs-lookup"><span data-stu-id="7af22-122">Name</span></span>|<span data-ttu-id="7af22-123">说明</span><span class="sxs-lookup"><span data-stu-id="7af22-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7af22-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7af22-124">Authorization</span></span>|<span data-ttu-id="7af22-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7af22-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7af22-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7af22-127">Request body</span></span>
<span data-ttu-id="7af22-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7af22-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7af22-129">响应</span><span class="sxs-lookup"><span data-stu-id="7af22-129">Response</span></span>

<span data-ttu-id="7af22-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [term](../resources/termstore-term.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7af22-130">If successful, this method returns a `200 OK` response code and a collection of [term](../resources/termstore-term.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7af22-131">示例</span><span class="sxs-lookup"><span data-stu-id="7af22-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7af22-132">请求</span><span class="sxs-lookup"><span data-stu-id="7af22-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7af22-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7af22-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/children
```
# <a name="c"></a>[<span data-ttu-id="7af22-134">C#</span><span class="sxs-lookup"><span data-stu-id="7af22-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7af22-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7af22-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7af22-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7af22-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7af22-137">响应</span><span class="sxs-lookup"><span data-stu-id="7af22-137">Response</span></span>
<span data-ttu-id="7af22-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7af22-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.term)"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {      
      "id": "81be9856-9856-81be-5698-be815698be81",
      "labels" : [
        {
          "name" : "Car",
          "languageTag" : "en-US",
          "isDefault" : true
        }
      ],
      "lastModifiedDateTime": "2019-06-21T20:01:37Z"
   }  
 ]
}
```

[术语]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "Get children of a term or termSet in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termchildren",
  "suppressions": []
}
-->
