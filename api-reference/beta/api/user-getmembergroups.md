---
title: 'user: getMemberGroups'
description: 返回用户是其成员的所有组。 检查是可传递的，这不同于读取
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c2ab1bcd9dce8e933ed65d51dd9b0ce010bc1b90
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896467"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="1c690-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="1c690-104">user: getMemberGroups</span></span>

<span data-ttu-id="1c690-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c690-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c690-106">Return all the groups that the user is a member of.</span><span class="sxs-lookup"><span data-stu-id="1c690-106">Return all the groups that the user is a member of.</span></span> <span data-ttu-id="1c690-107">The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span><span class="sxs-lookup"><span data-stu-id="1c690-107">The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="1c690-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1c690-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span></span> <span data-ttu-id="1c690-109">The maximum number of groups each request can return is 2046.</span><span class="sxs-lookup"><span data-stu-id="1c690-109">The maximum number of groups each request can return is 2046.</span></span> <span data-ttu-id="1c690-110">Note that Microsoft 365 groups cannot contain groups.</span><span class="sxs-lookup"><span data-stu-id="1c690-110">Note that Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="1c690-111">So membership in a Microsoft 365 group is always direct.</span><span class="sxs-lookup"><span data-stu-id="1c690-111">So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c690-112">权限</span><span class="sxs-lookup"><span data-stu-id="1c690-112">Permissions</span></span>

<span data-ttu-id="1c690-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="1c690-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1c690-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c690-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c690-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c690-115">Permission type</span></span>                        | <span data-ttu-id="1c690-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c690-116">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1c690-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c690-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c690-118">User.readbasic.all 和 GroupMember。 Read. All、GroupMember、User.readbasic.all 和 GroupMember，all，user. all 和 group。 read. all、user. all 和 group。 Read. all、、all 和 group. all、all、all、all 和 Group. all，all，</span><span class="sxs-lookup"><span data-stu-id="1c690-118">User.ReadBasic.All and GroupMember.Read.All, User.Read and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1c690-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c690-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c690-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c690-120">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="1c690-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c690-121">Application</span></span>                            | <span data-ttu-id="1c690-122">User.Read.All 和 GroupMember.Read.All、User.Read.All 和 Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c690-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>            |

## <a name="http-request"></a><span data-ttu-id="1c690-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c690-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="1c690-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c690-124">Request headers</span></span>

| <span data-ttu-id="1c690-125">标头</span><span class="sxs-lookup"><span data-stu-id="1c690-125">Header</span></span>        | <span data-ttu-id="1c690-126">值</span><span class="sxs-lookup"><span data-stu-id="1c690-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="1c690-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c690-127">Authorization</span></span> | <span data-ttu-id="1c690-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="1c690-128">Bearer {token}.</span></span> <span data-ttu-id="1c690-129">Required.</span><span class="sxs-lookup"><span data-stu-id="1c690-129">Required.</span></span> |
| <span data-ttu-id="1c690-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c690-130">Content-Type</span></span>  | <span data-ttu-id="1c690-131">application/json</span><span class="sxs-lookup"><span data-stu-id="1c690-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="1c690-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c690-132">Request body</span></span>

<span data-ttu-id="1c690-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1c690-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c690-134">参数</span><span class="sxs-lookup"><span data-stu-id="1c690-134">Parameter</span></span>           | <span data-ttu-id="1c690-135">类型</span><span class="sxs-lookup"><span data-stu-id="1c690-135">Type</span></span>    | <span data-ttu-id="1c690-136">说明</span><span class="sxs-lookup"><span data-stu-id="1c690-136">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1c690-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="1c690-137">securityEnabledOnly</span></span> | <span data-ttu-id="1c690-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c690-138">Boolean</span></span> | <span data-ttu-id="1c690-139">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned.</span><span class="sxs-lookup"><span data-stu-id="1c690-139">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned.</span></span> <span data-ttu-id="1c690-140">Note: Setting this parameter to **true** is only supported when calling this method on a user.</span><span class="sxs-lookup"><span data-stu-id="1c690-140">Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="1c690-141">响应</span><span class="sxs-lookup"><span data-stu-id="1c690-141">Response</span></span>

<span data-ttu-id="1c690-142">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和字符串集合，响应正文中包括用户是其成员的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="1c690-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="1c690-143">示例</span><span class="sxs-lookup"><span data-stu-id="1c690-143">Example</span></span>

<span data-ttu-id="1c690-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1c690-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1c690-145">请求</span><span class="sxs-lookup"><span data-stu-id="1c690-145">Request</span></span>

<span data-ttu-id="1c690-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c690-146">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1c690-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c690-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="1c690-148">C#</span><span class="sxs-lookup"><span data-stu-id="1c690-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c690-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c690-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c690-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c690-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1c690-151">响应</span><span class="sxs-lookup"><span data-stu-id="1c690-151">Response</span></span>

<span data-ttu-id="1c690-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="1c690-152">Here is an example of the response.</span></span> <span data-ttu-id="1c690-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="1c690-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1c690-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="1c690-154">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
