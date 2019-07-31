---
title: 'privilegedRole: selfDeactivate'
description: 停用分配给请求者的角色。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 534d0c178a0c487050a39fa6f1f92a948d477983
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978784"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="ee2c1-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="ee2c1-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee2c1-104">停用分配给请求者的角色。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="ee2c1-105">权限</span><span class="sxs-lookup"><span data-stu-id="ee2c1-105">Permissions</span></span>
<span data-ttu-id="ee2c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ee2c1-108">请求者只能调用```selfDeactivate```分配给他的角色。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="ee2c1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee2c1-109">Permission type</span></span>      | <span data-ttu-id="ee2c1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee2c1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee2c1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee2c1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee2c1-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee2c1-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee2c1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee2c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee2c1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-114">Not supported.</span></span>    |
|<span data-ttu-id="ee2c1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee2c1-115">Application</span></span> | <span data-ttu-id="ee2c1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee2c1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee2c1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="ee2c1-118">请注意``<id>`` , 它是目标角色 id。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ee2c1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee2c1-119">Request headers</span></span>
| <span data-ttu-id="ee2c1-120">名称</span><span class="sxs-lookup"><span data-stu-id="ee2c1-120">Name</span></span>       | <span data-ttu-id="ee2c1-121">说明</span><span class="sxs-lookup"><span data-stu-id="ee2c1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ee2c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee2c1-122">Authorization</span></span>  | <span data-ttu-id="ee2c1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee2c1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee2c1-125">Request body</span></span>
<span data-ttu-id="ee2c1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee2c1-127">响应</span><span class="sxs-lookup"><span data-stu-id="ee2c1-127">Response</span></span>

<span data-ttu-id="ee2c1-128">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="ee2c1-129">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="ee2c1-130">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="ee2c1-131">示例</span><span class="sxs-lookup"><span data-stu-id="ee2c1-131">Example</span></span>
<span data-ttu-id="ee2c1-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ee2c1-133">请求</span><span class="sxs-lookup"><span data-stu-id="ee2c1-133">Request</span></span>
<span data-ttu-id="ee2c1-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ee2c1-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ee2c1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ee2c1-136">C#</span><span class="sxs-lookup"><span data-stu-id="ee2c1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfdeactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee2c1-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ee2c1-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfdeactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ee2c1-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="ee2c1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfdeactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ee2c1-139">Java</span><span class="sxs-lookup"><span data-stu-id="ee2c1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedrole-selfdeactivate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee2c1-140">响应</span><span class="sxs-lookup"><span data-stu-id="ee2c1-140">Response</span></span>
<span data-ttu-id="ee2c1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ee2c1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
