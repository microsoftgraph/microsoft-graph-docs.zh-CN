---
title: 获取 synchronizationSchema
description: 检索给定同步作业或模板的架构。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 136e24507497db7a109272b41d1ad4c11d3b971e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969170"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="9465a-103">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="9465a-103">Get synchronizationSchema</span></span>

<span data-ttu-id="9465a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9465a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9465a-105">检索给定同步作业或模板的架构。</span><span class="sxs-lookup"><span data-stu-id="9465a-105">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="9465a-106">权限</span><span class="sxs-lookup"><span data-stu-id="9465a-106">Permissions</span></span>
<span data-ttu-id="9465a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9465a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9465a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9465a-109">Permission type</span></span>                        | <span data-ttu-id="9465a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9465a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9465a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9465a-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="9465a-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9465a-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="9465a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9465a-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="9465a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9465a-114">Not supported.</span></span> |
|<span data-ttu-id="9465a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9465a-115">Application</span></span>                            |<span data-ttu-id="9465a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9465a-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9465a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9465a-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="9465a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9465a-118">Request headers</span></span>

| <span data-ttu-id="9465a-119">名称</span><span class="sxs-lookup"><span data-stu-id="9465a-119">Name</span></span>           | <span data-ttu-id="9465a-120">类型</span><span class="sxs-lookup"><span data-stu-id="9465a-120">Type</span></span>    | <span data-ttu-id="9465a-121">说明</span><span class="sxs-lookup"><span data-stu-id="9465a-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="9465a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9465a-122">Authorization</span></span>  | <span data-ttu-id="9465a-123">string</span><span class="sxs-lookup"><span data-stu-id="9465a-123">string</span></span>  | <span data-ttu-id="9465a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9465a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9465a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9465a-126">Request body</span></span>

<span data-ttu-id="9465a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9465a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9465a-128">响应</span><span class="sxs-lookup"><span data-stu-id="9465a-128">Response</span></span>

<span data-ttu-id="9465a-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [synchronizationSchema](../resources/synchronization-synchronizationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9465a-129">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9465a-130">示例</span><span class="sxs-lookup"><span data-stu-id="9465a-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9465a-131">请求</span><span class="sxs-lookup"><span data-stu-id="9465a-131">Request</span></span>
<span data-ttu-id="9465a-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="9465a-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9465a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9465a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="c"></a>[<span data-ttu-id="9465a-134">C#</span><span class="sxs-lookup"><span data-stu-id="9465a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9465a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9465a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9465a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9465a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9465a-137">响应</span><span class="sxs-lookup"><span data-stu-id="9465a-137">Response</span></span>
<span data-ttu-id="9465a-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="9465a-138">The following is an example of a response.</span></span>

><span data-ttu-id="9465a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9465a-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9465a-140">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="9465a-140">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

{
    "directories": [
        {
            "name": "Azure Active Directory",
            "objects": [
                {
                    "name": "User",
                    "attributes": [
                        {
                            "name": "userPrincipalName",
                            "type": "string"
                        }
                    ]
                }
            ]
        },
        {
            "name": "Salesforce",
            "objects": [{}]
        }
    ],
    "synchronizationRules":[
        {
            "name": "USER_TO_USER",
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "Salesforce",
            "objectMappings": [
                {
                    "sourceObjectName": "User",
                    "targetObjectName": "User",
                    "attributeMappings": [
                        {
                            "source": {},
                            "targetAttributeName": "userName"
                        },
                        {}
                    ]
                },
                {}
            ]
        },
        {}
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


