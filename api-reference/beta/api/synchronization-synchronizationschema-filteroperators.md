---
title: 'synchronizationSchema: filterOperators'
description: 列出所有支持的范围筛选器中的运算符。
localization_priority: Normal
ms.openlocfilehash: 6c7f15c684bb0017c8e8430e390015029204ef1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835754"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="94fac-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="94fac-103">synchronizationSchema: filterOperators</span></span>

> <span data-ttu-id="94fac-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="94fac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94fac-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="94fac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94fac-106">列出所有支持的[范围筛选器](../resources/synchronization-filter.md)的运算符。</span><span class="sxs-lookup"><span data-stu-id="94fac-106">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94fac-107">权限</span><span class="sxs-lookup"><span data-stu-id="94fac-107">Permissions</span></span>
<span data-ttu-id="94fac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94fac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94fac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94fac-110">Permission type</span></span>                        | <span data-ttu-id="94fac-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94fac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="94fac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94fac-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="94fac-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94fac-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="94fac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94fac-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="94fac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94fac-115">Not supported.</span></span>|
|<span data-ttu-id="94fac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94fac-116">Application</span></span>                            |<span data-ttu-id="94fac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="94fac-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="94fac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94fac-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="94fac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="94fac-119">Request headers</span></span>

| <span data-ttu-id="94fac-120">名称</span><span class="sxs-lookup"><span data-stu-id="94fac-120">Name</span></span>           | <span data-ttu-id="94fac-121">类型</span><span class="sxs-lookup"><span data-stu-id="94fac-121">Type</span></span>    | <span data-ttu-id="94fac-122">说明</span><span class="sxs-lookup"><span data-stu-id="94fac-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="94fac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94fac-123">Authorization</span></span>  | <span data-ttu-id="94fac-124">string</span><span class="sxs-lookup"><span data-stu-id="94fac-124">string</span></span>  | <span data-ttu-id="94fac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94fac-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94fac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="94fac-127">Request body</span></span>

<span data-ttu-id="94fac-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94fac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94fac-129">响应</span><span class="sxs-lookup"><span data-stu-id="94fac-129">Response</span></span>

<span data-ttu-id="94fac-130">如果成功，此方法返回`200, OK`响应代码和响应正文中的[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="94fac-130">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94fac-131">示例</span><span class="sxs-lookup"><span data-stu-id="94fac-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="94fac-132">请求</span><span class="sxs-lookup"><span data-stu-id="94fac-132">Request</span></span>
<span data-ttu-id="94fac-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94fac-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="94fac-134">响应</span><span class="sxs-lookup"><span data-stu-id="94fac-134">Response</span></span>
<span data-ttu-id="94fac-135">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="94fac-135">The following is an example of a response.</span></span>

><span data-ttu-id="94fac-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="94fac-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="94fac-137">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="94fac-137">All the properties will be returned in an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
