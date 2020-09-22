---
title: 列表关系
description: 从关系导航属性中获取关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: ba593b7d5be184d5a53c0dd2af98dc655a3712bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042861"
---
# <a name="list-relations"></a><span data-ttu-id="d1096-103">列表关系</span><span class="sxs-lookup"><span data-stu-id="d1096-103">List relations</span></span>
<span data-ttu-id="d1096-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="d1096-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1096-105">从 "关系" 导航属性中获取 [术语] 或 [集] 的不同关系。</span><span class="sxs-lookup"><span data-stu-id="d1096-105">Get the different relation of a [term] or [set] from the relations navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1096-106">权限</span><span class="sxs-lookup"><span data-stu-id="d1096-106">Permissions</span></span>
<span data-ttu-id="d1096-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1096-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1096-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1096-109">Permission type</span></span>|<span data-ttu-id="d1096-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d1096-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1096-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1096-111">Delegated (work or school account)</span></span> |<span data-ttu-id="d1096-112">TermStore、TermStore 和所有</span><span class="sxs-lookup"><span data-stu-id="d1096-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="d1096-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1096-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1096-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1096-114">Not supported.</span></span>    |
|<span data-ttu-id="d1096-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1096-115">Application</span></span> | <span data-ttu-id="d1096-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1096-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="d1096-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1096-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /termStore/sets/{setId}/relations
GET /termStore/sets/{setId}/terms/{termId}/relations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1096-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d1096-118">Optional query parameters</span></span>
<span data-ttu-id="d1096-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d1096-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d1096-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d1096-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1096-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1096-121">Request headers</span></span>
|<span data-ttu-id="d1096-122">名称</span><span class="sxs-lookup"><span data-stu-id="d1096-122">Name</span></span>|<span data-ttu-id="d1096-123">说明</span><span class="sxs-lookup"><span data-stu-id="d1096-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d1096-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1096-124">Authorization</span></span>|<span data-ttu-id="d1096-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1096-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1096-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1096-127">Request body</span></span>
<span data-ttu-id="d1096-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1096-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1096-129">响应</span><span class="sxs-lookup"><span data-stu-id="d1096-129">Response</span></span>

<span data-ttu-id="d1096-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [relation](../resources/termstore-relation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d1096-130">If successful, this method returns a `200 OK` response code and a collection of [relation](../resources/termstore-relation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1096-131">示例</span><span class="sxs-lookup"><span data-stu-id="d1096-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d1096-132">请求</span><span class="sxs-lookup"><span data-stu-id="d1096-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d1096-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1096-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_relation"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/{setId}/relations
```
# <a name="c"></a>[<span data-ttu-id="d1096-134">C#</span><span class="sxs-lookup"><span data-stu-id="d1096-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-relation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1096-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1096-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-relation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1096-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1096-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-relation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d1096-137">响应</span><span class="sxs-lookup"><span data-stu-id="d1096-137">Response</span></span>
<span data-ttu-id="d1096-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d1096-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.relation)"
}-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "052c749c-749c-052c-9c74-2c059c742c05",
      "relationship": "pin"
    }
  ]
}
```


[set]: ../resources/termstore-set.md
[术语]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[microsoft.graph.termStore.relation]: ../resources/termstore-relation.md


<!--
{
  "type": "#page.annotation",
  "description": "Create a pinned term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/term list relations",
  "suppressions": [
  ]
}
-->


