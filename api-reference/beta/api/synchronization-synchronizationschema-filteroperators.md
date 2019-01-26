---
title: 'synchronizationSchema: filterOperators'
description: 列出所有支持的范围筛选器中的运算符。
localization_priority: Normal
ms.openlocfilehash: c564142aa6a26b3f83fa5f82036e3b97dc13e672
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573226"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="aafd6-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="aafd6-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aafd6-104">列出所有支持的[范围筛选器](../resources/synchronization-filter.md)的运算符。</span><span class="sxs-lookup"><span data-stu-id="aafd6-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aafd6-105">权限</span><span class="sxs-lookup"><span data-stu-id="aafd6-105">Permissions</span></span>
<span data-ttu-id="aafd6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aafd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aafd6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="aafd6-108">Permission type</span></span>                        | <span data-ttu-id="aafd6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aafd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="aafd6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aafd6-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="aafd6-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aafd6-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="aafd6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aafd6-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="aafd6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="aafd6-113">Not supported.</span></span>|
|<span data-ttu-id="aafd6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="aafd6-114">Application</span></span>                            |<span data-ttu-id="aafd6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aafd6-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="aafd6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aafd6-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="aafd6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="aafd6-117">Request headers</span></span>

| <span data-ttu-id="aafd6-118">名称</span><span class="sxs-lookup"><span data-stu-id="aafd6-118">Name</span></span>           | <span data-ttu-id="aafd6-119">类型</span><span class="sxs-lookup"><span data-stu-id="aafd6-119">Type</span></span>    | <span data-ttu-id="aafd6-120">说明</span><span class="sxs-lookup"><span data-stu-id="aafd6-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="aafd6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aafd6-121">Authorization</span></span>  | <span data-ttu-id="aafd6-122">string</span><span class="sxs-lookup"><span data-stu-id="aafd6-122">string</span></span>  | <span data-ttu-id="aafd6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aafd6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aafd6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="aafd6-125">Request body</span></span>

<span data-ttu-id="aafd6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aafd6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aafd6-127">响应</span><span class="sxs-lookup"><span data-stu-id="aafd6-127">Response</span></span>

<span data-ttu-id="aafd6-128">如果成功，此方法返回`200, OK`响应代码和响应正文中的[filterOperatorSchema](../resources/synchronization-filteroperatorschema.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="aafd6-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aafd6-129">示例</span><span class="sxs-lookup"><span data-stu-id="aafd6-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aafd6-130">请求</span><span class="sxs-lookup"><span data-stu-id="aafd6-130">Request</span></span>
<span data-ttu-id="aafd6-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aafd6-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="aafd6-132">响应</span><span class="sxs-lookup"><span data-stu-id="aafd6-132">Response</span></span>
<span data-ttu-id="aafd6-133">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="aafd6-133">The following is an example of a response.</span></span>

><span data-ttu-id="aafd6-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aafd6-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aafd6-135">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="aafd6-135">All the properties will be returned in an actual call.</span></span>

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
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [                
                "@string"
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
               "Boolean"
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
                "Boolean"
            ]
        },
        {
            "name": "IS NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
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
                "Boolean"
            ]
        },
        {
            "name": "NOT REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-filteroperators.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
