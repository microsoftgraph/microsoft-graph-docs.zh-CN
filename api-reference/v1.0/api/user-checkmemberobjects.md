---
title: 用户： checkMemberObjects
description: 检查指定用户对象的组或目录角色列表中的成员资格。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a33da99187ba8d8bbc64ea119dd3c3a13491a92e
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108408"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="173da-103">用户： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="173da-103">user: checkMemberObjects</span></span>

<span data-ttu-id="173da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="173da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="173da-105">检查指定用户对象的组或目录角色列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="173da-105">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="173da-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="173da-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="173da-107">权限</span><span class="sxs-lookup"><span data-stu-id="173da-107">Permissions</span></span>

<span data-ttu-id="173da-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="173da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="173da-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="173da-110">Permission type</span></span>                        | <span data-ttu-id="173da-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="173da-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="173da-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="173da-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="173da-113">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="173da-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="173da-114">此外：</span><span class="sxs-lookup"><span data-stu-id="173da-114">In addition:</span></span><br><br><ul><li><span data-ttu-id="173da-115">如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="173da-115">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="173da-116">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="173da-116">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="173da-117">如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</span><span class="sxs-lookup"><span data-stu-id="173da-117">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="173da-118">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="173da-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="173da-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="173da-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="173da-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="173da-120">Not supported.</span></span> |
| <span data-ttu-id="173da-121">Application</span><span class="sxs-lookup"><span data-stu-id="173da-121">Application</span></span>                            | <span data-ttu-id="173da-122">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="173da-122">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="173da-123">并</span><span class="sxs-lookup"><span data-stu-id="173da-123">And:</span></span><ul><li><span data-ttu-id="173da-124">如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="173da-124">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="173da-125">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="173da-125">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="173da-126">如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</span><span class="sxs-lookup"><span data-stu-id="173da-126">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="173da-127">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="173da-127">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="173da-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="173da-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="173da-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="173da-129">Request headers</span></span>

| <span data-ttu-id="173da-130">名称</span><span class="sxs-lookup"><span data-stu-id="173da-130">Name</span></span>          | <span data-ttu-id="173da-131">说明</span><span class="sxs-lookup"><span data-stu-id="173da-131">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="173da-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="173da-132">Authorization</span></span> | <span data-ttu-id="173da-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="173da-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="173da-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="173da-135">Content-Type</span></span>  | <span data-ttu-id="173da-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="173da-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="173da-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="173da-138">Request body</span></span>

<span data-ttu-id="173da-139">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="173da-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="173da-140">参数</span><span class="sxs-lookup"><span data-stu-id="173da-140">Parameter</span></span>    | <span data-ttu-id="173da-141">类型</span><span class="sxs-lookup"><span data-stu-id="173da-141">Type</span></span>        | <span data-ttu-id="173da-142">说明</span><span class="sxs-lookup"><span data-stu-id="173da-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="173da-143">ids</span><span class="sxs-lookup"><span data-stu-id="173da-143">ids</span></span>|<span data-ttu-id="173da-144">String collection</span><span class="sxs-lookup"><span data-stu-id="173da-144">String collection</span></span>|<span data-ttu-id="173da-145">一个集合，包含要检查其成员身份的目录角色的组、目录角色或 roleTemplate Id 的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="173da-145">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="173da-146">最大可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="173da-146">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="173da-147">响应</span><span class="sxs-lookup"><span data-stu-id="173da-147">Response</span></span>

<span data-ttu-id="173da-148">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的 String collection 对象。</span><span class="sxs-lookup"><span data-stu-id="173da-148">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="173da-149">示例</span><span class="sxs-lookup"><span data-stu-id="173da-149">Examples</span></span>

<span data-ttu-id="173da-150">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="173da-150">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="173da-151">请求</span><span class="sxs-lookup"><span data-stu-id="173da-151">Request</span></span>

<span data-ttu-id="173da-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="173da-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="173da-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="173da-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="173da-154">C#</span><span class="sxs-lookup"><span data-stu-id="173da-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="173da-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="173da-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="173da-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="173da-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="173da-157">Java</span><span class="sxs-lookup"><span data-stu-id="173da-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="173da-158">响应</span><span class="sxs-lookup"><span data-stu-id="173da-158">Response</span></span>

<span data-ttu-id="173da-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="173da-159">The following is an example of the response.</span></span> 

><span data-ttu-id="173da-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="173da-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
