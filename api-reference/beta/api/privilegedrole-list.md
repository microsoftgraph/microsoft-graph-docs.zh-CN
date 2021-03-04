---
title: 列出 privilegedRoles
description: 检索 privilegedRole 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 1567b4fbf3d1be3be85b309e2b6edab05e90828d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441314"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="75f4f-103">列出 privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="75f4f-103">List privilegedRoles</span></span>

<span data-ttu-id="75f4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75f4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75f4f-105">检索 [privilegedRole 对象](../resources/privilegedrole.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="75f4f-105">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="75f4f-106">若要筛选查询中的结果，请在 URL 中使用标准 OData ``$filter`` 表达式。</span><span class="sxs-lookup"><span data-stu-id="75f4f-106">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="75f4f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="75f4f-107">Permissions</span></span>
<span data-ttu-id="75f4f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="75f4f-110">请求者需要具有以下角色之一 _：Privileged Role Administrator、Global_ _Administrator、Security_ _Administrator_ 或 _Security Reader。_</span><span class="sxs-lookup"><span data-stu-id="75f4f-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="75f4f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="75f4f-111">Permission type</span></span>      | <span data-ttu-id="75f4f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75f4f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75f4f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75f4f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="75f4f-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="75f4f-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="75f4f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75f4f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75f4f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="75f4f-116">Not supported.</span></span>    |
|<span data-ttu-id="75f4f-117">Application</span><span class="sxs-lookup"><span data-stu-id="75f4f-117">Application</span></span> | <span data-ttu-id="75f4f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="75f4f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75f4f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75f4f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="75f4f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="75f4f-120">Optional query parameters</span></span>
<span data-ttu-id="75f4f-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="75f4f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75f4f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="75f4f-122">Request headers</span></span>
| <span data-ttu-id="75f4f-123">名称</span><span class="sxs-lookup"><span data-stu-id="75f4f-123">Name</span></span>      |<span data-ttu-id="75f4f-124">说明</span><span class="sxs-lookup"><span data-stu-id="75f4f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="75f4f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="75f4f-125">Authorization</span></span>  | <span data-ttu-id="75f4f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75f4f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75f4f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="75f4f-128">Request body</span></span>
<span data-ttu-id="75f4f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="75f4f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75f4f-130">响应</span><span class="sxs-lookup"><span data-stu-id="75f4f-130">Response</span></span>

<span data-ttu-id="75f4f-131">如果成功，此方法在响应正文中返回 `200 OK` [响应代码和 privilegedRole](../resources/privilegedrole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="75f4f-131">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="75f4f-132">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="75f4f-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="75f4f-133">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="75f4f-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="75f4f-134">示例</span><span class="sxs-lookup"><span data-stu-id="75f4f-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="75f4f-135">请求</span><span class="sxs-lookup"><span data-stu-id="75f4f-135">Request</span></span>
<span data-ttu-id="75f4f-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75f4f-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75f4f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="75f4f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="c"></a>[<span data-ttu-id="75f4f-138">C#</span><span class="sxs-lookup"><span data-stu-id="75f4f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75f4f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75f4f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75f4f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75f4f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75f4f-141">Java</span><span class="sxs-lookup"><span data-stu-id="75f4f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="75f4f-142">响应</span><span class="sxs-lookup"><span data-stu-id="75f4f-142">Response</span></span>
<span data-ttu-id="75f4f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75f4f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
