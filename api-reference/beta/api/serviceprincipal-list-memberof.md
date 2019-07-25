---
title: 列出 servicePrincipal memberOf
description: 获取此服务主体是其直接成员的组和目录角色。 此操作不可传递。
localization_priority: Normal
ms.openlocfilehash: f58210131c0ae8e107f5e4f4f7361cf741aec8b7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870041"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="19d4e-104">列出 servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="19d4e-104">List servicePrincipal memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19d4e-105">获取此服务主体是其直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="19d4e-105">Get the groups and directory roles that this service principal is a direct member of.</span></span> <span data-ttu-id="19d4e-106">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="19d4e-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="19d4e-107">权限</span><span class="sxs-lookup"><span data-stu-id="19d4e-107">Permissions</span></span>

<span data-ttu-id="19d4e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19d4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19d4e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="19d4e-110">Permission type</span></span>      | <span data-ttu-id="19d4e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19d4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19d4e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19d4e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19d4e-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19d4e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19d4e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19d4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19d4e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="19d4e-115">Not supported.</span></span>    |
|<span data-ttu-id="19d4e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="19d4e-116">Application</span></span> | <span data-ttu-id="19d4e-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19d4e-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19d4e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19d4e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19d4e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19d4e-119">Optional query parameters</span></span>

<span data-ttu-id="19d4e-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19d4e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19d4e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="19d4e-121">Request headers</span></span>
| <span data-ttu-id="19d4e-122">名称</span><span class="sxs-lookup"><span data-stu-id="19d4e-122">Name</span></span>       | <span data-ttu-id="19d4e-123">类型</span><span class="sxs-lookup"><span data-stu-id="19d4e-123">Type</span></span> | <span data-ttu-id="19d4e-124">说明</span><span class="sxs-lookup"><span data-stu-id="19d4e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="19d4e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="19d4e-125">Authorization</span></span>  | <span data-ttu-id="19d4e-126">string</span><span class="sxs-lookup"><span data-stu-id="19d4e-126">string</span></span>  | <span data-ttu-id="19d4e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19d4e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19d4e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="19d4e-129">Request body</span></span>
<span data-ttu-id="19d4e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19d4e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19d4e-131">响应</span><span class="sxs-lookup"><span data-stu-id="19d4e-131">Response</span></span>

<span data-ttu-id="19d4e-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="19d4e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19d4e-133">示例</span><span class="sxs-lookup"><span data-stu-id="19d4e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="19d4e-134">请求</span><span class="sxs-lookup"><span data-stu-id="19d4e-134">Request</span></span>

<span data-ttu-id="19d4e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19d4e-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="19d4e-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="19d4e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19d4e-137">C#</span><span class="sxs-lookup"><span data-stu-id="19d4e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19d4e-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="19d4e-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19d4e-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="19d4e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="19d4e-140">Java</span><span class="sxs-lookup"><span data-stu-id="19d4e-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-serviceprincipal-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="19d4e-141">响应</span><span class="sxs-lookup"><span data-stu-id="19d4e-141">Response</span></span>

<span data-ttu-id="19d4e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19d4e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
