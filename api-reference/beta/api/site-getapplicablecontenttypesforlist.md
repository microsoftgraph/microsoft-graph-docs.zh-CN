---
author: swapnil1993
title: site： getApplicableContentTypesForList
description: 获取可添加到列表中的网站内容类型。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 99ca8f23b153f8835fc841e142b79684601bd293
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772448"
---
# <a name="site-getapplicablecontenttypesforlist"></a><span data-ttu-id="7b78a-103">site： getApplicableContentTypesForList</span><span class="sxs-lookup"><span data-stu-id="7b78a-103">site: getApplicableContentTypesForList</span></span>
<span data-ttu-id="7b78a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b78a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b78a-105">获取[][][可添加到列表中的][contentType]网站内容类型。</span><span class="sxs-lookup"><span data-stu-id="7b78a-105">Get [site][] [contentTypes][contentType] that can be added to a list.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b78a-106">权限</span><span class="sxs-lookup"><span data-stu-id="7b78a-106">Permissions</span></span>

<span data-ttu-id="7b78a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b78a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b78a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b78a-109">Permission type</span></span>      | <span data-ttu-id="7b78a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b78a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b78a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b78a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7b78a-112">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7b78a-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="7b78a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b78a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b78a-114">不支持</span><span class="sxs-lookup"><span data-stu-id="7b78a-114">Not Supported</span></span>    |
|<span data-ttu-id="7b78a-115">Application</span><span class="sxs-lookup"><span data-stu-id="7b78a-115">Application</span></span> | <span data-ttu-id="7b78a-116">Sites.Read.All、Sites.ReadWrite.All、Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="7b78a-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b78a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b78a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/getApplicableContentTypesForList
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7b78a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7b78a-118">Optional query parameters</span></span>

<span data-ttu-id="7b78a-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7b78a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7b78a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7b78a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="7b78a-121">若要仅列出自定义内容类型，请使用 `$filter=isBuiltin eq false` 。</span><span class="sxs-lookup"><span data-stu-id="7b78a-121">To list only custom content types, use `$filter=isBuiltin eq false`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b78a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b78a-122">Request headers</span></span>
|<span data-ttu-id="7b78a-123">名称</span><span class="sxs-lookup"><span data-stu-id="7b78a-123">Name</span></span>|<span data-ttu-id="7b78a-124">说明</span><span class="sxs-lookup"><span data-stu-id="7b78a-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7b78a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b78a-125">Authorization</span></span>|<span data-ttu-id="7b78a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b78a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b78a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b78a-128">Request body</span></span>
<span data-ttu-id="7b78a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b78a-129">Do not supply a request body for this method.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="7b78a-130">函数参数</span><span class="sxs-lookup"><span data-stu-id="7b78a-130">Function Parameters</span></span>
<span data-ttu-id="7b78a-131">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="7b78a-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7b78a-132">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="7b78a-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7b78a-133">参数</span><span class="sxs-lookup"><span data-stu-id="7b78a-133">Parameter</span></span>|<span data-ttu-id="7b78a-134">类型</span><span class="sxs-lookup"><span data-stu-id="7b78a-134">Type</span></span>|<span data-ttu-id="7b78a-135">说明</span><span class="sxs-lookup"><span data-stu-id="7b78a-135">Description</span></span>|
|-|-|-|-|
|<span data-ttu-id="7b78a-136">listId</span><span class="sxs-lookup"><span data-stu-id="7b78a-136">listId</span></span>| <span data-ttu-id="7b78a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="7b78a-137">String</span></span> | <span data-ttu-id="7b78a-138">需要获取适用内容类型的列表的 GUID。</span><span class="sxs-lookup"><span data-stu-id="7b78a-138">GUID of the list for which the applicable content types need to be fetched.</span></span> <span data-ttu-id="7b78a-139">必需。</span><span class="sxs-lookup"><span data-stu-id="7b78a-139">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7b78a-140">响应</span><span class="sxs-lookup"><span data-stu-id="7b78a-140">Response</span></span>

<span data-ttu-id="7b78a-141">如果成功，此函数在响应 `200 OK` 正文中返回 响应代码和 [contentType](../resources/contenttype.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="7b78a-141">If successful, this function returns a `200 OK` response code and a [contentType](../resources/contenttype.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b78a-142">示例</span><span class="sxs-lookup"><span data-stu-id="7b78a-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b78a-143">请求</span><span class="sxs-lookup"><span data-stu-id="7b78a-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7b78a-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b78a-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "site_getapplicablecontenttypesforlist"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{siteId}/getApplicableContentTypesForList(listId='listId')
```
# <a name="c"></a>[<span data-ttu-id="7b78a-145">C#</span><span class="sxs-lookup"><span data-stu-id="7b78a-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-getapplicablecontenttypesforlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b78a-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b78a-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-getapplicablecontenttypesforlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b78a-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b78a-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-getapplicablecontenttypesforlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b78a-148">Java</span><span class="sxs-lookup"><span data-stu-id="7b78a-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/site-getapplicablecontenttypesforlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b78a-149">响应</span><span class="sxs-lookup"><span data-stu-id="7b78a-149">Response</span></span>

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
