---
title: 列出 servicePrincipal memberOf
description: 获取此服务主体是其直接成员的组和目录角色。 此操作不可传递。
localization_priority: Normal
ms.openlocfilehash: b928e64ee7be73ab9dcaa83628924b65445b2330
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269025"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="1a42c-104">列出 servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="1a42c-104">List servicePrincipal memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a42c-105">获取此服务主体是其直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="1a42c-105">Get the groups and directory roles that this service principal is a direct member of.</span></span> <span data-ttu-id="1a42c-106">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="1a42c-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a42c-107">权限</span><span class="sxs-lookup"><span data-stu-id="1a42c-107">Permissions</span></span>

<span data-ttu-id="1a42c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a42c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a42c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a42c-110">Permission type</span></span>      | <span data-ttu-id="1a42c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a42c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a42c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a42c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1a42c-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a42c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a42c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a42c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a42c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a42c-115">Not supported.</span></span>    |
|<span data-ttu-id="1a42c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a42c-116">Application</span></span> | <span data-ttu-id="1a42c-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a42c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a42c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a42c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a42c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1a42c-119">Optional query parameters</span></span>

<span data-ttu-id="1a42c-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1a42c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a42c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a42c-121">Request headers</span></span>
| <span data-ttu-id="1a42c-122">名称</span><span class="sxs-lookup"><span data-stu-id="1a42c-122">Name</span></span>       | <span data-ttu-id="1a42c-123">类型</span><span class="sxs-lookup"><span data-stu-id="1a42c-123">Type</span></span> | <span data-ttu-id="1a42c-124">说明</span><span class="sxs-lookup"><span data-stu-id="1a42c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a42c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a42c-125">Authorization</span></span>  | <span data-ttu-id="1a42c-126">string</span><span class="sxs-lookup"><span data-stu-id="1a42c-126">string</span></span>  | <span data-ttu-id="1a42c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a42c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a42c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a42c-129">Request body</span></span>
<span data-ttu-id="1a42c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a42c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a42c-131">响应</span><span class="sxs-lookup"><span data-stu-id="1a42c-131">Response</span></span>

<span data-ttu-id="1a42c-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a42c-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a42c-133">示例</span><span class="sxs-lookup"><span data-stu-id="1a42c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a42c-134">请求</span><span class="sxs-lookup"><span data-stu-id="1a42c-134">Request</span></span>

<span data-ttu-id="1a42c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a42c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="1a42c-136">响应</span><span class="sxs-lookup"><span data-stu-id="1a42c-136">Response</span></span>

<span data-ttu-id="1a42c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a42c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1a42c-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1a42c-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1a42c-141">C#</span><span class="sxs-lookup"><span data-stu-id="1a42c-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_serviceprincipal_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a42c-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a42c-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_serviceprincipal_memberof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1a42c-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="1a42c-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_serviceprincipal_memberof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/serviceprincipal-list-memberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/serviceprincipal-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
