---
title: 列出组
description: 从组导航属性获取组。
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: apiPageType
ms.openlocfilehash: 3996bf2cc502f47ad5a2ce60fc92bd9f9d570fe1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957157"
---
# <a name="list-groups"></a><span data-ttu-id="2d47f-103">列出组</span><span class="sxs-lookup"><span data-stu-id="2d47f-103">List groups</span></span>
<span data-ttu-id="2d47f-104">命名空间：microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="2d47f-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d47f-105">获取存储 [的组](../resources/termstore-group.md) 对象 [列表](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="2d47f-105">Get the list of [group](../resources/termstore-group.md) objects of a [store](../resources/termstore-store.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="2d47f-106">权限</span><span class="sxs-lookup"><span data-stu-id="2d47f-106">Permissions</span></span>
<span data-ttu-id="2d47f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d47f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d47f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d47f-109">Permission type</span></span>|<span data-ttu-id="2d47f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d47f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d47f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d47f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d47f-112">TermStore.Read.All、TermStore.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d47f-112">TermStore.Read.All, TermStore.ReadWrite.All</span></span> |
|<span data-ttu-id="2d47f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d47f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d47f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d47f-114">Not supported.</span></span>    |
|<span data-ttu-id="2d47f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d47f-115">Application</span></span> | <span data-ttu-id="2d47f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d47f-116">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d47f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d47f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /termStore/groups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2d47f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2d47f-118">Optional query parameters</span></span>
<span data-ttu-id="2d47f-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2d47f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2d47f-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2d47f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2d47f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d47f-121">Request headers</span></span>
|<span data-ttu-id="2d47f-122">名称</span><span class="sxs-lookup"><span data-stu-id="2d47f-122">Name</span></span>|<span data-ttu-id="2d47f-123">说明</span><span class="sxs-lookup"><span data-stu-id="2d47f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d47f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d47f-124">Authorization</span></span>|<span data-ttu-id="2d47f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d47f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d47f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d47f-127">Request body</span></span>
<span data-ttu-id="2d47f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2d47f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d47f-129">响应</span><span class="sxs-lookup"><span data-stu-id="2d47f-129">Response</span></span>

<span data-ttu-id="2d47f-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [group](../resources/termstore-group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2d47f-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/termstore-group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2d47f-131">示例</span><span class="sxs-lookup"><span data-stu-id="2d47f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2d47f-132">请求</span><span class="sxs-lookup"><span data-stu-id="2d47f-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2d47f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d47f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/termStore/groups
```
# <a name="c"></a>[<span data-ttu-id="2d47f-134">C#</span><span class="sxs-lookup"><span data-stu-id="2d47f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d47f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d47f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d47f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d47f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d47f-137">Java</span><span class="sxs-lookup"><span data-stu-id="2d47f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2d47f-138">响应</span><span class="sxs-lookup"><span data-stu-id="2d47f-138">Response</span></span>
<span data-ttu-id="2d47f-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2d47f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.termStore.group)"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "85825593-5593-8582-9355-828593558285",
      "createdDateTime": "2019-06-21T20:01:37Z",
      "description": "My term group",
      "scope" : "global",
      "displayName": "myGroup"  
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Get termGroup entity in termStore",
  "keywords": "term,termStore",
  "section": "documentation",
  "tocPath": "termStore/List termGroups",
  "suppressions": [
  ]
}
-->



