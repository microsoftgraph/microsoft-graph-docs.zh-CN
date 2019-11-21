---
title: 用户： checkMemberObjects
description: 检查指定用户对象的组或目录角色列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8bec7df1327ef3d04ba0b3121e04d2e446fcf190
ms.sourcegitcommit: c25828c596b7e0939fa164a3d7754722943152c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2019
ms.locfileid: "38757305"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="d381c-103">用户： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="d381c-103">user: checkMemberObjects</span></span>

<span data-ttu-id="d381c-104">检查指定用户对象的组或目录角色列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="d381c-104">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="d381c-105">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="d381c-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="d381c-106">权限</span><span class="sxs-lookup"><span data-stu-id="d381c-106">Permissions</span></span>

<span data-ttu-id="d381c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d381c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d381c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d381c-109">Permission type</span></span>                        | <span data-ttu-id="d381c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d381c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d381c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d381c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d381c-112">User.readbasic.all，user. all，All。</span><span class="sxs-lookup"><span data-stu-id="d381c-112">User.ReadBasic, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="d381c-113">此外：</span><span class="sxs-lookup"><span data-stu-id="d381c-113">In addition:</span></span><br><br><ul><li><span data-ttu-id="d381c-114">如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="d381c-114">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="d381c-115">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="d381c-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="d381c-116">如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</span><span class="sxs-lookup"><span data-stu-id="d381c-116">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="d381c-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d381c-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="d381c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d381c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d381c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d381c-119">Not supported.</span></span> |
| <span data-ttu-id="d381c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d381c-120">Application</span></span>                            | <span data-ttu-id="d381c-121">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="d381c-121">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="d381c-122">并</span><span class="sxs-lookup"><span data-stu-id="d381c-122">And:</span></span><ul><li><span data-ttu-id="d381c-123">如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="d381c-123">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="d381c-124">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="d381c-124">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="d381c-125">如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</span><span class="sxs-lookup"><span data-stu-id="d381c-125">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="d381c-126">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d381c-126">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d381c-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d381c-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="d381c-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="d381c-128">Request headers</span></span>

| <span data-ttu-id="d381c-129">名称</span><span class="sxs-lookup"><span data-stu-id="d381c-129">Name</span></span>          | <span data-ttu-id="d381c-130">说明</span><span class="sxs-lookup"><span data-stu-id="d381c-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d381c-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d381c-131">Authorization</span></span> | <span data-ttu-id="d381c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d381c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d381c-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d381c-134">Content-Type</span></span>  | <span data-ttu-id="d381c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d381c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d381c-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="d381c-137">Request body</span></span>

<span data-ttu-id="d381c-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d381c-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d381c-139">参数</span><span class="sxs-lookup"><span data-stu-id="d381c-139">Parameter</span></span>    | <span data-ttu-id="d381c-140">类型</span><span class="sxs-lookup"><span data-stu-id="d381c-140">Type</span></span>        | <span data-ttu-id="d381c-141">说明</span><span class="sxs-lookup"><span data-stu-id="d381c-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d381c-142">ids</span><span class="sxs-lookup"><span data-stu-id="d381c-142">ids</span></span>|<span data-ttu-id="d381c-143">String collection</span><span class="sxs-lookup"><span data-stu-id="d381c-143">String collection</span></span>|<span data-ttu-id="d381c-144">一个集合，包含要检查其成员身份的目录角色的组、目录角色或 roleTemplate Id 的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="d381c-144">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="d381c-145">最大可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="d381c-145">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="d381c-146">响应</span><span class="sxs-lookup"><span data-stu-id="d381c-146">Response</span></span>

<span data-ttu-id="d381c-147">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的 String collection 对象。</span><span class="sxs-lookup"><span data-stu-id="d381c-147">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d381c-148">示例</span><span class="sxs-lookup"><span data-stu-id="d381c-148">Examples</span></span>

<span data-ttu-id="d381c-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d381c-149">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d381c-150">请求</span><span class="sxs-lookup"><span data-stu-id="d381c-150">Request</span></span>

<span data-ttu-id="d381c-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d381c-151">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d381c-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="d381c-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d381c-153">响应</span><span class="sxs-lookup"><span data-stu-id="d381c-153">Response</span></span>

<span data-ttu-id="d381c-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d381c-154">The following is an example of the response.</span></span> 

><span data-ttu-id="d381c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d381c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
