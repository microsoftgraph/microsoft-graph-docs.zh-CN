---
title: 用户： checkMemberObjects
description: 检查指定用户对象的组、目录角色或管理单元对象的列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 654208a1163e2d99c0685d72588d64d9b0bf228f
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853847"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="bd3e4-103">用户： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="bd3e4-103">user: checkMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd3e4-104">检查指定用户对象的组、目录角色或管理单元对象的列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-104">Check for membership in a list of group, directory role, or administrative unit objects for the specified user object.</span></span> <span data-ttu-id="bd3e4-105">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd3e4-106">权限</span><span class="sxs-lookup"><span data-stu-id="bd3e4-106">Permissions</span></span>

<span data-ttu-id="bd3e4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd3e4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd3e4-109">Permission type</span></span>                        | <span data-ttu-id="bd3e4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd3e4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd3e4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd3e4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd3e4-112">User.readbasic.all，user. all，All。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-112">User.ReadBasic, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="bd3e4-113">此外：</span><span class="sxs-lookup"><span data-stu-id="bd3e4-113">In addition:</span></span><br><br><ul><li><span data-ttu-id="bd3e4-114">如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="bd3e4-114">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="bd3e4-115">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="bd3e4-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="bd3e4-116">如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</span><span class="sxs-lookup"><span data-stu-id="bd3e4-116">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="bd3e4-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bd3e4-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="bd3e4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd3e4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd3e4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-119">Not supported.</span></span> |
| <span data-ttu-id="bd3e4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd3e4-120">Application</span></span>                            | <span data-ttu-id="bd3e4-121">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="bd3e4-121">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="bd3e4-122">并</span><span class="sxs-lookup"><span data-stu-id="bd3e4-122">And:</span></span><ul><li><span data-ttu-id="bd3e4-123">如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="bd3e4-123">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="bd3e4-124">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="bd3e4-124">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="bd3e4-125">如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</span><span class="sxs-lookup"><span data-stu-id="bd3e4-125">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="bd3e4-126">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd3e4-126">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd3e4-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd3e4-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="bd3e4-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd3e4-128">Request headers</span></span>

| <span data-ttu-id="bd3e4-129">名称</span><span class="sxs-lookup"><span data-stu-id="bd3e4-129">Name</span></span>          | <span data-ttu-id="bd3e4-130">说明</span><span class="sxs-lookup"><span data-stu-id="bd3e4-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bd3e4-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd3e4-131">Authorization</span></span> | <span data-ttu-id="bd3e4-132">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="bd3e4-132">Bearer {token}</span></span> |
| <span data-ttu-id="bd3e4-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd3e4-133">Content-Type</span></span>  | <span data-ttu-id="bd3e4-134">application/json</span><span class="sxs-lookup"><span data-stu-id="bd3e4-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd3e4-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd3e4-135">Request body</span></span>

<span data-ttu-id="bd3e4-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bd3e4-137">参数</span><span class="sxs-lookup"><span data-stu-id="bd3e4-137">Parameter</span></span>    | <span data-ttu-id="bd3e4-138">类型</span><span class="sxs-lookup"><span data-stu-id="bd3e4-138">Type</span></span>        | <span data-ttu-id="bd3e4-139">说明</span><span class="sxs-lookup"><span data-stu-id="bd3e4-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bd3e4-140">ids</span><span class="sxs-lookup"><span data-stu-id="bd3e4-140">ids</span></span>|<span data-ttu-id="bd3e4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="bd3e4-141">String collection</span></span>|<span data-ttu-id="bd3e4-142">包含目录角色的组、目录角色、管理单元或 roleTemplate Id 的对象 Id 的集合，用于检查成员身份。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-142">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="bd3e4-143">最高可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-143">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="bd3e4-144">响应</span><span class="sxs-lookup"><span data-stu-id="bd3e4-144">Response</span></span>

<span data-ttu-id="bd3e4-145">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的 String collection 对象。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-145">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd3e4-146">示例</span><span class="sxs-lookup"><span data-stu-id="bd3e4-146">Examples</span></span>

<span data-ttu-id="bd3e4-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-147">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bd3e4-148">请求</span><span class="sxs-lookup"><span data-stu-id="bd3e4-148">Request</span></span>

<span data-ttu-id="bd3e4-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberObjects
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

### <a name="response"></a><span data-ttu-id="bd3e4-150">响应</span><span class="sxs-lookup"><span data-stu-id="bd3e4-150">Response</span></span>

<span data-ttu-id="bd3e4-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-151">The following is an example of the response.</span></span> 

><span data-ttu-id="bd3e4-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bd3e4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
