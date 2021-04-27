---
title: 获取 privilegedRole
description: '检索 privilegedRole 对象的属性和关系。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 6eb4838d23ed501ee2875e9aef3484752692584f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055272"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="a0e26-103">获取 privilegedRole</span><span class="sxs-lookup"><span data-stu-id="a0e26-103">Get privilegedRole</span></span>

<span data-ttu-id="a0e26-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0e26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0e26-105">检索 [privilegedRole 对象的属性和](../resources/privilegedrole.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="a0e26-105">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a0e26-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0e26-106">Permissions</span></span>
<span data-ttu-id="a0e26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0e26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a0e26-109">请求程序需要具有以下角色之一 _：Privileged Role Administrator、Global_ _Administrator、Security_ _Administrator_ 或 _Security Reader。_</span><span class="sxs-lookup"><span data-stu-id="a0e26-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="a0e26-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0e26-110">Permission type</span></span>      | <span data-ttu-id="a0e26-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0e26-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0e26-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0e26-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a0e26-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a0e26-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a0e26-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0e26-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0e26-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0e26-115">Not supported.</span></span>    |
|<span data-ttu-id="a0e26-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0e26-116">Application</span></span> | <span data-ttu-id="a0e26-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0e26-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0e26-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0e26-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a0e26-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a0e26-119">Optional query parameters</span></span>
<span data-ttu-id="a0e26-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a0e26-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0e26-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0e26-121">Request headers</span></span>
| <span data-ttu-id="a0e26-122">名称</span><span class="sxs-lookup"><span data-stu-id="a0e26-122">Name</span></span>      |<span data-ttu-id="a0e26-123">说明</span><span class="sxs-lookup"><span data-stu-id="a0e26-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0e26-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0e26-124">Authorization</span></span>  | <span data-ttu-id="a0e26-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0e26-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0e26-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0e26-127">Request body</span></span>
<span data-ttu-id="a0e26-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0e26-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0e26-129">响应</span><span class="sxs-lookup"><span data-stu-id="a0e26-129">Response</span></span>

<span data-ttu-id="a0e26-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [privilegedRole](../resources/privilegedrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0e26-130">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="a0e26-131">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="a0e26-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a0e26-132">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="a0e26-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="a0e26-133">示例</span><span class="sxs-lookup"><span data-stu-id="a0e26-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a0e26-134">请求</span><span class="sxs-lookup"><span data-stu-id="a0e26-134">Request</span></span>
<span data-ttu-id="a0e26-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0e26-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0e26-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0e26-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
# <a name="c"></a>[<span data-ttu-id="a0e26-137">C#</span><span class="sxs-lookup"><span data-stu-id="a0e26-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0e26-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0e26-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0e26-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0e26-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0e26-140">Java</span><span class="sxs-lookup"><span data-stu-id="a0e26-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a0e26-141">响应</span><span class="sxs-lookup"><span data-stu-id="a0e26-141">Response</span></span>
<span data-ttu-id="a0e26-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a0e26-142">Here is an example of the response.</span></span> <span data-ttu-id="a0e26-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a0e26-143">Note: The response object shown here might be shortened for readability.</span></span>
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
