---
title: 获取 privilegedRoleAssignment
description: 检索的属性和 privilegedRoleAssignment 对象的关系。
ms.openlocfilehash: ad8815842698be0ef6a3eef37dc3e26f7dc11dbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043701"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="5bd42-103">获取 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5bd42-103">Get privilegedRoleAssignment</span></span>

> <span data-ttu-id="5bd42-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5bd42-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bd42-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5bd42-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5bd42-106">检索的属性和 privilegedRoleAssignment 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="5bd42-106">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5bd42-107">权限</span><span class="sxs-lookup"><span data-stu-id="5bd42-107">Permissions</span></span>
<span data-ttu-id="5bd42-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bd42-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5bd42-110">请求者需要拥有以下角色之一：_具有权限的角色管理员_、_全局管理员_、_安全管理员_或_安全读取器_。</span><span class="sxs-lookup"><span data-stu-id="5bd42-110">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="5bd42-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bd42-111">Permission type</span></span>      | <span data-ttu-id="5bd42-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5bd42-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bd42-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd42-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5bd42-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5bd42-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5bd42-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd42-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bd42-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bd42-116">Not supported.</span></span>    |
|<span data-ttu-id="5bd42-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5bd42-117">Application</span></span> | <span data-ttu-id="5bd42-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bd42-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bd42-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bd42-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5bd42-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5bd42-120">Optional query parameters</span></span>
<span data-ttu-id="5bd42-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5bd42-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bd42-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bd42-122">Request headers</span></span>
| <span data-ttu-id="5bd42-123">名称</span><span class="sxs-lookup"><span data-stu-id="5bd42-123">Name</span></span>      |<span data-ttu-id="5bd42-124">说明</span><span class="sxs-lookup"><span data-stu-id="5bd42-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5bd42-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd42-125">Authorization</span></span>  | <span data-ttu-id="5bd42-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5bd42-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5bd42-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bd42-128">Request body</span></span>
<span data-ttu-id="5bd42-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5bd42-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bd42-130">响应</span><span class="sxs-lookup"><span data-stu-id="5bd42-130">Response</span></span>

<span data-ttu-id="5bd42-131">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5bd42-131">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="5bd42-132">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="5bd42-132">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="5bd42-133">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="5bd42-133">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="5bd42-134">示例</span><span class="sxs-lookup"><span data-stu-id="5bd42-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5bd42-135">请求</span><span class="sxs-lookup"><span data-stu-id="5bd42-135">Request</span></span>
<span data-ttu-id="5bd42-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5bd42-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="5bd42-137">响应</span><span class="sxs-lookup"><span data-stu-id="5bd42-137">Response</span></span>
<span data-ttu-id="5bd42-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bd42-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->