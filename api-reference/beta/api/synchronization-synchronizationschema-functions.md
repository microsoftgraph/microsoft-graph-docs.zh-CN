---
title: synchronizationSchema： 函数
description: 列出所有 attributeMappingSource 当前支持的功能。
localization_priority: Normal
ms.openlocfilehash: 5dc7734e9d747ac1e832aebb7d9c7355c2fbb52f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841005"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="13ff6-103">synchronizationSchema： 函数</span><span class="sxs-lookup"><span data-stu-id="13ff6-103">synchronizationSchema: functions</span></span>

> <span data-ttu-id="13ff6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="13ff6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13ff6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="13ff6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13ff6-106">列出所有[attributeMappingSource](../resources/synchronization-attributemappingsource.md)当前支持的功能。</span><span class="sxs-lookup"><span data-stu-id="13ff6-106">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="13ff6-107">权限</span><span class="sxs-lookup"><span data-stu-id="13ff6-107">Permissions</span></span>
<span data-ttu-id="13ff6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="13ff6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13ff6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="13ff6-110">Permission type</span></span>                        | <span data-ttu-id="13ff6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="13ff6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="13ff6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="13ff6-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="13ff6-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13ff6-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="13ff6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="13ff6-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="13ff6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="13ff6-115">Not supported.</span></span>|
|<span data-ttu-id="13ff6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="13ff6-116">Application</span></span>                            |<span data-ttu-id="13ff6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="13ff6-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="13ff6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="13ff6-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="13ff6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="13ff6-119">Request headers</span></span>

| <span data-ttu-id="13ff6-120">名称</span><span class="sxs-lookup"><span data-stu-id="13ff6-120">Name</span></span>           | <span data-ttu-id="13ff6-121">类型</span><span class="sxs-lookup"><span data-stu-id="13ff6-121">Type</span></span>    | <span data-ttu-id="13ff6-122">说明</span><span class="sxs-lookup"><span data-stu-id="13ff6-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="13ff6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="13ff6-123">Authorization</span></span>  | <span data-ttu-id="13ff6-124">string</span><span class="sxs-lookup"><span data-stu-id="13ff6-124">string</span></span>  | <span data-ttu-id="13ff6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="13ff6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13ff6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="13ff6-127">Request body</span></span>

<span data-ttu-id="13ff6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="13ff6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13ff6-129">响应</span><span class="sxs-lookup"><span data-stu-id="13ff6-129">Response</span></span>

<span data-ttu-id="13ff6-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="13ff6-130">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13ff6-131">示例</span><span class="sxs-lookup"><span data-stu-id="13ff6-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="13ff6-132">请求</span><span class="sxs-lookup"><span data-stu-id="13ff6-132">Request</span></span>
<span data-ttu-id="13ff6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="13ff6-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```

##### <a name="response"></a><span data-ttu-id="13ff6-134">响应</span><span class="sxs-lookup"><span data-stu-id="13ff6-134">Response</span></span>
<span data-ttu-id="13ff6-135">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="13ff6-135">The following is an example of a response.</span></span>

><span data-ttu-id="13ff6-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="13ff6-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="13ff6-137">将返回实际呼叫中的所有属性。</span><span class="sxs-lookup"><span data-stu-id="13ff6-137">All the properties will be returned in an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: functions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
