---
title: 获取术语
description: 读取术语对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: b26b1bc5da13bd8edabe3f381f950c47894800d2
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456476"
---
# <a name="get-term"></a><span data-ttu-id="023ac-103">获取术语</span><span class="sxs-lookup"><span data-stu-id="023ac-103">Get term</span></span>
<span data-ttu-id="023ac-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="023ac-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="023ac-105">读取术语对象的属性 [和](../resources/termstore-term.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="023ac-105">Read the properties and relationships of a [term](../resources/termstore-term.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="023ac-106">权限</span><span class="sxs-lookup"><span data-stu-id="023ac-106">Permissions</span></span>
<span data-ttu-id="023ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="023ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="023ac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="023ac-109">Permission type</span></span>|<span data-ttu-id="023ac-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="023ac-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="023ac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="023ac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="023ac-112">TermStore.Read.All、TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="023ac-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="023ac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="023ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="023ac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="023ac-114">Not supported.</span></span>    |
|<span data-ttu-id="023ac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="023ac-115">Application</span></span> | <span data-ttu-id="023ac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="023ac-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="023ac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="023ac-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
} -->

``` http
GET /termStore/groups/{group-id}/sets/{set-id}/terms/{term-id}
GET /termStore/sets/{set-id}/terms/{term-id}
GET /sites/{site-id}/termStore/groups/{group-id}/sets/{set-id}/terms/{term-id}
GET /sites/{site-id}/termStore/sets/{set-id}/terms/{term-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="023ac-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="023ac-118">Optional query parameters</span></span>
<span data-ttu-id="023ac-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="023ac-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="023ac-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="023ac-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="023ac-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="023ac-121">Request headers</span></span>
|<span data-ttu-id="023ac-122">名称</span><span class="sxs-lookup"><span data-stu-id="023ac-122">Name</span></span>|<span data-ttu-id="023ac-123">说明</span><span class="sxs-lookup"><span data-stu-id="023ac-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="023ac-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="023ac-124">Authorization</span></span>|<span data-ttu-id="023ac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="023ac-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="023ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="023ac-127">Request body</span></span>
<span data-ttu-id="023ac-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="023ac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="023ac-129">响应</span><span class="sxs-lookup"><span data-stu-id="023ac-129">Response</span></span>

<span data-ttu-id="023ac-130">如果成功，此方法在响应正文中返回 响应代码 `200 OK` 和术语对象。 [](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="023ac-130">If successful, this method returns a `200 OK` response code and a [term](../resources/termstore-term.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="023ac-131">示例</span><span class="sxs-lookup"><span data-stu-id="023ac-131">Examples</span></span>

### <a name="example-1-get-a-termstore-term"></a><span data-ttu-id="023ac-132">示例 1：获取术语存储术语</span><span class="sxs-lookup"><span data-stu-id="023ac-132">Example 1: Get a termStore term</span></span>

#### <a name="request"></a><span data-ttu-id="023ac-133">请求</span><span class="sxs-lookup"><span data-stu-id="023ac-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="023ac-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="023ac-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_term_1"
} -->

``` http
GET https://graph.microsoft.com/beta/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f/terms/81be9856-9856-81be-5698-be815698be81
```
# <a name="c"></a>[<span data-ttu-id="023ac-135">C#</span><span class="sxs-lookup"><span data-stu-id="023ac-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-term-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="023ac-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="023ac-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-term-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="023ac-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="023ac-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-term-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="023ac-138">Java</span><span class="sxs-lookup"><span data-stu-id="023ac-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-term-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="023ac-139">响应</span><span class="sxs-lookup"><span data-stu-id="023ac-139">Response</span></span>
><span data-ttu-id="023ac-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="023ac-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2--get-a-site-collection-termstore-term"></a><span data-ttu-id="023ac-141">示例 2：获取网站集术语存储术语</span><span class="sxs-lookup"><span data-stu-id="023ac-141">Example 2 : Get a site collection termStore term</span></span>

#### <a name="request"></a><span data-ttu-id="023ac-142">请求</span><span class="sxs-lookup"><span data-stu-id="023ac-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_term_1"
} -->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/groups/1FFD3F87-9464-488A-A0EC-8FB90911182C/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f/terms/81be9856-9856-81be-5698-be815698be81
```

#### <a name="response"></a><span data-ttu-id="023ac-143">响应</span><span class="sxs-lookup"><span data-stu-id="023ac-143">Response</span></span>
><span data-ttu-id="023ac-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="023ac-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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



