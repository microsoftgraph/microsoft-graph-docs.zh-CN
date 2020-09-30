---
title: 获取 privilegedRoleAssignment
description: 检索 privilegedRoleAssignment 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 243e7bd118830ff42b337c0dca64bac9404679cc
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314900"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="0aed1-103">获取 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0aed1-103">Get privilegedRoleAssignment</span></span>

<span data-ttu-id="0aed1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aed1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aed1-105">检索 privilegedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0aed1-105">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0aed1-106">权限</span><span class="sxs-lookup"><span data-stu-id="0aed1-106">Permissions</span></span>
<span data-ttu-id="0aed1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0aed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0aed1-109">请求者需要具有以下角色之一： _特权角色管理员_、 _全局管理员_、 _安全管理员_或 _安全读者_。</span><span class="sxs-lookup"><span data-stu-id="0aed1-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="0aed1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0aed1-110">Permission type</span></span>      | <span data-ttu-id="0aed1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0aed1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aed1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0aed1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0aed1-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0aed1-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0aed1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0aed1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aed1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0aed1-115">Not supported.</span></span>    |
|<span data-ttu-id="0aed1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0aed1-116">Application</span></span> | <span data-ttu-id="0aed1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0aed1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0aed1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0aed1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0aed1-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0aed1-119">Optional query parameters</span></span>
<span data-ttu-id="0aed1-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0aed1-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0aed1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0aed1-121">Request headers</span></span>
| <span data-ttu-id="0aed1-122">名称</span><span class="sxs-lookup"><span data-stu-id="0aed1-122">Name</span></span>      |<span data-ttu-id="0aed1-123">说明</span><span class="sxs-lookup"><span data-stu-id="0aed1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0aed1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0aed1-124">Authorization</span></span>  | <span data-ttu-id="0aed1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0aed1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0aed1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0aed1-127">Request body</span></span>
<span data-ttu-id="0aed1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0aed1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0aed1-129">响应</span><span class="sxs-lookup"><span data-stu-id="0aed1-129">Response</span></span>

<span data-ttu-id="0aed1-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0aed1-130">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="0aed1-131">请注意，需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="0aed1-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="0aed1-132">否则，将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="0aed1-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="0aed1-133">示例</span><span class="sxs-lookup"><span data-stu-id="0aed1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0aed1-134">请求</span><span class="sxs-lookup"><span data-stu-id="0aed1-134">Request</span></span>
<span data-ttu-id="0aed1-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0aed1-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0aed1-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0aed1-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="0aed1-137">C#</span><span class="sxs-lookup"><span data-stu-id="0aed1-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0aed1-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0aed1-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0aed1-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0aed1-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0aed1-140">响应</span><span class="sxs-lookup"><span data-stu-id="0aed1-140">Response</span></span>
<span data-ttu-id="0aed1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0aed1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->