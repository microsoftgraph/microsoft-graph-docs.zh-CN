---
title: 获取 synchronizationSchema
description: 检索给定同步作业或模板的架构。
localization_priority: Normal
ms.openlocfilehash: 3b834d955a79c45ef5ae1e43ec9ca0f1fd18cedd
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637960"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="8d981-103">获取 synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="8d981-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d981-104">检索给定同步作业或模板的架构。</span><span class="sxs-lookup"><span data-stu-id="8d981-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d981-105">权限</span><span class="sxs-lookup"><span data-stu-id="8d981-105">Permissions</span></span>
<span data-ttu-id="8d981-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d981-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d981-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d981-108">Permission type</span></span>                        | <span data-ttu-id="8d981-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d981-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d981-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d981-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="8d981-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d981-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8d981-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d981-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8d981-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d981-113">Not supported.</span></span> |
|<span data-ttu-id="8d981-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d981-114">Application</span></span>                            |<span data-ttu-id="8d981-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d981-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8d981-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d981-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="8d981-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d981-117">Request headers</span></span>

| <span data-ttu-id="8d981-118">名称</span><span class="sxs-lookup"><span data-stu-id="8d981-118">Name</span></span>           | <span data-ttu-id="8d981-119">类型</span><span class="sxs-lookup"><span data-stu-id="8d981-119">Type</span></span>    | <span data-ttu-id="8d981-120">说明</span><span class="sxs-lookup"><span data-stu-id="8d981-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8d981-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d981-121">Authorization</span></span>  | <span data-ttu-id="8d981-122">string</span><span class="sxs-lookup"><span data-stu-id="8d981-122">string</span></span>  | <span data-ttu-id="8d981-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d981-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d981-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d981-125">Request body</span></span>

<span data-ttu-id="8d981-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d981-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d981-127">响应</span><span class="sxs-lookup"><span data-stu-id="8d981-127">Response</span></span>

<span data-ttu-id="8d981-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[synchronizationSchema](../resources/synchronization-synchronizationschema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8d981-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d981-129">示例</span><span class="sxs-lookup"><span data-stu-id="8d981-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8d981-130">请求</span><span class="sxs-lookup"><span data-stu-id="8d981-130">Request</span></span>
<span data-ttu-id="8d981-131">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="8d981-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="8d981-132">响应</span><span class="sxs-lookup"><span data-stu-id="8d981-132">Response</span></span>
<span data-ttu-id="8d981-133">响应示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="8d981-133">The following is an example of a response.</span></span>

><span data-ttu-id="8d981-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8d981-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8d981-135">所有属性将在实际调用中返回。</span><span class="sxs-lookup"><span data-stu-id="8d981-135">All the properties will be returned in an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8d981-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8d981-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8d981-137">语言</span><span class="sxs-lookup"><span data-stu-id="8d981-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d981-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d981-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
