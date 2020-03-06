---
title: 列出 domainNameReferences
description: 使用对域的引用检索 directoryObject 列表。 返回的列表将包含对域具有依赖性的所有目录对象。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 513c36432c828720e90ac015a2bc38a69aecbf0a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517886"
---
# <a name="list-domainnamereferences"></a><span data-ttu-id="8761b-104">列出 domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="8761b-104">List domainNameReferences</span></span>

<span data-ttu-id="8761b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8761b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8761b-106">使用对域的引用检索[directoryObject](../resources/directoryobject.md)列表。</span><span class="sxs-lookup"><span data-stu-id="8761b-106">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain.</span></span> <span data-ttu-id="8761b-107">返回的列表将包含对域具有依赖性的所有目录对象。</span><span class="sxs-lookup"><span data-stu-id="8761b-107">The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="permissions"></a><span data-ttu-id="8761b-108">权限</span><span class="sxs-lookup"><span data-stu-id="8761b-108">Permissions</span></span>

<span data-ttu-id="8761b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8761b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8761b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8761b-111">Permission type</span></span>      | <span data-ttu-id="8761b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8761b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8761b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8761b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8761b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8761b-114">Not supported.</span></span> |
|<span data-ttu-id="8761b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8761b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8761b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8761b-116">Not supported.</span></span>    |
|<span data-ttu-id="8761b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8761b-117">Application</span></span> | <span data-ttu-id="8761b-118">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8761b-118">Domain.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="8761b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8761b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="8761b-120">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="8761b-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8761b-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8761b-121">Optional query parameters</span></span>

<span data-ttu-id="8761b-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8761b-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8761b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="8761b-123">Request headers</span></span>

| <span data-ttu-id="8761b-124">名称</span><span class="sxs-lookup"><span data-stu-id="8761b-124">Name</span></span>      |<span data-ttu-id="8761b-125">说明</span><span class="sxs-lookup"><span data-stu-id="8761b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8761b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="8761b-126">Authorization</span></span>  | <span data-ttu-id="8761b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8761b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8761b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8761b-129">Request body</span></span>

<span data-ttu-id="8761b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8761b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8761b-131">响应</span><span class="sxs-lookup"><span data-stu-id="8761b-131">Response</span></span>

<span data-ttu-id="8761b-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8761b-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8761b-133">示例</span><span class="sxs-lookup"><span data-stu-id="8761b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8761b-134">请求</span><span class="sxs-lookup"><span data-stu-id="8761b-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8761b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8761b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/{domain-name}/domainNameReferences
```
# <a name="c"></a>[<span data-ttu-id="8761b-136">C#</span><span class="sxs-lookup"><span data-stu-id="8761b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domainnamereferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8761b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8761b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domainnamereferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8761b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8761b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domainnamereferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8761b-139">Java</span><span class="sxs-lookup"><span data-stu-id="8761b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domainnamereferences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8761b-140">响应</span><span class="sxs-lookup"><span data-stu-id="8761b-140">Response</span></span>
<span data-ttu-id="8761b-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8761b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
