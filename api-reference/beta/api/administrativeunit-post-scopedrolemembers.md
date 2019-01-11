---
title: 添加 scopedRoleMember
description: 添加新 scopedRoleMembership。 注意： 只有*用户帐户管理员*和*技术支持管理员*角色当前支持范围角色成员身份。
localization_priority: Normal
ms.openlocfilehash: e2ff1803ac0357fa8fef9e1cf68b2ff78f877895
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860016"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="0bb9d-104">添加 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="0bb9d-104">Add a scopedRoleMember</span></span>

> <span data-ttu-id="0bb9d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bb9d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0bb9d-107">添加新[scopedRoleMembership](../resources/scopedrolemembership.md)。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-107">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="0bb9d-108">注意： 只有*用户帐户管理员*和*技术支持管理员*角色当前支持范围角色成员身份。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-108">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bb9d-109">权限</span><span class="sxs-lookup"><span data-stu-id="0bb9d-109">Permissions</span></span>
<span data-ttu-id="0bb9d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0bb9d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0bb9d-112">Permission type</span></span>      | <span data-ttu-id="0bb9d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0bb9d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bb9d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0bb9d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0bb9d-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0bb9d-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0bb9d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0bb9d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bb9d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-117">Not supported.</span></span>    |
|<span data-ttu-id="0bb9d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0bb9d-118">Application</span></span> | <span data-ttu-id="0bb9d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bb9d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0bb9d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="0bb9d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0bb9d-121">Request headers</span></span>
| <span data-ttu-id="0bb9d-122">名称</span><span class="sxs-lookup"><span data-stu-id="0bb9d-122">Name</span></span>      |<span data-ttu-id="0bb9d-123">说明</span><span class="sxs-lookup"><span data-stu-id="0bb9d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0bb9d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bb9d-124">Authorization</span></span>  | <span data-ttu-id="0bb9d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bb9d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0bb9d-127">Request body</span></span>
<span data-ttu-id="0bb9d-128">在请求正文中，提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-128">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0bb9d-129">响应</span><span class="sxs-lookup"><span data-stu-id="0bb9d-129">Response</span></span>

<span data-ttu-id="0bb9d-130">如果成功，此方法返回`201 Created`响应正文中的响应代码和[scopedRoleMembership](../resources/scopedrolemembership.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-130">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bb9d-131">示例</span><span class="sxs-lookup"><span data-stu-id="0bb9d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0bb9d-132">请求</span><span class="sxs-lookup"><span data-stu-id="0bb9d-132">Request</span></span>
<span data-ttu-id="0bb9d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="0bb9d-134">在请求正文中，提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-134">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0bb9d-135">响应</span><span class="sxs-lookup"><span data-stu-id="0bb9d-135">Response</span></span>
<span data-ttu-id="0bb9d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0bb9d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedrolemembership"
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
<!-- {
  "type": "#page.annotation",
  "description": "Create scopedRoleMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
