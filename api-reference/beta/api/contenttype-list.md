---
author: swapnil1993
title: 列出 contentTypes
description: 列出网站或列表中的内容类型
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 20d2b451a607a899f7873ba5be5aad671faad972
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770493"
---
# <a name="list-contenttypes"></a><span data-ttu-id="b2e9c-103">列出 contentTypes</span><span class="sxs-lookup"><span data-stu-id="b2e9c-103">List contentTypes</span></span>
<span data-ttu-id="b2e9c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2e9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="b2e9c-105">获取网站[或列表中][contentType][的内容类型][][集合][]</span><span class="sxs-lookup"><span data-stu-id="b2e9c-105">Get the collection of [content types][contentType] in a [site][] or a [list][]</span></span>

## <a name="permissions"></a><span data-ttu-id="b2e9c-106">权限</span><span class="sxs-lookup"><span data-stu-id="b2e9c-106">Permissions</span></span>

<span data-ttu-id="b2e9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="b2e9c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2e9c-109">Permission type</span></span>      | <span data-ttu-id="b2e9c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2e9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2e9c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2e9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b2e9c-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b2e9c-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="b2e9c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2e9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2e9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-114">Not supported.</span></span>    |
|<span data-ttu-id="b2e9c-115">Application</span><span class="sxs-lookup"><span data-stu-id="b2e9c-115">Application</span></span> | <span data-ttu-id="b2e9c-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b2e9c-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2e9c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2e9c-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes
GET /sites/{site-id}/lists/{list-id}/contentTypes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2e9c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b2e9c-118">Optional query parameters</span></span>

<span data-ttu-id="b2e9c-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b2e9c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2e9c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2e9c-121">Request headers</span></span>
|<span data-ttu-id="b2e9c-122">名称</span><span class="sxs-lookup"><span data-stu-id="b2e9c-122">Name</span></span>|<span data-ttu-id="b2e9c-123">说明</span><span class="sxs-lookup"><span data-stu-id="b2e9c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b2e9c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2e9c-124">Authorization</span></span>|<span data-ttu-id="b2e9c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2e9c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2e9c-127">Request body</span></span>
<span data-ttu-id="b2e9c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2e9c-129">响应</span><span class="sxs-lookup"><span data-stu-id="b2e9c-129">Response</span></span>

<span data-ttu-id="b2e9c-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [contentType](../resources/contenttype.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b2e9c-130">If successful, this method returns a `200 OK` response code and a collection of [contentType](../resources/contenttype.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2e9c-131">示例</span><span class="sxs-lookup"><span data-stu-id="b2e9c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2e9c-132">请求</span><span class="sxs-lookup"><span data-stu-id="b2e9c-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b2e9c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2e9c-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum_contentTypes"} -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes
```
# <a name="c"></a>[<span data-ttu-id="b2e9c-134">C#</span><span class="sxs-lookup"><span data-stu-id="b2e9c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-contenttypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b2e9c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2e9c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-contenttypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b2e9c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2e9c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-contenttypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b2e9c-137">Java</span><span class="sxs-lookup"><span data-stu-id="b2e9c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-contenttypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2e9c-138">响应</span><span class="sxs-lookup"><span data-stu-id="b2e9c-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.contentType)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "id":"0x",
        "description":"",
        "group":"_Hidden",
        "hidden":false,
        "name":"System",
        "base": {
            "name": "System",
            "id": "0x"
        }
    },
    {
        "id":"0x00A7470EADF4194E2E9ED1031B61DA0884",
        "name": "docSet",
        "description": "custom docset",
        "hidden":false,
        "base": {
            "name": "Document Set",
            "id": "0x0120D520"
        },
        "group": "Custom Content Types"
    }
  ]
}
```


[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
[列表]: ../resources/list.md
[list]: ../resources/list.md
