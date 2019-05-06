---
title: 获取 privilegedRoleAssignment
description: 检索 privilegedRoleAssignment 对象的属性和关系。
localization_priority: Normal
ms.openlocfilehash: 1ebdf020fc3f534ec62edb345748869bd46f42d4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594632"
---
# <a name="get-privilegedroleassignment"></a><span data-ttu-id="f33a2-103">获取 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="f33a2-103">Get privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f33a2-104">检索 privilegedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f33a2-104">Retrieve the properties and relationships of privilegedRoleAssignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f33a2-105">权限</span><span class="sxs-lookup"><span data-stu-id="f33a2-105">Permissions</span></span>
<span data-ttu-id="f33a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f33a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f33a2-108">请求者需要具有以下角色之一:_特权角色管理员_、_全局管理员_、_安全管理员_或_安全读者_。</span><span class="sxs-lookup"><span data-stu-id="f33a2-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="f33a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f33a2-109">Permission type</span></span>      | <span data-ttu-id="f33a2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f33a2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f33a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f33a2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f33a2-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f33a2-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f33a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f33a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f33a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f33a2-114">Not supported.</span></span>    |
|<span data-ttu-id="f33a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f33a2-115">Application</span></span> | <span data-ttu-id="f33a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f33a2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f33a2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f33a2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f33a2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f33a2-118">Optional query parameters</span></span>
<span data-ttu-id="f33a2-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f33a2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f33a2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f33a2-120">Request headers</span></span>
| <span data-ttu-id="f33a2-121">名称</span><span class="sxs-lookup"><span data-stu-id="f33a2-121">Name</span></span>      |<span data-ttu-id="f33a2-122">说明</span><span class="sxs-lookup"><span data-stu-id="f33a2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f33a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f33a2-123">Authorization</span></span>  | <span data-ttu-id="f33a2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f33a2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f33a2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f33a2-126">Request body</span></span>
<span data-ttu-id="f33a2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f33a2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f33a2-128">响应</span><span class="sxs-lookup"><span data-stu-id="f33a2-128">Response</span></span>

<span data-ttu-id="f33a2-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f33a2-129">If successful, this method returns a `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="f33a2-130">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="f33a2-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f33a2-131">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="f33a2-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="f33a2-132">示例</span><span class="sxs-lookup"><span data-stu-id="f33a2-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f33a2-133">请求</span><span class="sxs-lookup"><span data-stu-id="f33a2-133">Request</span></span>
<span data-ttu-id="f33a2-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f33a2-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="f33a2-135">响应</span><span class="sxs-lookup"><span data-stu-id="f33a2-135">Response</span></span>
<span data-ttu-id="f33a2-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f33a2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f33a2-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f33a2-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f33a2-140">语言</span><span class="sxs-lookup"><span data-stu-id="f33a2-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f33a2-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="f33a2-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_privilegedroleassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
