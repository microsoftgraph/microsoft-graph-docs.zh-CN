---
title: user： checkMemberObjects
description: 检查指定用户对象的组、目录角色或管理单元对象列表中的成员身份。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1f23615fb3e62eb30f576e8015986541063d8dd2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720359"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="9d8bc-103">user： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="9d8bc-103">user: checkMemberObjects</span></span>

<span data-ttu-id="9d8bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d8bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d8bc-105">检查指定用户对象的组、目录角色或管理单元对象列表中的成员身份。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-105">Check for membership in a list of group, directory role, or administrative unit objects for the specified user object.</span></span> <span data-ttu-id="9d8bc-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d8bc-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="9d8bc-107">Permissions</span></span>

<span data-ttu-id="9d8bc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9d8bc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d8bc-110">Permission type</span></span>                        | <span data-ttu-id="9d8bc-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d8bc-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9d8bc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d8bc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9d8bc-113">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8bc-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="9d8bc-114">此外：</span><span class="sxs-lookup"><span data-stu-id="9d8bc-114">In addition:</span></span><br><br><ul><li><span data-ttu-id="9d8bc-115">如果检查组成员身份：Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8bc-115">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="9d8bc-116">如果检查管理单元中的成员身份：AdministrativeUnit.Read.All、AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8bc-116">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="9d8bc-117">如果检查目录角色中的成员身份：RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9d8bc-117">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="9d8bc-118">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d8bc-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="9d8bc-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d8bc-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d8bc-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-120">Not supported.</span></span> |
| <span data-ttu-id="9d8bc-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d8bc-121">Application</span></span>                            | <span data-ttu-id="9d8bc-122">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8bc-122">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="9d8bc-123">并且：</span><span class="sxs-lookup"><span data-stu-id="9d8bc-123">And:</span></span><ul><li><span data-ttu-id="9d8bc-124">如果检查组成员身份：Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8bc-124">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="9d8bc-125">如果检查管理单元中的成员身份：AdministrativeUnit.Read.All、AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8bc-125">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="9d8bc-126">如果检查目录角色中的成员身份：RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="9d8bc-126">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="9d8bc-127">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d8bc-127">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d8bc-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d8bc-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="9d8bc-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d8bc-129">Request headers</span></span>

| <span data-ttu-id="9d8bc-130">名称</span><span class="sxs-lookup"><span data-stu-id="9d8bc-130">Name</span></span>          | <span data-ttu-id="9d8bc-131">说明</span><span class="sxs-lookup"><span data-stu-id="9d8bc-131">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9d8bc-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d8bc-132">Authorization</span></span> | <span data-ttu-id="9d8bc-133">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9d8bc-133">Bearer {token}</span></span> |
| <span data-ttu-id="9d8bc-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d8bc-134">Content-Type</span></span>  | <span data-ttu-id="9d8bc-135">application/json</span><span class="sxs-lookup"><span data-stu-id="9d8bc-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d8bc-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d8bc-136">Request body</span></span>

<span data-ttu-id="9d8bc-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9d8bc-138">参数</span><span class="sxs-lookup"><span data-stu-id="9d8bc-138">Parameter</span></span>    | <span data-ttu-id="9d8bc-139">类型</span><span class="sxs-lookup"><span data-stu-id="9d8bc-139">Type</span></span>        | <span data-ttu-id="9d8bc-140">说明</span><span class="sxs-lookup"><span data-stu-id="9d8bc-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9d8bc-141">ids</span><span class="sxs-lookup"><span data-stu-id="9d8bc-141">ids</span></span>|<span data-ttu-id="9d8bc-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9d8bc-142">String collection</span></span>|<span data-ttu-id="9d8bc-143">包含要检查成员身份的目录角色的组、目录角色、管理单元或 roleTemplate ID 的对象 ID 的集合。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-143">A collection that contains the object IDs of the groups, directory roles, administrative units, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="9d8bc-144">最多可指定 20 个对象。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-144">Up to 20 objects may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="9d8bc-145">响应</span><span class="sxs-lookup"><span data-stu-id="9d8bc-145">Response</span></span>

<span data-ttu-id="9d8bc-146">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和新的 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-146">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d8bc-147">示例</span><span class="sxs-lookup"><span data-stu-id="9d8bc-147">Examples</span></span>

<span data-ttu-id="9d8bc-148">下面是如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-148">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9d8bc-149">请求</span><span class="sxs-lookup"><span data-stu-id="9d8bc-149">Request</span></span>

<span data-ttu-id="9d8bc-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9d8bc-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d8bc-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9d8bc-152">C#</span><span class="sxs-lookup"><span data-stu-id="9d8bc-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d8bc-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d8bc-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d8bc-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d8bc-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d8bc-155">Java</span><span class="sxs-lookup"><span data-stu-id="9d8bc-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9d8bc-156">响应</span><span class="sxs-lookup"><span data-stu-id="9d8bc-156">Response</span></span>

<span data-ttu-id="9d8bc-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-157">The following is an example of the response.</span></span> 

><span data-ttu-id="9d8bc-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9d8bc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


