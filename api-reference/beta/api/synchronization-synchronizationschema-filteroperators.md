---
title: synchronizationSchema：filterOperators
description: 列出范围筛选器中支持的所有运算符。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 0f2274490bba86653e6c1423fa832db265394526
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625642"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="d8435-103">synchronizationSchema：filterOperators</span><span class="sxs-lookup"><span data-stu-id="d8435-103">synchronizationSchema: filterOperators</span></span>

<span data-ttu-id="d8435-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8435-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8435-105">列出范围筛选器中 [支持的所有运算符](../resources/synchronization-filter.md)。</span><span class="sxs-lookup"><span data-stu-id="d8435-105">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8435-106">权限</span><span class="sxs-lookup"><span data-stu-id="d8435-106">Permissions</span></span>
<span data-ttu-id="d8435-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8435-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8435-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8435-109">Permission type</span></span>                        | <span data-ttu-id="d8435-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8435-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8435-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8435-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="d8435-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8435-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="d8435-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8435-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d8435-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8435-114">Not supported.</span></span>|
|<span data-ttu-id="d8435-115">Application</span><span class="sxs-lookup"><span data-stu-id="d8435-115">Application</span></span>                            |<span data-ttu-id="d8435-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8435-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d8435-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8435-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="d8435-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8435-118">Request headers</span></span>

| <span data-ttu-id="d8435-119">名称</span><span class="sxs-lookup"><span data-stu-id="d8435-119">Name</span></span>           | <span data-ttu-id="d8435-120">类型</span><span class="sxs-lookup"><span data-stu-id="d8435-120">Type</span></span>    | <span data-ttu-id="d8435-121">说明</span><span class="sxs-lookup"><span data-stu-id="d8435-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d8435-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8435-122">Authorization</span></span>  | <span data-ttu-id="d8435-123">string</span><span class="sxs-lookup"><span data-stu-id="d8435-123">string</span></span>  | <span data-ttu-id="d8435-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8435-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8435-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8435-126">Request body</span></span>

<span data-ttu-id="d8435-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d8435-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8435-128">响应</span><span class="sxs-lookup"><span data-stu-id="d8435-128">Response</span></span>

<span data-ttu-id="d8435-129">如果成功，此方法在响应正文中返回响应代码和 `200, OK` [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="d8435-129">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8435-130">示例</span><span class="sxs-lookup"><span data-stu-id="d8435-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8435-131">请求</span><span class="sxs-lookup"><span data-stu-id="d8435-131">Request</span></span>
<span data-ttu-id="d8435-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="d8435-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8435-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8435-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="c"></a>[<span data-ttu-id="d8435-134">C#</span><span class="sxs-lookup"><span data-stu-id="d8435-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8435-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8435-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8435-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8435-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8435-137">Java</span><span class="sxs-lookup"><span data-stu-id="d8435-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationschema-filteroperators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8435-138">响应</span><span class="sxs-lookup"><span data-stu-id="d8435-138">Response</span></span>
<span data-ttu-id="d8435-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="d8435-139">The following is an example of a response.</span></span>

><span data-ttu-id="d8435-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d8435-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d8435-141">在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8435-141">All the properties will be returned in an actual call.</span></span>

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


