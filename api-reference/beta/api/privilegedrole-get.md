---
title: 获取 privilegedRole
description: '检索 privilegedRole 对象的属性和关系。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 64cc3fe214149d61f8f8cbd43fabc0ef1d3b81e3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441338"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="6440d-103">获取 privilegedRole</span><span class="sxs-lookup"><span data-stu-id="6440d-103">Get privilegedRole</span></span>

<span data-ttu-id="6440d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6440d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6440d-105">检索 [privilegedRole 对象的属性和](../resources/privilegedrole.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="6440d-105">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6440d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6440d-106">Permissions</span></span>
<span data-ttu-id="6440d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6440d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6440d-109">请求者需要具有以下角色之一 _：Privileged Role Administrator、Global_ _Administrator、Security_ _Administrator_ 或 _Security Reader。_</span><span class="sxs-lookup"><span data-stu-id="6440d-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="6440d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6440d-110">Permission type</span></span>      | <span data-ttu-id="6440d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6440d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6440d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6440d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6440d-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6440d-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6440d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6440d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6440d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6440d-115">Not supported.</span></span>    |
|<span data-ttu-id="6440d-116">Application</span><span class="sxs-lookup"><span data-stu-id="6440d-116">Application</span></span> | <span data-ttu-id="6440d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6440d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6440d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6440d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6440d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6440d-119">Optional query parameters</span></span>
<span data-ttu-id="6440d-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6440d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6440d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6440d-121">Request headers</span></span>
| <span data-ttu-id="6440d-122">名称</span><span class="sxs-lookup"><span data-stu-id="6440d-122">Name</span></span>      |<span data-ttu-id="6440d-123">说明</span><span class="sxs-lookup"><span data-stu-id="6440d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6440d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6440d-124">Authorization</span></span>  | <span data-ttu-id="6440d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6440d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6440d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6440d-127">Request body</span></span>
<span data-ttu-id="6440d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6440d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6440d-129">响应</span><span class="sxs-lookup"><span data-stu-id="6440d-129">Response</span></span>

<span data-ttu-id="6440d-130">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [privilegedRole](../resources/privilegedrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6440d-130">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="6440d-131">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="6440d-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6440d-132">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="6440d-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6440d-133">示例</span><span class="sxs-lookup"><span data-stu-id="6440d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6440d-134">请求</span><span class="sxs-lookup"><span data-stu-id="6440d-134">Request</span></span>
<span data-ttu-id="6440d-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6440d-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6440d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="6440d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="6440d-137">C#</span><span class="sxs-lookup"><span data-stu-id="6440d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6440d-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6440d-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6440d-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6440d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6440d-140">Java</span><span class="sxs-lookup"><span data-stu-id="6440d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6440d-141">响应</span><span class="sxs-lookup"><span data-stu-id="6440d-141">Response</span></span>
<span data-ttu-id="6440d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6440d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
