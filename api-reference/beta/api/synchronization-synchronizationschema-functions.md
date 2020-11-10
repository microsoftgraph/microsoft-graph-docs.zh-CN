---
title: synchronizationSchema：函数
description: 列出 attributeMappingSource 中当前支持的所有函数。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6bfd4bf92e49b2c213db561285321552a3383377
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971408"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="f563d-103">synchronizationSchema：函数</span><span class="sxs-lookup"><span data-stu-id="f563d-103">synchronizationSchema: functions</span></span>

<span data-ttu-id="f563d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f563d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f563d-105">列出 [attributeMappingSource](../resources/synchronization-attributemappingsource.md)中当前支持的所有函数。</span><span class="sxs-lookup"><span data-stu-id="f563d-105">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f563d-106">权限</span><span class="sxs-lookup"><span data-stu-id="f563d-106">Permissions</span></span>
<span data-ttu-id="f563d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f563d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f563d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f563d-109">Permission type</span></span>                        | <span data-ttu-id="f563d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f563d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f563d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f563d-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="f563d-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f563d-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="f563d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f563d-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="f563d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f563d-114">Not supported.</span></span>|
|<span data-ttu-id="f563d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f563d-115">Application</span></span>                            |<span data-ttu-id="f563d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f563d-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f563d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f563d-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="f563d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f563d-118">Request headers</span></span>

| <span data-ttu-id="f563d-119">名称</span><span class="sxs-lookup"><span data-stu-id="f563d-119">Name</span></span>           | <span data-ttu-id="f563d-120">类型</span><span class="sxs-lookup"><span data-stu-id="f563d-120">Type</span></span>    | <span data-ttu-id="f563d-121">说明</span><span class="sxs-lookup"><span data-stu-id="f563d-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="f563d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f563d-122">Authorization</span></span>  | <span data-ttu-id="f563d-123">string</span><span class="sxs-lookup"><span data-stu-id="f563d-123">string</span></span>  | <span data-ttu-id="f563d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f563d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f563d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f563d-126">Request body</span></span>

<span data-ttu-id="f563d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f563d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f563d-128">响应</span><span class="sxs-lookup"><span data-stu-id="f563d-128">Response</span></span>

<span data-ttu-id="f563d-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f563d-129">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f563d-130">示例</span><span class="sxs-lookup"><span data-stu-id="f563d-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f563d-131">请求</span><span class="sxs-lookup"><span data-stu-id="f563d-131">Request</span></span>
<span data-ttu-id="f563d-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="f563d-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f563d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f563d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```
# <a name="c"></a>[<span data-ttu-id="f563d-134">C#</span><span class="sxs-lookup"><span data-stu-id="f563d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-functions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f563d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f563d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-functions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f563d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f563d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-functions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f563d-137">Java</span><span class="sxs-lookup"><span data-stu-id="f563d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationschema-functions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f563d-138">响应</span><span class="sxs-lookup"><span data-stu-id="f563d-138">Response</span></span>
<span data-ttu-id="f563d-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="f563d-139">The following is an example of a response.</span></span>

><span data-ttu-id="f563d-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f563d-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f563d-141">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="f563d-141">All the properties will be returned in an actual call.</span></span>

<!--
{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        }
    ]
}
```

<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "IsNothing",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Join",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "separator",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Prepend",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "prefix",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Mid",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "start",
                    "required": true,
                    "type": "Integer"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "length",
                    "required": true,
                    "type": "Integer"
                }
            ]
        },
        {
            "name": "Not",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Replace",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Find",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpression",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpressionGroupName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Replacement",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "ReplacementPropertyName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Template",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "SingleAppRoleAssignment",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Split",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "delimiter",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "StripSpaces",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Switch",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "defaultValue",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "switchValue",
                    "required": false,
                    "type": "String"
                }
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
  "description": "synchronizationSchema: functions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


