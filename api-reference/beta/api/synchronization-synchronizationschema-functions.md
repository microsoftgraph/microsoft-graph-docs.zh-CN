---
title: 'synchronizationSchema: 函数'
description: 列出 attributeMappingSource 中当前支持的所有函数。
localization_priority: Normal
ms.openlocfilehash: c1563255a7444c65030799de3477bbadcaf7a196
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637988"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="a6061-103">synchronizationSchema: 函数</span><span class="sxs-lookup"><span data-stu-id="a6061-103">synchronizationSchema: functions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6061-104">列出[attributeMappingSource](../resources/synchronization-attributemappingsource.md)中当前支持的所有函数。</span><span class="sxs-lookup"><span data-stu-id="a6061-104">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6061-105">权限</span><span class="sxs-lookup"><span data-stu-id="a6061-105">Permissions</span></span>
<span data-ttu-id="a6061-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6061-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6061-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6061-108">Permission type</span></span>                        | <span data-ttu-id="a6061-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6061-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6061-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6061-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="a6061-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6061-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="a6061-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6061-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="a6061-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6061-113">Not supported.</span></span>|
|<span data-ttu-id="a6061-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6061-114">Application</span></span>                            |<span data-ttu-id="a6061-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6061-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a6061-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6061-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="a6061-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6061-117">Request headers</span></span>

| <span data-ttu-id="a6061-118">名称</span><span class="sxs-lookup"><span data-stu-id="a6061-118">Name</span></span>           | <span data-ttu-id="a6061-119">类型</span><span class="sxs-lookup"><span data-stu-id="a6061-119">Type</span></span>    | <span data-ttu-id="a6061-120">说明</span><span class="sxs-lookup"><span data-stu-id="a6061-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="a6061-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6061-121">Authorization</span></span>  | <span data-ttu-id="a6061-122">string</span><span class="sxs-lookup"><span data-stu-id="a6061-122">string</span></span>  | <span data-ttu-id="a6061-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a6061-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6061-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6061-125">Request body</span></span>

<span data-ttu-id="a6061-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a6061-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6061-127">响应</span><span class="sxs-lookup"><span data-stu-id="a6061-127">Response</span></span>

<span data-ttu-id="a6061-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="a6061-128">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6061-129">示例</span><span class="sxs-lookup"><span data-stu-id="a6061-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6061-130">请求</span><span class="sxs-lookup"><span data-stu-id="a6061-130">Request</span></span>
<span data-ttu-id="a6061-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="a6061-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```

##### <a name="response"></a><span data-ttu-id="a6061-132">响应</span><span class="sxs-lookup"><span data-stu-id="a6061-132">Response</span></span>
<span data-ttu-id="a6061-133">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="a6061-133">The following is an example of a response.</span></span>

><span data-ttu-id="a6061-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a6061-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a6061-135">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="a6061-135">All the properties will be returned in an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a6061-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a6061-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a6061-137">语言</span><span class="sxs-lookup"><span data-stu-id="a6061-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationschema_functions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6061-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="a6061-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationschema_functions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-functions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-functions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
