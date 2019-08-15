---
title: 'synchronizationSchema: filterOperators'
description: 列出作用域筛选器支持的所有运算符。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dbe23e5a909639dfc43cda4b03aaf7f26f761d19
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409727"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="190f6-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="190f6-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="190f6-104">列出[作用域筛选器](../resources/synchronization-filter.md)支持的所有运算符。</span><span class="sxs-lookup"><span data-stu-id="190f6-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="190f6-105">权限</span><span class="sxs-lookup"><span data-stu-id="190f6-105">Permissions</span></span>
<span data-ttu-id="190f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="190f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="190f6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="190f6-108">Permission type</span></span>                        | <span data-ttu-id="190f6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="190f6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="190f6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="190f6-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="190f6-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="190f6-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="190f6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="190f6-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="190f6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="190f6-113">Not supported.</span></span>|
|<span data-ttu-id="190f6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="190f6-114">Application</span></span>                            |<span data-ttu-id="190f6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="190f6-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="190f6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="190f6-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="190f6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="190f6-117">Request headers</span></span>

| <span data-ttu-id="190f6-118">名称</span><span class="sxs-lookup"><span data-stu-id="190f6-118">Name</span></span>           | <span data-ttu-id="190f6-119">类型</span><span class="sxs-lookup"><span data-stu-id="190f6-119">Type</span></span>    | <span data-ttu-id="190f6-120">说明</span><span class="sxs-lookup"><span data-stu-id="190f6-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="190f6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="190f6-121">Authorization</span></span>  | <span data-ttu-id="190f6-122">string</span><span class="sxs-lookup"><span data-stu-id="190f6-122">string</span></span>  | <span data-ttu-id="190f6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="190f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="190f6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="190f6-125">Request body</span></span>

<span data-ttu-id="190f6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="190f6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="190f6-127">响应</span><span class="sxs-lookup"><span data-stu-id="190f6-127">Response</span></span>

<span data-ttu-id="190f6-128">如果成功, 此方法在响应`200, OK`正文中返回响应代码和[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="190f6-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="190f6-129">示例</span><span class="sxs-lookup"><span data-stu-id="190f6-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="190f6-130">请求</span><span class="sxs-lookup"><span data-stu-id="190f6-130">Request</span></span>
<span data-ttu-id="190f6-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="190f6-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="190f6-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="190f6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="190f6-133">C#</span><span class="sxs-lookup"><span data-stu-id="190f6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="190f6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="190f6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="190f6-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="190f6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="190f6-136">响应</span><span class="sxs-lookup"><span data-stu-id="190f6-136">Response</span></span>
<span data-ttu-id="190f6-137">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="190f6-137">The following is an example of a response.</span></span>

><span data-ttu-id="190f6-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="190f6-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="190f6-139">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="190f6-139">All the properties will be returned in an actual call.</span></span>

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
