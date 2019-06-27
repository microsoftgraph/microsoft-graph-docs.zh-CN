---
title: 添加 scopedRoleMember
description: '添加新的 scopedRoleMembership。 注意: 对于作用域角色成员身份, 目前仅支持*用户帐户管理员*和*支持人员管理员*角色。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e933158e2510f26048b7f770aa43dfcd67b6cae9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258679"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="62837-104">添加 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="62837-104">Add a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62837-105">添加新的[scopedRoleMembership](../resources/scopedrolemembership.md)。</span><span class="sxs-lookup"><span data-stu-id="62837-105">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="62837-106">注意: 对于作用域角色成员身份, 目前仅支持*用户帐户管理员*和*支持人员管理员*角色。</span><span class="sxs-lookup"><span data-stu-id="62837-106">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="62837-107">权限</span><span class="sxs-lookup"><span data-stu-id="62837-107">Permissions</span></span>
<span data-ttu-id="62837-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62837-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="62837-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="62837-110">Permission type</span></span>      | <span data-ttu-id="62837-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62837-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="62837-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62837-112">Delegated (work or school account)</span></span> | <span data-ttu-id="62837-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="62837-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="62837-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62837-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62837-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="62837-115">Not supported.</span></span>    |
|<span data-ttu-id="62837-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="62837-116">Application</span></span> | <span data-ttu-id="62837-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="62837-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="62837-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62837-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="62837-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="62837-119">Request headers</span></span>
| <span data-ttu-id="62837-120">名称</span><span class="sxs-lookup"><span data-stu-id="62837-120">Name</span></span>      |<span data-ttu-id="62837-121">说明</span><span class="sxs-lookup"><span data-stu-id="62837-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="62837-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62837-122">Authorization</span></span>  | <span data-ttu-id="62837-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="62837-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="62837-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="62837-125">Request body</span></span>
<span data-ttu-id="62837-126">在请求正文中, 提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62837-126">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="62837-127">响应</span><span class="sxs-lookup"><span data-stu-id="62837-127">Response</span></span>

<span data-ttu-id="62837-128">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[scopedRoleMembership](../resources/scopedrolemembership.md)对象。</span><span class="sxs-lookup"><span data-stu-id="62837-128">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62837-129">示例</span><span class="sxs-lookup"><span data-stu-id="62837-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="62837-130">请求</span><span class="sxs-lookup"><span data-stu-id="62837-130">Request</span></span>
<span data-ttu-id="62837-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62837-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="62837-132">在请求正文中, 提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62837-132">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="62837-133">响应</span><span class="sxs-lookup"><span data-stu-id="62837-133">Response</span></span>
<span data-ttu-id="62837-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="62837-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="62837-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="62837-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="62837-138">C#</span><span class="sxs-lookup"><span data-stu-id="62837-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_scopedrolemembership_from_administrativeunit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="62837-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="62837-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_scopedrolemembership_from_administrativeunit-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="62837-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="62837-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_scopedrolemembership_from_administrativeunit-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
