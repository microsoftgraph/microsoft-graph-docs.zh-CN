---
title: synchronizationSchema： functions
description: 列出 attributeMappingSource 中当前支持的所有函数。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ff6d231f8f20d96262530230304028368554e41b
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625960"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="9895b-103">synchronizationSchema： functions</span><span class="sxs-lookup"><span data-stu-id="9895b-103">synchronizationSchema: functions</span></span>

<span data-ttu-id="9895b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9895b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9895b-105">列出 [attributeMappingSource 中当前支持的所有函数](../resources/synchronization-attributemappingsource.md)。</span><span class="sxs-lookup"><span data-stu-id="9895b-105">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9895b-106">权限</span><span class="sxs-lookup"><span data-stu-id="9895b-106">Permissions</span></span>
<span data-ttu-id="9895b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9895b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9895b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9895b-109">Permission type</span></span>                        | <span data-ttu-id="9895b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9895b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9895b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9895b-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="9895b-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9895b-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="9895b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9895b-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9895b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9895b-114">Not supported.</span></span>|
|<span data-ttu-id="9895b-115">Application</span><span class="sxs-lookup"><span data-stu-id="9895b-115">Application</span></span>                            |<span data-ttu-id="9895b-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9895b-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9895b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9895b-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="9895b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9895b-118">Request headers</span></span>

| <span data-ttu-id="9895b-119">名称</span><span class="sxs-lookup"><span data-stu-id="9895b-119">Name</span></span>           | <span data-ttu-id="9895b-120">类型</span><span class="sxs-lookup"><span data-stu-id="9895b-120">Type</span></span>    | <span data-ttu-id="9895b-121">说明</span><span class="sxs-lookup"><span data-stu-id="9895b-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="9895b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9895b-122">Authorization</span></span>  | <span data-ttu-id="9895b-123">string</span><span class="sxs-lookup"><span data-stu-id="9895b-123">string</span></span>  | <span data-ttu-id="9895b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9895b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9895b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9895b-126">Request body</span></span>

<span data-ttu-id="9895b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9895b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9895b-128">响应</span><span class="sxs-lookup"><span data-stu-id="9895b-128">Response</span></span>

<span data-ttu-id="9895b-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9895b-129">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9895b-130">示例</span><span class="sxs-lookup"><span data-stu-id="9895b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9895b-131">请求</span><span class="sxs-lookup"><span data-stu-id="9895b-131">Request</span></span>
<span data-ttu-id="9895b-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="9895b-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9895b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9895b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```
# <a name="c"></a>[<span data-ttu-id="9895b-134">C#</span><span class="sxs-lookup"><span data-stu-id="9895b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-functions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9895b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9895b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-functions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9895b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9895b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-functions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9895b-137">Java</span><span class="sxs-lookup"><span data-stu-id="9895b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationschema-functions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9895b-138">响应</span><span class="sxs-lookup"><span data-stu-id="9895b-138">Response</span></span>
<span data-ttu-id="9895b-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="9895b-139">The following is an example of a response.</span></span>

><span data-ttu-id="9895b-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9895b-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9895b-141">在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9895b-141">All the properties will be returned in an actual call.</span></span>

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


