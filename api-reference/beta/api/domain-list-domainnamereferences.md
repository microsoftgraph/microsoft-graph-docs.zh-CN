---
title: 列出 domainNameReferences
description: 检索包含对域的引用的 directoryObject 列表。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 505c78a9adef3efc2baae05487a46b59d97d6ca6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436545"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="8cf14-103">列出 domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="8cf14-103">List domainNameReferences</span></span>

<span data-ttu-id="8cf14-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cf14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cf14-105">检索包含对域 [的引用的 directoryObject](../resources/directoryobject.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="8cf14-105">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="8cf14-106">返回的列表将包含所有依赖域的目录对象。</span><span class="sxs-lookup"><span data-stu-id="8cf14-106">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cf14-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="8cf14-107">Permissions</span></span>

<span data-ttu-id="8cf14-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cf14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8cf14-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cf14-110">Permission type</span></span>      | <span data-ttu-id="8cf14-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cf14-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cf14-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cf14-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8cf14-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cf14-113">Not supported.</span></span> |
|<span data-ttu-id="8cf14-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cf14-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cf14-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cf14-115">Not supported.</span></span>    |
|<span data-ttu-id="8cf14-116">Application</span><span class="sxs-lookup"><span data-stu-id="8cf14-116">Application</span></span> | <span data-ttu-id="8cf14-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cf14-117">Domain.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8cf14-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cf14-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="8cf14-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="8cf14-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8cf14-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8cf14-120">Optional query parameters</span></span>

<span data-ttu-id="8cf14-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8cf14-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cf14-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cf14-122">Request headers</span></span>

| <span data-ttu-id="8cf14-123">名称</span><span class="sxs-lookup"><span data-stu-id="8cf14-123">Name</span></span>      |<span data-ttu-id="8cf14-124">说明</span><span class="sxs-lookup"><span data-stu-id="8cf14-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8cf14-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cf14-125">Authorization</span></span>  | <span data-ttu-id="8cf14-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8cf14-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cf14-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cf14-128">Request body</span></span>

<span data-ttu-id="8cf14-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8cf14-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cf14-130">响应</span><span class="sxs-lookup"><span data-stu-id="8cf14-130">Response</span></span>

<span data-ttu-id="8cf14-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8cf14-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cf14-132">示例</span><span class="sxs-lookup"><span data-stu-id="8cf14-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8cf14-133">请求</span><span class="sxs-lookup"><span data-stu-id="8cf14-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8cf14-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cf14-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```
# <a name="c"></a>[<span data-ttu-id="8cf14-135">C#</span><span class="sxs-lookup"><span data-stu-id="8cf14-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domainnamereferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cf14-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cf14-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domainnamereferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cf14-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cf14-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domainnamereferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8cf14-138">Java</span><span class="sxs-lookup"><span data-stu-id="8cf14-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domainnamereferences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8cf14-139">响应</span><span class="sxs-lookup"><span data-stu-id="8cf14-139">Response</span></span>
<span data-ttu-id="8cf14-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8cf14-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
