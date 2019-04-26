---
title: 添加 scopedRoleMember
description: '添加新的 scopedRoleMembership。 注意: 对于作用域角色成员身份, 目前仅支持*用户帐户管理员*和*支持人员管理员*角色。'
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d866c2d4b126a7c08ff1b471cc871ba47a823df
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322763"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="6a0f2-104">添加 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="6a0f2-104">Add a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a0f2-105">添加新的[scopedRoleMembership](../resources/scopedrolemembership.md)。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-105">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="6a0f2-106">注意: 对于作用域角色成员身份, 目前仅支持*用户帐户管理员*和*支持人员管理员*角色。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-106">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a0f2-107">权限</span><span class="sxs-lookup"><span data-stu-id="6a0f2-107">Permissions</span></span>
<span data-ttu-id="6a0f2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6a0f2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a0f2-110">Permission type</span></span>      | <span data-ttu-id="6a0f2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a0f2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a0f2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a0f2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6a0f2-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a0f2-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a0f2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a0f2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a0f2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-115">Not supported.</span></span>    |
|<span data-ttu-id="6a0f2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a0f2-116">Application</span></span> | <span data-ttu-id="6a0f2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a0f2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a0f2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="6a0f2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a0f2-119">Request headers</span></span>
| <span data-ttu-id="6a0f2-120">名称</span><span class="sxs-lookup"><span data-stu-id="6a0f2-120">Name</span></span>      |<span data-ttu-id="6a0f2-121">说明</span><span class="sxs-lookup"><span data-stu-id="6a0f2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a0f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a0f2-122">Authorization</span></span>  | <span data-ttu-id="6a0f2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a0f2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a0f2-125">Request body</span></span>
<span data-ttu-id="6a0f2-126">在请求正文中, 提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-126">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6a0f2-127">响应</span><span class="sxs-lookup"><span data-stu-id="6a0f2-127">Response</span></span>

<span data-ttu-id="6a0f2-128">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[scopedRoleMembership](../resources/scopedrolemembership.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-128">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a0f2-129">示例</span><span class="sxs-lookup"><span data-stu-id="6a0f2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a0f2-130">请求</span><span class="sxs-lookup"><span data-stu-id="6a0f2-130">Request</span></span>
<span data-ttu-id="6a0f2-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="6a0f2-132">在请求正文中, 提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-132">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6a0f2-133">响应</span><span class="sxs-lookup"><span data-stu-id="6a0f2-133">Response</span></span>
<span data-ttu-id="6a0f2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a0f2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
