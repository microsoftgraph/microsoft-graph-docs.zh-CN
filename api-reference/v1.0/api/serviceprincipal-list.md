---
title: 列出 servicePrincipals
description: 检索 servicePrincipal 对象列表。
author: sureshja
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f7d6064546887a820a4d056d22de40fb084b6d2
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383943"
---
# <a name="list-serviceprincipals"></a><span data-ttu-id="6f00d-103">列出 servicePrincipals</span><span class="sxs-lookup"><span data-stu-id="6f00d-103">List servicePrincipals</span></span>

<span data-ttu-id="6f00d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f00d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f00d-105">检索[servicePrincipal](../resources/serviceprincipal.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6f00d-105">Retrieve a list of [servicePrincipal](../resources/serviceprincipal.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f00d-106">权限</span><span class="sxs-lookup"><span data-stu-id="6f00d-106">Permissions</span></span>

<span data-ttu-id="6f00d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f00d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f00d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f00d-109">Permission type</span></span>      | <span data-ttu-id="6f00d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6f00d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f00d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f00d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6f00d-112">所有的读取全部、全部的 Directory.accessasuser.all、全部、全部、全部、目录、全部、</span><span class="sxs-lookup"><span data-stu-id="6f00d-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6f00d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f00d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f00d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f00d-114">Not supported.</span></span>    |
|<span data-ttu-id="6f00d-115">Application</span><span class="sxs-lookup"><span data-stu-id="6f00d-115">Application</span></span> | <span data-ttu-id="6f00d-116">应用程序。全部，全部读取全部，全部</span><span class="sxs-lookup"><span data-stu-id="6f00d-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f00d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f00d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6f00d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6f00d-118">Optional query parameters</span></span>

<span data-ttu-id="6f00d-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6f00d-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f00d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f00d-120">Request headers</span></span>
| <span data-ttu-id="6f00d-121">名称</span><span class="sxs-lookup"><span data-stu-id="6f00d-121">Name</span></span>           | <span data-ttu-id="6f00d-122">说明</span><span class="sxs-lookup"><span data-stu-id="6f00d-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="6f00d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f00d-123">Authorization</span></span>  | <span data-ttu-id="6f00d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6f00d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6f00d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f00d-126">Request body</span></span>

<span data-ttu-id="6f00d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f00d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f00d-128">响应</span><span class="sxs-lookup"><span data-stu-id="6f00d-128">Response</span></span>

<span data-ttu-id="6f00d-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[servicePrincipal](../resources/serviceprincipal.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6f00d-129">If successful, this method returns a `200 OK` response code and collection of [servicePrincipal](../resources/serviceprincipal.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6f00d-130">示例</span><span class="sxs-lookup"><span data-stu-id="6f00d-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="6f00d-131">请求</span><span class="sxs-lookup"><span data-stu-id="6f00d-131">Request</span></span>
<span data-ttu-id="6f00d-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f00d-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f00d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f00d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/serviceprincipals
```
# <a name="c"></a>[<span data-ttu-id="6f00d-134">C#</span><span class="sxs-lookup"><span data-stu-id="6f00d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f00d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f00d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f00d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f00d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f00d-137">Java</span><span class="sxs-lookup"><span data-stu-id="6f00d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6f00d-138">响应</span><span class="sxs-lookup"><span data-stu-id="6f00d-138">Response</span></span>
<span data-ttu-id="6f00d-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6f00d-139">Here is an example of the response.</span></span> 

> <span data-ttu-id="6f00d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6f00d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [{
        "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
        "deletedDateTime": null,
        "accountEnabled": true,
        "appDisplayName": "My App",
        "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
        "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
        "appRoleAssignmentRequired": false,
        "displayName": "foo",
        "homepage": null,
        "logoutUrl": null,
        "publisherName": "Contoso",
        "replyUrls": [],
        "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
        ],
        "tags": [],
        "addIns": [],
        "appRoles": [],
        "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
        },
        "keyCredentials": [],
        "oauth2PermissionScopes": [],
        "passwordCredentials": []
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipals",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
