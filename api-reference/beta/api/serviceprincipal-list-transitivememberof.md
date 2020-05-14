---
title: 列出 servicePrincipal 可传递的 memberOf
description: 获取此服务主体所属的组和目录角色。 此操作是可传递的，将包括此服务主体是其嵌套成员的所有组。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 8ddbb893b5fcc821ea0187e8bfbc5b0c814309b9
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2020
ms.locfileid: "44226915"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="dcb6f-104">列出 servicePrincipal 可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="dcb6f-104">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="dcb6f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcb6f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcb6f-106">获取此服务主体所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-106">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="dcb6f-107">此操作是可传递的，将包括此服务主体是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-107">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcb6f-108">权限</span><span class="sxs-lookup"><span data-stu-id="dcb6f-108">Permissions</span></span>
<span data-ttu-id="dcb6f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcb6f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcb6f-111">Permission type</span></span>      | <span data-ttu-id="dcb6f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcb6f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcb6f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcb6f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dcb6f-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dcb6f-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dcb6f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcb6f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcb6f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-116">Not supported.</span></span>    |
|<span data-ttu-id="dcb6f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcb6f-117">Application</span></span> | <span data-ttu-id="dcb6f-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcb6f-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="dcb6f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcb6f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dcb6f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dcb6f-120">Optional query parameters</span></span>
<span data-ttu-id="dcb6f-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcb6f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcb6f-122">Request headers</span></span>
| <span data-ttu-id="dcb6f-123">名称</span><span class="sxs-lookup"><span data-stu-id="dcb6f-123">Name</span></span>       | <span data-ttu-id="dcb6f-124">类型</span><span class="sxs-lookup"><span data-stu-id="dcb6f-124">Type</span></span> | <span data-ttu-id="dcb6f-125">说明</span><span class="sxs-lookup"><span data-stu-id="dcb6f-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="dcb6f-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcb6f-126">Authorization</span></span>  | <span data-ttu-id="dcb6f-127">string</span><span class="sxs-lookup"><span data-stu-id="dcb6f-127">string</span></span>  | <span data-ttu-id="dcb6f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcb6f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcb6f-130">Request body</span></span>
<span data-ttu-id="dcb6f-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcb6f-132">响应</span><span class="sxs-lookup"><span data-stu-id="dcb6f-132">Response</span></span>

<span data-ttu-id="dcb6f-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcb6f-134">示例</span><span class="sxs-lookup"><span data-stu-id="dcb6f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcb6f-135">请求</span><span class="sxs-lookup"><span data-stu-id="dcb6f-135">Request</span></span>

<span data-ttu-id="dcb6f-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcb6f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcb6f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="dcb6f-138">C#</span><span class="sxs-lookup"><span data-stu-id="dcb6f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcb6f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcb6f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcb6f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcb6f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dcb6f-141">响应</span><span class="sxs-lookup"><span data-stu-id="dcb6f-141">Response</span></span>

<span data-ttu-id="dcb6f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dcb6f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List servicePrincipal transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
