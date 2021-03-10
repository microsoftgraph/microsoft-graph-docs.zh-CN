---
title: 获取 synchronizationSchema
description: 检索给定同步作业或模板的架构。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 84c1dc9112851330be721f425a01228d278d014b
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625963"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="53b14-103">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="53b14-103">Get synchronizationSchema</span></span>

<span data-ttu-id="53b14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53b14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53b14-105">检索给定同步作业或模板的架构。</span><span class="sxs-lookup"><span data-stu-id="53b14-105">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="53b14-106">权限</span><span class="sxs-lookup"><span data-stu-id="53b14-106">Permissions</span></span>
<span data-ttu-id="53b14-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53b14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53b14-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53b14-109">Permission type</span></span>                        | <span data-ttu-id="53b14-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53b14-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="53b14-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53b14-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="53b14-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="53b14-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="53b14-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53b14-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="53b14-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="53b14-114">Not supported.</span></span> |
|<span data-ttu-id="53b14-115">Application</span><span class="sxs-lookup"><span data-stu-id="53b14-115">Application</span></span>                            |<span data-ttu-id="53b14-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b14-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="53b14-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53b14-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="53b14-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="53b14-118">Request headers</span></span>

| <span data-ttu-id="53b14-119">名称</span><span class="sxs-lookup"><span data-stu-id="53b14-119">Name</span></span>           | <span data-ttu-id="53b14-120">类型</span><span class="sxs-lookup"><span data-stu-id="53b14-120">Type</span></span>    | <span data-ttu-id="53b14-121">说明</span><span class="sxs-lookup"><span data-stu-id="53b14-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="53b14-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53b14-122">Authorization</span></span>  | <span data-ttu-id="53b14-123">string</span><span class="sxs-lookup"><span data-stu-id="53b14-123">string</span></span>  | <span data-ttu-id="53b14-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53b14-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53b14-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="53b14-126">Request body</span></span>

<span data-ttu-id="53b14-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53b14-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53b14-128">响应</span><span class="sxs-lookup"><span data-stu-id="53b14-128">Response</span></span>

<span data-ttu-id="53b14-129">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [synchronizationSchema](../resources/synchronization-synchronizationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53b14-129">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53b14-130">示例</span><span class="sxs-lookup"><span data-stu-id="53b14-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="53b14-131">请求</span><span class="sxs-lookup"><span data-stu-id="53b14-131">Request</span></span>
<span data-ttu-id="53b14-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="53b14-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53b14-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="53b14-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="c"></a>[<span data-ttu-id="53b14-134">C#</span><span class="sxs-lookup"><span data-stu-id="53b14-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53b14-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53b14-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53b14-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53b14-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53b14-137">Java</span><span class="sxs-lookup"><span data-stu-id="53b14-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="53b14-138">响应</span><span class="sxs-lookup"><span data-stu-id="53b14-138">Response</span></span>
<span data-ttu-id="53b14-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="53b14-139">The following is an example of a response.</span></span>

><span data-ttu-id="53b14-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53b14-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="53b14-141">在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53b14-141">All the properties will be returned in an actual call.</span></span>
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


