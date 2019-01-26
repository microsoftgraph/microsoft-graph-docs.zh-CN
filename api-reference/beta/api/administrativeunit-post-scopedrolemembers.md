---
title: 添加 scopedRoleMember
description: 添加新 scopedRoleMembership。 注意： 只有*用户帐户管理员*和*技术支持管理员*角色当前支持范围角色成员身份。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e93dc3bc245b323e3c40fdd5678f4bfba495eafd
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571826"
---
# <a name="add-a-scopedrolemember"></a><span data-ttu-id="71f02-104">添加 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="71f02-104">Add a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71f02-105">添加新[scopedRoleMembership](../resources/scopedrolemembership.md)。</span><span class="sxs-lookup"><span data-stu-id="71f02-105">Add a new [scopedRoleMembership](../resources/scopedrolemembership.md).</span></span> <span data-ttu-id="71f02-106">注意： 只有*用户帐户管理员*和*技术支持管理员*角色当前支持范围角色成员身份。</span><span class="sxs-lookup"><span data-stu-id="71f02-106">NOTE: Only the *User account administrator* and *Helpdesk administrator* roles are currently supported for scoped-role memberships.</span></span>

## <a name="permissions"></a><span data-ttu-id="71f02-107">权限</span><span class="sxs-lookup"><span data-stu-id="71f02-107">Permissions</span></span>
<span data-ttu-id="71f02-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71f02-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="71f02-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="71f02-110">Permission type</span></span>      | <span data-ttu-id="71f02-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71f02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71f02-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71f02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71f02-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71f02-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71f02-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71f02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71f02-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71f02-115">Not supported.</span></span>    |
|<span data-ttu-id="71f02-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="71f02-116">Application</span></span> | <span data-ttu-id="71f02-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="71f02-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="71f02-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71f02-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/scopedRoleMembers
```
## <a name="request-headers"></a><span data-ttu-id="71f02-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="71f02-119">Request headers</span></span>
| <span data-ttu-id="71f02-120">名称</span><span class="sxs-lookup"><span data-stu-id="71f02-120">Name</span></span>      |<span data-ttu-id="71f02-121">说明</span><span class="sxs-lookup"><span data-stu-id="71f02-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71f02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71f02-122">Authorization</span></span>  | <span data-ttu-id="71f02-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71f02-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71f02-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="71f02-125">Request body</span></span>
<span data-ttu-id="71f02-126">在请求正文中，提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71f02-126">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="71f02-127">响应</span><span class="sxs-lookup"><span data-stu-id="71f02-127">Response</span></span>

<span data-ttu-id="71f02-128">如果成功，此方法返回`201 Created`响应正文中的响应代码和[scopedRoleMembership](../resources/scopedrolemembership.md)对象。</span><span class="sxs-lookup"><span data-stu-id="71f02-128">If successful, this method returns `201 Created` response code and [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71f02-129">示例</span><span class="sxs-lookup"><span data-stu-id="71f02-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71f02-130">请求</span><span class="sxs-lookup"><span data-stu-id="71f02-130">Request</span></span>
<span data-ttu-id="71f02-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71f02-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="71f02-132">在请求正文中，提供[scopedRoleMembership](../resources/scopedrolemembership.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71f02-132">In the request body, supply a JSON representation of [scopedRoleMembership](../resources/scopedrolemembership.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="71f02-133">响应</span><span class="sxs-lookup"><span data-stu-id="71f02-133">Response</span></span>
<span data-ttu-id="71f02-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71f02-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/administrativeunit-post-scopedrolemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
