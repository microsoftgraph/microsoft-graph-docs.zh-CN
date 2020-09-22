---
title: 'synchronizationSchema: filterOperators'
description: 列出作用域筛选器支持的所有运算符。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aaea4985f19a475f57c655cebd6d909d5f09e0fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076651"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="0ea99-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="0ea99-103">synchronizationSchema: filterOperators</span></span>

<span data-ttu-id="0ea99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ea99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ea99-105">列出 [作用域筛选器](../resources/synchronization-filter.md)支持的所有运算符。</span><span class="sxs-lookup"><span data-stu-id="0ea99-105">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea99-106">权限</span><span class="sxs-lookup"><span data-stu-id="0ea99-106">Permissions</span></span>
<span data-ttu-id="0ea99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ea99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea99-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ea99-109">Permission type</span></span>                        | <span data-ttu-id="0ea99-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ea99-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ea99-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ea99-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="0ea99-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea99-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0ea99-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ea99-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0ea99-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ea99-114">Not supported.</span></span>|
|<span data-ttu-id="0ea99-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ea99-115">Application</span></span>                            |<span data-ttu-id="0ea99-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ea99-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0ea99-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ea99-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="0ea99-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ea99-118">Request headers</span></span>

| <span data-ttu-id="0ea99-119">名称</span><span class="sxs-lookup"><span data-stu-id="0ea99-119">Name</span></span>           | <span data-ttu-id="0ea99-120">类型</span><span class="sxs-lookup"><span data-stu-id="0ea99-120">Type</span></span>    | <span data-ttu-id="0ea99-121">说明</span><span class="sxs-lookup"><span data-stu-id="0ea99-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0ea99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea99-122">Authorization</span></span>  | <span data-ttu-id="0ea99-123">string</span><span class="sxs-lookup"><span data-stu-id="0ea99-123">string</span></span>  | <span data-ttu-id="0ea99-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ea99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ea99-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ea99-126">Request body</span></span>

<span data-ttu-id="0ea99-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ea99-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea99-128">响应</span><span class="sxs-lookup"><span data-stu-id="0ea99-128">Response</span></span>

<span data-ttu-id="0ea99-129">如果成功，此方法 `200, OK` 在响应正文中返回响应代码和 [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="0ea99-129">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ea99-130">示例</span><span class="sxs-lookup"><span data-stu-id="0ea99-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ea99-131">请求</span><span class="sxs-lookup"><span data-stu-id="0ea99-131">Request</span></span>
<span data-ttu-id="0ea99-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0ea99-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ea99-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea99-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="c"></a>[<span data-ttu-id="0ea99-134">C#</span><span class="sxs-lookup"><span data-stu-id="0ea99-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ea99-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ea99-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ea99-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ea99-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0ea99-137">响应</span><span class="sxs-lookup"><span data-stu-id="0ea99-137">Response</span></span>
<span data-ttu-id="0ea99-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0ea99-138">The following is an example of a response.</span></span>

><span data-ttu-id="0ea99-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0ea99-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0ea99-140">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="0ea99-140">All the properties will be returned in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filterOperatorSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "String",
                "Integer"
            ]
        }
    ]
}
```
<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "IS FALSE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "IS NOT NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS TRUE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "NOT EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "NOT REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        }
    ]
}
-->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: synchronizationschema_filteroperators/container/arity:\r\n       Expected type String but actual was Binary. Property: arity, actual value: 'Binary'"
  ]
}
-->


