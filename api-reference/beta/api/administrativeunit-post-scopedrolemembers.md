---
title: 添加 scopedRoleMember
description: 添加新的 scopedRoleMembership。 注意：对于作用域角色成员身份，目前仅支持*用户帐户管理员*和*支持人员管理员*角色。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6fe72ec5158eb055b6f4309089aa8dc0327571a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441702"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="e8e48-104">添加 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="e8e48-104">Add a scopedRoleMember</span></span>

<span data-ttu-id="e8e48-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e8e48-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8e48-106">添加新的[scopedRoleMembership](../resources/scopedrolemembership.md)。</span><span class="sxs-lookup"><span data-stu-id="e8e48-106">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="e8e48-107">注意：对于作用域角色成员身份，目前仅支持*用户帐户管理员*和*支持人员管理员*角色。</span><span class="sxs-lookup"><span data-stu-id="e8e48-107">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8e48-108">权限</span><span class="sxs-lookup"><span data-stu-id="e8e48-108">Permissions</span></span>
<span data-ttu-id="e8e48-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8e48-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e8e48-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8e48-111">Permission type</span></span>      | <span data-ttu-id="e8e48-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8e48-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8e48-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8e48-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e8e48-114">RoleManagement、Directory.accessasuser.all 和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="e8e48-114">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e8e48-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8e48-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8e48-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8e48-116">Not supported.</span></span>    |
|<span data-ttu-id="e8e48-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8e48-117">Application</span></span> | <span data-ttu-id="e8e48-118">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="e8e48-118">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8e48-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8e48-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="e8e48-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8e48-120">Request headers</span></span>
| <span data-ttu-id="e8e48-121">名称</span><span class="sxs-lookup"><span data-stu-id="e8e48-121">Name</span></span>      |<span data-ttu-id="e8e48-122">说明</span><span class="sxs-lookup"><span data-stu-id="e8e48-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8e48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8e48-123">Authorization</span></span>  | <span data-ttu-id="e8e48-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8e48-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8e48-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8e48-126">Request body</span></span>
<span data-ttu-id="e8e48-127">在请求正文中，提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8e48-127">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e8e48-128">响应</span><span class="sxs-lookup"><span data-stu-id="e8e48-128">Response</span></span>

<span data-ttu-id="e8e48-129">如果成功，此方法在`201 Created`响应正文中返回响应代码和[scopedRoleMembership](../resources/scopedrolemembership.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e8e48-129">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8e48-130">示例</span><span class="sxs-lookup"><span data-stu-id="e8e48-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8e48-131">请求</span><span class="sxs-lookup"><span data-stu-id="e8e48-131">Request</span></span>
<span data-ttu-id="e8e48-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8e48-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8e48-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8e48-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e8e48-134">C#</span><span class="sxs-lookup"><span data-stu-id="e8e48-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-scopedrolemembership-from-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8e48-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8e48-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-scopedrolemembership-from-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8e48-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8e48-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-scopedrolemembership-from-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e8e48-137">在请求正文中，提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8e48-137">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e8e48-138">响应</span><span class="sxs-lookup"><span data-stu-id="e8e48-138">Response</span></span>
<span data-ttu-id="e8e48-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8e48-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
