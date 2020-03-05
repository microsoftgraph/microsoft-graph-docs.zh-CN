---
title: 列出 servicePrincipal 可传递的 memberOf
description: 获取此服务主体所属的组和目录角色。 此操作是可传递的，将包括此服务主体是其嵌套成员的所有组。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: ff520f6c30cc540545d379bc2ef2cd611bd2267d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453423"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="290db-104">列出 servicePrincipal 可传递的 memberOf</span><span class="sxs-lookup"><span data-stu-id="290db-104">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="290db-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="290db-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="290db-106">获取此服务主体所属的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="290db-106">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="290db-107">此操作是可传递的，将包括此服务主体是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="290db-107">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="290db-108">权限</span><span class="sxs-lookup"><span data-stu-id="290db-108">Permissions</span></span>
<span data-ttu-id="290db-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="290db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="290db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="290db-111">Permission type</span></span>      | <span data-ttu-id="290db-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="290db-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="290db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="290db-113">Delegated (work or school account)</span></span> | <span data-ttu-id="290db-114">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="290db-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="290db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="290db-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="290db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="290db-116">Not supported.</span></span>    |
|<span data-ttu-id="290db-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="290db-117">Application</span></span> | <span data-ttu-id="290db-118">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="290db-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="290db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="290db-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="290db-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="290db-120">Optional query parameters</span></span>
<span data-ttu-id="290db-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="290db-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="290db-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="290db-122">Request headers</span></span>
| <span data-ttu-id="290db-123">名称</span><span class="sxs-lookup"><span data-stu-id="290db-123">Name</span></span>       | <span data-ttu-id="290db-124">类型</span><span class="sxs-lookup"><span data-stu-id="290db-124">Type</span></span> | <span data-ttu-id="290db-125">说明</span><span class="sxs-lookup"><span data-stu-id="290db-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="290db-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="290db-126">Authorization</span></span>  | <span data-ttu-id="290db-127">string</span><span class="sxs-lookup"><span data-stu-id="290db-127">string</span></span>  | <span data-ttu-id="290db-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="290db-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="290db-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="290db-130">Request body</span></span>
<span data-ttu-id="290db-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="290db-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="290db-132">响应</span><span class="sxs-lookup"><span data-stu-id="290db-132">Response</span></span>

<span data-ttu-id="290db-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="290db-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="290db-134">示例</span><span class="sxs-lookup"><span data-stu-id="290db-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="290db-135">请求</span><span class="sxs-lookup"><span data-stu-id="290db-135">Request</span></span>

<span data-ttu-id="290db-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="290db-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="290db-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="290db-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="290db-138">C#</span><span class="sxs-lookup"><span data-stu-id="290db-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="290db-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="290db-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="290db-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="290db-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="290db-141">响应</span><span class="sxs-lookup"><span data-stu-id="290db-141">Response</span></span>

<span data-ttu-id="290db-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="290db-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
