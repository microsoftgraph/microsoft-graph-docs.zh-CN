---
title: 获取术语
description: 读取术语对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5d154606c4f3581f0c5136ebd04d863185cf1721
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330160"
---
# <a name="get-term"></a><span data-ttu-id="64adb-103">获取术语</span><span class="sxs-lookup"><span data-stu-id="64adb-103">Get term</span></span>
<span data-ttu-id="64adb-104">命名空间： termStore</span><span class="sxs-lookup"><span data-stu-id="64adb-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64adb-105">读取 [术语](../resources/termstore-term.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="64adb-105">Read the properties and relationships of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64adb-106">权限</span><span class="sxs-lookup"><span data-stu-id="64adb-106">Permissions</span></span>
<span data-ttu-id="64adb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64adb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64adb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64adb-109">Permission type</span></span>|<span data-ttu-id="64adb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64adb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64adb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64adb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64adb-112">TermStore、TermStore 和所有</span><span class="sxs-lookup"><span data-stu-id="64adb-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="64adb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64adb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64adb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64adb-114">Not supported.</span></span>    |
|<span data-ttu-id="64adb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="64adb-115">Application</span></span> | <span data-ttu-id="64adb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="64adb-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="64adb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64adb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
GET /termStore/groups/{groupId}/sets/{setId}/terms/{termId}
GET /termStore/sets/{setId}/terms/{termId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64adb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="64adb-118">Optional query parameters</span></span>
<span data-ttu-id="64adb-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="64adb-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="64adb-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="64adb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="64adb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="64adb-121">Request headers</span></span>
|<span data-ttu-id="64adb-122">名称</span><span class="sxs-lookup"><span data-stu-id="64adb-122">Name</span></span>|<span data-ttu-id="64adb-123">说明</span><span class="sxs-lookup"><span data-stu-id="64adb-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64adb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="64adb-124">Authorization</span></span>|<span data-ttu-id="64adb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64adb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64adb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="64adb-127">Request body</span></span>
<span data-ttu-id="64adb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64adb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64adb-129">响应</span><span class="sxs-lookup"><span data-stu-id="64adb-129">Response</span></span>

<span data-ttu-id="64adb-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [term](../resources/termstore-term.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64adb-130">If successful, this method returns a `200 OK` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64adb-131">示例</span><span class="sxs-lookup"><span data-stu-id="64adb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64adb-132">请求</span><span class="sxs-lookup"><span data-stu-id="64adb-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64adb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="64adb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term"
} -->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/{groupId}/sets/{setId}/terms/{termId}
```
# <a name="c"></a>[<span data-ttu-id="64adb-134">C#</span><span class="sxs-lookup"><span data-stu-id="64adb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64adb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64adb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64adb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64adb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="64adb-137">响应</span><span class="sxs-lookup"><span data-stu-id="64adb-137">Response</span></span>
<span data-ttu-id="64adb-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="64adb-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "81be9856-9856-81be-5698-be815698be81",
  "createdDateTime": "2019-06-21T20:01:37Z",
  "labels" : [
    {
        "name" : "Copy of myTerm",
        "languageTag" : "en-US",
        "isDefault" : true
    }
  ],
  "lastModifiedDateTime": "2019-06-21T20:01:37Z"
}
```

[microsoft.graph.termStore.term]: ../resources/termstore-term.md

<!--
{
  "type": "#page.annotation",
  "description": "Get term entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get term",
  "suppressions": [
  ]
}
-->

