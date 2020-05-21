---
title: 列出 servicePrincipal memberOf
description: 获取此服务主体是其直接成员的组和目录角色。 此操作不可传递。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 7ead981f3bd7402fbe8b28c4b7ac8855e32fa74c
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335932"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="37e3e-104">列出 servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="37e3e-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="37e3e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e3e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37e3e-106">获取此[servicePrincipal](../resources/serviceprincipal.md)是其直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="37e3e-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="37e3e-107">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="37e3e-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="37e3e-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="37e3e-108">Permissions</span></span>

<span data-ttu-id="37e3e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37e3e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37e3e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="37e3e-111">Permission type</span></span>      | <span data-ttu-id="37e3e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37e3e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37e3e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37e3e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="37e3e-114">所有的读取全部、全部的 Directory.accessasuser.all、全部、全部、全部、目录、全部、</span><span class="sxs-lookup"><span data-stu-id="37e3e-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="37e3e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37e3e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37e3e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="37e3e-116">Not supported.</span></span>    |
|<span data-ttu-id="37e3e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="37e3e-117">Application</span></span> | <span data-ttu-id="37e3e-118">应用程序。全部，全部读取全部，全部为，全部为。</span><span class="sxs-lookup"><span data-stu-id="37e3e-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="37e3e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37e3e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37e3e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="37e3e-120">Optional query parameters</span></span>

<span data-ttu-id="37e3e-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="37e3e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37e3e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="37e3e-122">Request headers</span></span>
| <span data-ttu-id="37e3e-123">名称</span><span class="sxs-lookup"><span data-stu-id="37e3e-123">Name</span></span>           | <span data-ttu-id="37e3e-124">说明</span><span class="sxs-lookup"><span data-stu-id="37e3e-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="37e3e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="37e3e-125">Authorization</span></span>  | <span data-ttu-id="37e3e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37e3e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="37e3e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="37e3e-128">Request body</span></span>
<span data-ttu-id="37e3e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="37e3e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37e3e-130">响应</span><span class="sxs-lookup"><span data-stu-id="37e3e-130">Response</span></span>

<span data-ttu-id="37e3e-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="37e3e-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37e3e-132">示例</span><span class="sxs-lookup"><span data-stu-id="37e3e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37e3e-133">请求</span><span class="sxs-lookup"><span data-stu-id="37e3e-133">Request</span></span>

<span data-ttu-id="37e3e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37e3e-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="37e3e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="37e3e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="37e3e-136">C#</span><span class="sxs-lookup"><span data-stu-id="37e3e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37e3e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37e3e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37e3e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37e3e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37e3e-139">Java</span><span class="sxs-lookup"><span data-stu-id="37e3e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37e3e-140">响应</span><span class="sxs-lookup"><span data-stu-id="37e3e-140">Response</span></span>

<span data-ttu-id="37e3e-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="37e3e-141">Here is an example of the response.</span></span> 
><span data-ttu-id="37e3e-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37e3e-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
