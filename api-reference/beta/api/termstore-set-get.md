---
title: 获取集
description: 读取 set 对象的属性和关系。
author: mohitpcad
localization_priority: Normal
ms.prod: taxonomy
doc_type: apiPageType
ms.openlocfilehash: 995ed341a5b92e11f6ecfa7cac8405ec7dc2a2af
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456462"
---
# <a name="get-set"></a><span data-ttu-id="2aba8-103">获取集</span><span class="sxs-lookup"><span data-stu-id="2aba8-103">Get set</span></span>
<span data-ttu-id="2aba8-104">命名空间：microsoft.graph.termStore [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="2aba8-104">Namespace: microsoft.graph.termStore [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>

<span data-ttu-id="2aba8-105">读取 set 对象的属性 [和](../resources/termstore-set.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="2aba8-105">Read the properties and relationships of a [set](../resources/termstore-set.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2aba8-106">权限</span><span class="sxs-lookup"><span data-stu-id="2aba8-106">Permissions</span></span>
<span data-ttu-id="2aba8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2aba8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2aba8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2aba8-109">Permission type</span></span>|<span data-ttu-id="2aba8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2aba8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2aba8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2aba8-111">Delegated (work or school account)</span></span> |<span data-ttu-id="2aba8-112">TermStore.Read.All、TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2aba8-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="2aba8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2aba8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2aba8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2aba8-114">Not supported.</span></span>    |
|<span data-ttu-id="2aba8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2aba8-115">Application</span></span> | <span data-ttu-id="2aba8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2aba8-116">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="2aba8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2aba8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/sets/{set-id}
GET /sites/{site-id}/termStore/sets/{set-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2aba8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2aba8-118">Optional query parameters</span></span>
<span data-ttu-id="2aba8-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2aba8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2aba8-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2aba8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2aba8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2aba8-121">Request headers</span></span>
|<span data-ttu-id="2aba8-122">名称</span><span class="sxs-lookup"><span data-stu-id="2aba8-122">Name</span></span>|<span data-ttu-id="2aba8-123">说明</span><span class="sxs-lookup"><span data-stu-id="2aba8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2aba8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2aba8-124">Authorization</span></span>|<span data-ttu-id="2aba8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2aba8-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2aba8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2aba8-127">Request body</span></span>
<span data-ttu-id="2aba8-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2aba8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2aba8-129">响应</span><span class="sxs-lookup"><span data-stu-id="2aba8-129">Response</span></span>

<span data-ttu-id="2aba8-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [set](../resources/termstore-set.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2aba8-130">If successful, this method returns a `200 OK` response code and a [set](../resources/termstore-set.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2aba8-131">示例</span><span class="sxs-lookup"><span data-stu-id="2aba8-131">Examples</span></span>

### <a name="example-1-get-a-termstore-set"></a><span data-ttu-id="2aba8-132">示例 1：获取 termStore 集</span><span class="sxs-lookup"><span data-stu-id="2aba8-132">Example 1: Get a termStore set</span></span>

#### <a name="request"></a><span data-ttu-id="2aba8-133">请求</span><span class="sxs-lookup"><span data-stu-id="2aba8-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_set_2"
}-->

``` http
GET https://graph.microsoft.com/beta/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f
```
# <a name="c"></a>[<span data-ttu-id="2aba8-134">C#</span><span class="sxs-lookup"><span data-stu-id="2aba8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-set-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2aba8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2aba8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-set-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2aba8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2aba8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-set-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2aba8-137">Java</span><span class="sxs-lookup"><span data-stu-id="2aba8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-set-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2aba8-138">响应</span><span class="sxs-lookup"><span data-stu-id="2aba8-138">Response</span></span>
><span data-ttu-id="2aba8-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2aba8-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "createdDateTime": "2019-06-21T20:01:37Z",  
  "description": "Starting term Set",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

### <a name="example-2-get-a-site-collection-termstore-set"></a><span data-ttu-id="2aba8-140">示例 2：获取网站集术语Store集</span><span class="sxs-lookup"><span data-stu-id="2aba8-140">Example 2: Get a site collection termStore Set</span></span>

#### <a name="request"></a><span data-ttu-id="2aba8-141">请求</span><span class="sxs-lookup"><span data-stu-id="2aba8-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_siteCollection_termStore_set"
}-->

``` http
GET https://graph.microsoft.com/beta/sites/microsoft.sharepoint.com,c6482504-4a85-4b21-858a-7e88dafc8232,d90ca07d-25c0-4ce7-864b-d68b607e697f/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f
```

#### <a name="response"></a><span data-ttu-id="2aba8-142">响应</span><span class="sxs-lookup"><span data-stu-id="2aba8-142">Response</span></span>
><span data-ttu-id="2aba8-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2aba8-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.set"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{

  "createdDateTime": "2019-06-21T20:01:37Z",  
  "description": "Starting term Set",
  "id": "8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f",
  "localizedNames" : [
    {
      "languageTag" : "en-US",
      "name" : "Department"
    }
  ]
}
```

[microsoft.graph.termStore.group]: ../resources/termstore-group.md
[microsoft.graph.termStore.set]: ../resources/termstore-set.md
[microsoft.graph.termStore.store]: ../resources/termstore-store.md

<!--
{
  "type": "#page.annotation",
  "description": "Get termSet entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/Get termSet",
  "suppressions": [
  ]
}
-->


