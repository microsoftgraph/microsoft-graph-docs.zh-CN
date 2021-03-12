---
title: user： checkMemberObjects
description: 检查指定用户对象的组或目录角色列表中的成员身份。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4f27a53030e1c01b3efb1967f9f0620033e36f28
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722389"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="386b6-103">user： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="386b6-103">user: checkMemberObjects</span></span>

<span data-ttu-id="386b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="386b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="386b6-105">检查指定用户对象的组或目录角色列表中的成员身份。</span><span class="sxs-lookup"><span data-stu-id="386b6-105">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="386b6-106">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="386b6-106">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="386b6-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="386b6-107">Permissions</span></span>

<span data-ttu-id="386b6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="386b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="386b6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="386b6-110">Permission type</span></span>                        | <span data-ttu-id="386b6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="386b6-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="386b6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="386b6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="386b6-113">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386b6-113">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="386b6-114">此外：</span><span class="sxs-lookup"><span data-stu-id="386b6-114">In addition:</span></span><br><br><ul><li><span data-ttu-id="386b6-115">如果检查组成员身份：Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386b6-115">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="386b6-116">如果检查管理单元中的成员身份：AdministrativeUnit.Read.All、AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386b6-116">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="386b6-117">如果检查目录角色中的成员身份：RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="386b6-117">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="386b6-118">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="386b6-118">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="386b6-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="386b6-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="386b6-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="386b6-120">Not supported.</span></span> |
| <span data-ttu-id="386b6-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="386b6-121">Application</span></span>                            | <span data-ttu-id="386b6-122">User.ReadBasic.All、User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386b6-122">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="386b6-123">而且：</span><span class="sxs-lookup"><span data-stu-id="386b6-123">And:</span></span><ul><li><span data-ttu-id="386b6-124">如果检查组成员身份：Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386b6-124">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="386b6-125">如果检查管理单元中的成员身份：AdministrativeUnit.Read.All、AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386b6-125">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="386b6-126">如果检查目录角色中的成员身份：RoleManagement.Read.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="386b6-126">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="386b6-127">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="386b6-127">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="386b6-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="386b6-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="386b6-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="386b6-129">Request headers</span></span>

| <span data-ttu-id="386b6-130">名称</span><span class="sxs-lookup"><span data-stu-id="386b6-130">Name</span></span>          | <span data-ttu-id="386b6-131">说明</span><span class="sxs-lookup"><span data-stu-id="386b6-131">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="386b6-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="386b6-132">Authorization</span></span> | <span data-ttu-id="386b6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="386b6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="386b6-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="386b6-135">Content-Type</span></span>  | <span data-ttu-id="386b6-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="386b6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="386b6-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="386b6-138">Request body</span></span>

<span data-ttu-id="386b6-139">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="386b6-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="386b6-140">参数</span><span class="sxs-lookup"><span data-stu-id="386b6-140">Parameter</span></span>    | <span data-ttu-id="386b6-141">类型</span><span class="sxs-lookup"><span data-stu-id="386b6-141">Type</span></span>        | <span data-ttu-id="386b6-142">说明</span><span class="sxs-lookup"><span data-stu-id="386b6-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="386b6-143">ids</span><span class="sxs-lookup"><span data-stu-id="386b6-143">ids</span></span>|<span data-ttu-id="386b6-144">String collection</span><span class="sxs-lookup"><span data-stu-id="386b6-144">String collection</span></span>|<span data-ttu-id="386b6-145">包含要检查成员身份的目录角色的组、目录角色或 roleTemplate ID 的对象 ID 的集合。</span><span class="sxs-lookup"><span data-stu-id="386b6-145">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="386b6-146">可以指定最多 20 个对象。</span><span class="sxs-lookup"><span data-stu-id="386b6-146">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="386b6-147">响应</span><span class="sxs-lookup"><span data-stu-id="386b6-147">Response</span></span>

<span data-ttu-id="386b6-148">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="386b6-148">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="386b6-149">示例</span><span class="sxs-lookup"><span data-stu-id="386b6-149">Examples</span></span>

<span data-ttu-id="386b6-150">下面是如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="386b6-150">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="386b6-151">请求</span><span class="sxs-lookup"><span data-stu-id="386b6-151">Request</span></span>

<span data-ttu-id="386b6-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="386b6-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="386b6-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="386b6-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="386b6-154">C#</span><span class="sxs-lookup"><span data-stu-id="386b6-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="386b6-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="386b6-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="386b6-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="386b6-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="386b6-157">Java</span><span class="sxs-lookup"><span data-stu-id="386b6-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="386b6-158">响应</span><span class="sxs-lookup"><span data-stu-id="386b6-158">Response</span></span>

<span data-ttu-id="386b6-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="386b6-159">The following is an example of the response.</span></span> 

><span data-ttu-id="386b6-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="386b6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

