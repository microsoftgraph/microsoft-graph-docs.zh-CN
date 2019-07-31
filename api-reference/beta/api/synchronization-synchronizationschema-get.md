---
title: 获取 synchronizationSchema
description: 检索给定同步作业或模板的架构。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55f6b6935808cd96bf9eebf8e2662d0649bbb66c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977665"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="5bceb-103">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="5bceb-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bceb-104">检索给定同步作业或模板的架构。</span><span class="sxs-lookup"><span data-stu-id="5bceb-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bceb-105">权限</span><span class="sxs-lookup"><span data-stu-id="5bceb-105">Permissions</span></span>
<span data-ttu-id="5bceb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bceb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bceb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bceb-108">Permission type</span></span>                        | <span data-ttu-id="5bceb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5bceb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bceb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bceb-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="5bceb-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5bceb-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="5bceb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bceb-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="5bceb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bceb-113">Not supported.</span></span> |
|<span data-ttu-id="5bceb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bceb-114">Application</span></span>                            |<span data-ttu-id="5bceb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bceb-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5bceb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bceb-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="5bceb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bceb-117">Request headers</span></span>

| <span data-ttu-id="5bceb-118">名称</span><span class="sxs-lookup"><span data-stu-id="5bceb-118">Name</span></span>           | <span data-ttu-id="5bceb-119">类型</span><span class="sxs-lookup"><span data-stu-id="5bceb-119">Type</span></span>    | <span data-ttu-id="5bceb-120">说明</span><span class="sxs-lookup"><span data-stu-id="5bceb-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="5bceb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bceb-121">Authorization</span></span>  | <span data-ttu-id="5bceb-122">string</span><span class="sxs-lookup"><span data-stu-id="5bceb-122">string</span></span>  | <span data-ttu-id="5bceb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5bceb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bceb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bceb-125">Request body</span></span>

<span data-ttu-id="5bceb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5bceb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bceb-127">响应</span><span class="sxs-lookup"><span data-stu-id="5bceb-127">Response</span></span>

<span data-ttu-id="5bceb-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[synchronizationSchema](../resources/synchronization-synchronizationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5bceb-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bceb-129">示例</span><span class="sxs-lookup"><span data-stu-id="5bceb-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5bceb-130">请求</span><span class="sxs-lookup"><span data-stu-id="5bceb-130">Request</span></span>
<span data-ttu-id="5bceb-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="5bceb-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5bceb-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5bceb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5bceb-133">C#</span><span class="sxs-lookup"><span data-stu-id="5bceb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bceb-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bceb-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5bceb-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="5bceb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5bceb-136">Java</span><span class="sxs-lookup"><span data-stu-id="5bceb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5bceb-137">响应</span><span class="sxs-lookup"><span data-stu-id="5bceb-137">Response</span></span>
<span data-ttu-id="5bceb-138">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="5bceb-138">The following is an example of a response.</span></span>

><span data-ttu-id="5bceb-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5bceb-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5bceb-140">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="5bceb-140">All the properties will be returned in an actual call.</span></span>
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
