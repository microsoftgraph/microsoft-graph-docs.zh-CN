---
title: 添加 scopedRoleMember
description: 添加新的 scopedRoleMembership。 注意：对于作用域角色成员身份，目前仅支持 *用户帐户管理员* 和 *支持人员管理员* 角色。
localization_priority: Normal
author: anandyadavMSFT
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56bd18794a6e138b537524f63f4f1fc5cac483bc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962520"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="ce7cc-104">添加 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="ce7cc-104">Add a scopedRoleMember</span></span>

<span data-ttu-id="ce7cc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce7cc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce7cc-106">添加新的 [scopedRoleMembership](../resources/scopedrolemembership.md)。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-106">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="ce7cc-107">注意：对于作用域角色成员身份，目前仅支持 *用户帐户管理员* 和 *支持人员管理员* 角色。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-107">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce7cc-108">权限</span><span class="sxs-lookup"><span data-stu-id="ce7cc-108">Permissions</span></span>
<span data-ttu-id="ce7cc-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ce7cc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce7cc-111">Permission type</span></span>      | <span data-ttu-id="ce7cc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce7cc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce7cc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce7cc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ce7cc-114">RoleManagement、Directory.accessasuser.all 和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ce7cc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce7cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce7cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-116">Not supported.</span></span>    |
|<span data-ttu-id="ce7cc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce7cc-117">Application</span></span> | <span data-ttu-id="ce7cc-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="ce7cc-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce7cc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce7cc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="ce7cc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce7cc-120">Request headers</span></span>
| <span data-ttu-id="ce7cc-121">名称</span><span class="sxs-lookup"><span data-stu-id="ce7cc-121">Name</span></span>      |<span data-ttu-id="ce7cc-122">说明</span><span class="sxs-lookup"><span data-stu-id="ce7cc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce7cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce7cc-123">Authorization</span></span>  | <span data-ttu-id="ce7cc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce7cc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce7cc-126">Request body</span></span>
<span data-ttu-id="ce7cc-127">在请求正文中，提供 [scopedRoleMembership](../resources/scopedrolemembership.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-127">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ce7cc-128">响应</span><span class="sxs-lookup"><span data-stu-id="ce7cc-128">Response</span></span>

<span data-ttu-id="ce7cc-129">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [scopedRoleMembership](../resources/scopedrolemembership.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-129">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce7cc-130">示例</span><span class="sxs-lookup"><span data-stu-id="ce7cc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce7cc-131">请求</span><span class="sxs-lookup"><span data-stu-id="ce7cc-131">Request</span></span>
<span data-ttu-id="ce7cc-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce7cc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce7cc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_scopedrolemembership_from_administrativeunit"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers
Content-type: application/json
Content-length: 272

{
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="ce7cc-134">C#</span><span class="sxs-lookup"><span data-stu-id="ce7cc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce7cc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce7cc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce7cc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce7cc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce7cc-137">Java</span><span class="sxs-lookup"><span data-stu-id="ce7cc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-scopedrolemembership-from-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ce7cc-138">在请求正文中，提供 [scopedRoleMembership](../resources/scopedrolemembership.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-138">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ce7cc-139">响应</span><span class="sxs-lookup"><span data-stu-id="ce7cc-139">Response</span></span>
<span data-ttu-id="ce7cc-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce7cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 294

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships/$entity",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleId": "roleId-value",
  "roleMemberInfo": {
    "id": "id-value",
    "displayName": "displayName-value",
    "userPrincipalName": "userPrincipalName-value"
  },
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


