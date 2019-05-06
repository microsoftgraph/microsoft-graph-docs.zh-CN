---
title: 创建 privilegedRoleAssignment
description: 使用此 API 创建新的 privilegedRoleAssignment。
localization_priority: Normal
ms.openlocfilehash: d6fb9462f429cfc19c5d4cf0e1829da6057674c4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593799"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="2729b-103">创建 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="2729b-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2729b-104">使用此 API 创建新的[privilegedRoleAssignment](../resources/privilegedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="2729b-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2729b-105">权限</span><span class="sxs-lookup"><span data-stu-id="2729b-105">Permissions</span></span>
<span data-ttu-id="2729b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2729b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2729b-108">请求者需要具有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="2729b-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="2729b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2729b-109">Permission type</span></span>      | <span data-ttu-id="2729b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2729b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2729b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2729b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2729b-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2729b-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2729b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2729b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2729b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2729b-114">Not supported.</span></span>    |
|<span data-ttu-id="2729b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2729b-115">Application</span></span> | <span data-ttu-id="2729b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2729b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2729b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2729b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="2729b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2729b-118">Request headers</span></span>
| <span data-ttu-id="2729b-119">名称</span><span class="sxs-lookup"><span data-stu-id="2729b-119">Name</span></span>       | <span data-ttu-id="2729b-120">说明</span><span class="sxs-lookup"><span data-stu-id="2729b-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2729b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2729b-121">Authorization</span></span>  | <span data-ttu-id="2729b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2729b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2729b-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2729b-124">Request body</span></span>
<span data-ttu-id="2729b-125">在请求正文中, 提供[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2729b-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2729b-126">响应</span><span class="sxs-lookup"><span data-stu-id="2729b-126">Response</span></span>

<span data-ttu-id="2729b-127">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2729b-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="2729b-128">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="2729b-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2729b-129">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="2729b-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="2729b-130">示例</span><span class="sxs-lookup"><span data-stu-id="2729b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2729b-131">请求</span><span class="sxs-lookup"><span data-stu-id="2729b-131">Request</span></span>
<span data-ttu-id="2729b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2729b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
<span data-ttu-id="2729b-133">在请求正文中, 提供[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2729b-133">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2729b-134">响应</span><span class="sxs-lookup"><span data-stu-id="2729b-134">Response</span></span>
<span data-ttu-id="2729b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2729b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2729b-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="2729b-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2729b-139">语言</span><span class="sxs-lookup"><span data-stu-id="2729b-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_privilegedroleassignment_from_privilegedroleassignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2729b-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="2729b-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_privilegedroleassignment_from_privilegedroleassignments-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
