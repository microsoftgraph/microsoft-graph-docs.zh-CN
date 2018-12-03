---
title: 列表分配
description: 检索与角色相关联的 privilegedRoleAssignment 对象的列表。 每个 privilegedRoleAssignment 代表角色分配给用户。
ms.openlocfilehash: 52cc720381baa6b7c82fe3b5c88d469081da3b81
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046197"
---
# <a name="list-assignments"></a><span data-ttu-id="41151-104">列表分配</span><span class="sxs-lookup"><span data-stu-id="41151-104">List assignments</span></span>

> <span data-ttu-id="41151-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="41151-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41151-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="41151-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41151-107">检索与角色相关联的[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="41151-107">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects that are associated with the role.</span></span> <span data-ttu-id="41151-108">每个[privilegedRoleAssignment](../resources/privilegedroleassignment.md)代表角色分配给用户。</span><span class="sxs-lookup"><span data-stu-id="41151-108">Each [privilegedRoleAssignment](../resources/privilegedroleassignment.md) represents a role assignment to a user.</span></span>
## <a name="permissions"></a><span data-ttu-id="41151-109">权限</span><span class="sxs-lookup"><span data-stu-id="41151-109">Permissions</span></span>
<span data-ttu-id="41151-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41151-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="41151-112">请求者需要拥有以下角色之一：_具有权限的角色管理员_、_全局管理员_、_安全管理员_或_安全读取器_。</span><span class="sxs-lookup"><span data-stu-id="41151-112">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="41151-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="41151-113">Permission type</span></span>      | <span data-ttu-id="41151-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41151-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41151-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41151-115">Delegated (work or school account)</span></span> | <span data-ttu-id="41151-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41151-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41151-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41151-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41151-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="41151-118">Not supported.</span></span>    |
|<span data-ttu-id="41151-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="41151-119">Application</span></span> | <span data-ttu-id="41151-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="41151-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41151-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41151-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}/assignments
```

<span data-ttu-id="41151-122">请注意，``<id>``是目标角色 id。</span><span class="sxs-lookup"><span data-stu-id="41151-122">Note that ``<id>`` is the target role id.</span></span>
## <a name="optional-query-parameters"></a><span data-ttu-id="41151-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41151-123">Optional query parameters</span></span>
<span data-ttu-id="41151-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="41151-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41151-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="41151-125">Request headers</span></span>
| <span data-ttu-id="41151-126">名称</span><span class="sxs-lookup"><span data-stu-id="41151-126">Name</span></span>      |<span data-ttu-id="41151-127">说明</span><span class="sxs-lookup"><span data-stu-id="41151-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41151-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="41151-128">Authorization</span></span>  | <span data-ttu-id="41151-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41151-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41151-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="41151-131">Request body</span></span>
<span data-ttu-id="41151-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41151-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41151-133">响应</span><span class="sxs-lookup"><span data-stu-id="41151-133">Response</span></span>

<span data-ttu-id="41151-134">如果成功，此方法返回`200 OK`响应代码和响应正文中的[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="41151-134">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="41151-135">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="41151-135">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="41151-136">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="41151-136">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="41151-137">示例</span><span class="sxs-lookup"><span data-stu-id="41151-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41151-138">请求</span><span class="sxs-lookup"><span data-stu-id="41151-138">Request</span></span>
<span data-ttu-id="41151-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41151-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}/assignments
```
##### <a name="response"></a><span data-ttu-id="41151-140">响应</span><span class="sxs-lookup"><span data-stu-id="41151-140">Response</span></span>
<span data-ttu-id="41151-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41151-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
