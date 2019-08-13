---
title: 列出 privilegedRoles
description: 检索 privilegedRole 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 73db2d842a1ca11c05d7bb4d9fb0b671d6636133
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361204"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="c9b5b-103">列出 privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="c9b5b-103">List privilegedRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9b5b-104">检索[privilegedRole](../resources/privilegedrole.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-104">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="c9b5b-105">若要筛选查询中的结果，请在 URL 中使用标准 OData ``$filter`` 表达式。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9b5b-106">权限</span><span class="sxs-lookup"><span data-stu-id="c9b5b-106">Permissions</span></span>
<span data-ttu-id="c9b5b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c9b5b-109">请求者需要具有以下角色之一:_特权角色管理员_、_全局管理员_、_安全管理员_或_安全读者_。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="c9b5b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9b5b-110">Permission type</span></span>      | <span data-ttu-id="c9b5b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9b5b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9b5b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9b5b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c9b5b-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c9b5b-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c9b5b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9b5b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9b5b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-115">Not supported.</span></span>    |
|<span data-ttu-id="c9b5b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9b5b-116">Application</span></span> | <span data-ttu-id="c9b5b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9b5b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9b5b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c9b5b-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c9b5b-119">Optional query parameters</span></span>
<span data-ttu-id="c9b5b-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9b5b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9b5b-121">Request headers</span></span>
| <span data-ttu-id="c9b5b-122">名称</span><span class="sxs-lookup"><span data-stu-id="c9b5b-122">Name</span></span>      |<span data-ttu-id="c9b5b-123">说明</span><span class="sxs-lookup"><span data-stu-id="c9b5b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c9b5b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9b5b-124">Authorization</span></span>  | <span data-ttu-id="c9b5b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9b5b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9b5b-127">Request body</span></span>
<span data-ttu-id="c9b5b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9b5b-129">响应</span><span class="sxs-lookup"><span data-stu-id="c9b5b-129">Response</span></span>

<span data-ttu-id="c9b5b-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedRole](../resources/privilegedrole.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="c9b5b-131">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c9b5b-132">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c9b5b-133">示例</span><span class="sxs-lookup"><span data-stu-id="c9b5b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9b5b-134">请求</span><span class="sxs-lookup"><span data-stu-id="c9b5b-134">Request</span></span>
<span data-ttu-id="c9b5b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c9b5b-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c9b5b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9b5b-137">C#</span><span class="sxs-lookup"><span data-stu-id="c9b5b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9b5b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9b5b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9b5b-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="c9b5b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c9b5b-140">Java</span><span class="sxs-lookup"><span data-stu-id="c9b5b-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c9b5b-141">响应</span><span class="sxs-lookup"><span data-stu-id="c9b5b-141">Response</span></span>
<span data-ttu-id="c9b5b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9b5b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
