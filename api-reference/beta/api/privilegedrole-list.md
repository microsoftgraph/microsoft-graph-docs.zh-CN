---
title: 列出 privilegedRoles
description: 检索 privilegedRole 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 83125ee854fc75fe3e5c8d233df3013ceaadcd51
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315005"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="5f9cb-103">列出 privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="5f9cb-103">List privilegedRoles</span></span>

<span data-ttu-id="5f9cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f9cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f9cb-105">检索 [privilegedRole](../resources/privilegedrole.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-105">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="5f9cb-106">若要筛选查询中的结果，请在 URL 中使用标准 OData ``$filter`` 表达式。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="5f9cb-107">权限</span><span class="sxs-lookup"><span data-stu-id="5f9cb-107">Permissions</span></span>
<span data-ttu-id="5f9cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5f9cb-110">请求者需要具有以下角色之一： _特权角色管理员_、 _全局管理员_、 _安全管理员_或 _安全读者_。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="5f9cb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f9cb-111">Permission type</span></span>      | <span data-ttu-id="5f9cb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f9cb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f9cb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f9cb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5f9cb-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5f9cb-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5f9cb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f9cb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f9cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-116">Not supported.</span></span>    |
|<span data-ttu-id="5f9cb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f9cb-117">Application</span></span> | <span data-ttu-id="5f9cb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f9cb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f9cb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5f9cb-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5f9cb-120">Optional query parameters</span></span>
<span data-ttu-id="5f9cb-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f9cb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f9cb-122">Request headers</span></span>
| <span data-ttu-id="5f9cb-123">名称</span><span class="sxs-lookup"><span data-stu-id="5f9cb-123">Name</span></span>      |<span data-ttu-id="5f9cb-124">说明</span><span class="sxs-lookup"><span data-stu-id="5f9cb-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f9cb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f9cb-125">Authorization</span></span>  | <span data-ttu-id="5f9cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f9cb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f9cb-128">Request body</span></span>
<span data-ttu-id="5f9cb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f9cb-130">响应</span><span class="sxs-lookup"><span data-stu-id="5f9cb-130">Response</span></span>

<span data-ttu-id="5f9cb-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [privilegedRole](../resources/privilegedrole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="5f9cb-132">请注意，需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5f9cb-133">否则，将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="5f9cb-134">示例</span><span class="sxs-lookup"><span data-stu-id="5f9cb-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f9cb-135">请求</span><span class="sxs-lookup"><span data-stu-id="5f9cb-135">Request</span></span>
<span data-ttu-id="5f9cb-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5f9cb-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f9cb-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="c"></a>[<span data-ttu-id="5f9cb-138">C#</span><span class="sxs-lookup"><span data-stu-id="5f9cb-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f9cb-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f9cb-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f9cb-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f9cb-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5f9cb-141">响应</span><span class="sxs-lookup"><span data-stu-id="5f9cb-141">Response</span></span>
<span data-ttu-id="5f9cb-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f9cb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->