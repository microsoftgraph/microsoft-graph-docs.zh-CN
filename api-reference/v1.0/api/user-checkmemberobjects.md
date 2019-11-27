---
title: 用户： checkMemberObjects
description: 检查指定用户对象的组或目录角色列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da8993fb65fcc9a0a7bb0f887c3e743b196c686a
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621631"
---
# <a name="user-checkmemberobjects"></a><span data-ttu-id="bbca1-103">用户： checkMemberObjects</span><span class="sxs-lookup"><span data-stu-id="bbca1-103">user: checkMemberObjects</span></span>

<span data-ttu-id="bbca1-104">检查指定用户对象的组或目录角色列表中的成员资格。</span><span class="sxs-lookup"><span data-stu-id="bbca1-104">Check for membership in a list of group or directory roles for the specified user object.</span></span> <span data-ttu-id="bbca1-105">此方法是可传递的。</span><span class="sxs-lookup"><span data-stu-id="bbca1-105">This method is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbca1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="bbca1-106">Permissions</span></span>

<span data-ttu-id="bbca1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbca1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bbca1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbca1-109">Permission type</span></span>                        | <span data-ttu-id="bbca1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbca1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bbca1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbca1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbca1-112">User.readbasic.all，user. all，All。</span><span class="sxs-lookup"><span data-stu-id="bbca1-112">User.ReadBasic, User.Read.All, User.ReadWrite.All</span></span><br><br><span data-ttu-id="bbca1-113">此外：</span><span class="sxs-lookup"><span data-stu-id="bbca1-113">In addition:</span></span><br><br><ul><li><span data-ttu-id="bbca1-114">如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="bbca1-114">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="bbca1-115">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="bbca1-115">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="bbca1-116">如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</span><span class="sxs-lookup"><span data-stu-id="bbca1-116">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="bbca1-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bbca1-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
| <span data-ttu-id="bbca1-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbca1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbca1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbca1-119">Not supported.</span></span> |
| <span data-ttu-id="bbca1-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbca1-120">Application</span></span>                            | <span data-ttu-id="bbca1-121">User.readbasic.all、所有用户读写全部。 All</span><span class="sxs-lookup"><span data-stu-id="bbca1-121">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span><br><span data-ttu-id="bbca1-122">并</span><span class="sxs-lookup"><span data-stu-id="bbca1-122">And:</span></span><ul><li><span data-ttu-id="bbca1-123">如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="bbca1-123">If checking for membership in groups: Group.Read.All, Group.ReadWrite.All</span></span></li><li><span data-ttu-id="bbca1-124">如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="bbca1-124">If checking for membership in administrative units: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</span></span></li><li><span data-ttu-id="bbca1-125">如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</span><span class="sxs-lookup"><span data-stu-id="bbca1-125">If checking for membership in directory roles: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span></li></ul><span data-ttu-id="bbca1-126">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbca1-126">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbca1-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbca1-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="bbca1-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbca1-128">Request headers</span></span>

| <span data-ttu-id="bbca1-129">名称</span><span class="sxs-lookup"><span data-stu-id="bbca1-129">Name</span></span>          | <span data-ttu-id="bbca1-130">说明</span><span class="sxs-lookup"><span data-stu-id="bbca1-130">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bbca1-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbca1-131">Authorization</span></span> | <span data-ttu-id="bbca1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbca1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbca1-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bbca1-134">Content-Type</span></span>  | <span data-ttu-id="bbca1-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bbca1-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbca1-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbca1-137">Request body</span></span>

<span data-ttu-id="bbca1-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="bbca1-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bbca1-139">参数</span><span class="sxs-lookup"><span data-stu-id="bbca1-139">Parameter</span></span>    | <span data-ttu-id="bbca1-140">类型</span><span class="sxs-lookup"><span data-stu-id="bbca1-140">Type</span></span>        | <span data-ttu-id="bbca1-141">说明</span><span class="sxs-lookup"><span data-stu-id="bbca1-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bbca1-142">ids</span><span class="sxs-lookup"><span data-stu-id="bbca1-142">ids</span></span>|<span data-ttu-id="bbca1-143">String collection</span><span class="sxs-lookup"><span data-stu-id="bbca1-143">String collection</span></span>|<span data-ttu-id="bbca1-144">一个集合，包含要检查其成员身份的目录角色的组、目录角色或 roleTemplate Id 的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="bbca1-144">A collection that contains the object IDs of the groups, directory roles, or roleTemplate IDs of directory roles, in which to check membership.</span></span> <span data-ttu-id="bbca1-145">最大可指定20个对象。</span><span class="sxs-lookup"><span data-stu-id="bbca1-145">You can specify up to 20 objects.</span></span>|

## <a name="response"></a><span data-ttu-id="bbca1-146">响应</span><span class="sxs-lookup"><span data-stu-id="bbca1-146">Response</span></span>

<span data-ttu-id="bbca1-147">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的 String collection 对象。</span><span class="sxs-lookup"><span data-stu-id="bbca1-147">If successful, this method returns a `200 OK` response code and a new String collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbca1-148">示例</span><span class="sxs-lookup"><span data-stu-id="bbca1-148">Examples</span></span>

<span data-ttu-id="bbca1-149">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="bbca1-149">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bbca1-150">请求</span><span class="sxs-lookup"><span data-stu-id="bbca1-150">Request</span></span>

<span data-ttu-id="bbca1-151">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bbca1-151">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bbca1-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbca1-152">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bbca1-153">C#</span><span class="sxs-lookup"><span data-stu-id="bbca1-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bbca1-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbca1-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bbca1-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbca1-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bbca1-156">Java</span><span class="sxs-lookup"><span data-stu-id="bbca1-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bbca1-157">响应</span><span class="sxs-lookup"><span data-stu-id="bbca1-157">Response</span></span>

<span data-ttu-id="bbca1-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bbca1-158">The following is an example of the response.</span></span> 

><span data-ttu-id="bbca1-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bbca1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
