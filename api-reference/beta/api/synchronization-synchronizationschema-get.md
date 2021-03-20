---
title: 获取 synchronizationSchema
description: 检索给定同步作业或模板的架构。
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: bd321f3375623914afa6cc9c803b18e2a22d1ed4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952946"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="c61b3-103">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="c61b3-103">Get synchronizationSchema</span></span>

<span data-ttu-id="c61b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c61b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c61b3-105">检索给定同步作业或模板的架构。</span><span class="sxs-lookup"><span data-stu-id="c61b3-105">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="c61b3-106">权限</span><span class="sxs-lookup"><span data-stu-id="c61b3-106">Permissions</span></span>
<span data-ttu-id="c61b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c61b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c61b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c61b3-109">Permission type</span></span>                        | <span data-ttu-id="c61b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c61b3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c61b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c61b3-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="c61b3-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c61b3-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="c61b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c61b3-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c61b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c61b3-114">Not supported.</span></span> |
|<span data-ttu-id="c61b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c61b3-115">Application</span></span>                            |<span data-ttu-id="c61b3-116">Application.ReadWrite.OwnedBy、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c61b3-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c61b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c61b3-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="c61b3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c61b3-118">Request headers</span></span>

| <span data-ttu-id="c61b3-119">名称</span><span class="sxs-lookup"><span data-stu-id="c61b3-119">Name</span></span>           | <span data-ttu-id="c61b3-120">类型</span><span class="sxs-lookup"><span data-stu-id="c61b3-120">Type</span></span>    | <span data-ttu-id="c61b3-121">说明</span><span class="sxs-lookup"><span data-stu-id="c61b3-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c61b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c61b3-122">Authorization</span></span>  | <span data-ttu-id="c61b3-123">string</span><span class="sxs-lookup"><span data-stu-id="c61b3-123">string</span></span>  | <span data-ttu-id="c61b3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c61b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c61b3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c61b3-126">Request body</span></span>

<span data-ttu-id="c61b3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c61b3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c61b3-128">响应</span><span class="sxs-lookup"><span data-stu-id="c61b3-128">Response</span></span>

<span data-ttu-id="c61b3-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [synchronizationSchema](../resources/synchronization-synchronizationschema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c61b3-129">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c61b3-130">示例</span><span class="sxs-lookup"><span data-stu-id="c61b3-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c61b3-131">请求</span><span class="sxs-lookup"><span data-stu-id="c61b3-131">Request</span></span>
<span data-ttu-id="c61b3-132">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="c61b3-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c61b3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c61b3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="c"></a>[<span data-ttu-id="c61b3-134">C#</span><span class="sxs-lookup"><span data-stu-id="c61b3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c61b3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c61b3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c61b3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c61b3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c61b3-137">Java</span><span class="sxs-lookup"><span data-stu-id="c61b3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c61b3-138">响应</span><span class="sxs-lookup"><span data-stu-id="c61b3-138">Response</span></span>
<span data-ttu-id="c61b3-139">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="c61b3-139">The following is an example of a response.</span></span>

><span data-ttu-id="c61b3-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c61b3-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c61b3-141">在实际调用中将返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c61b3-141">All the properties will be returned in an actual call.</span></span>
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


