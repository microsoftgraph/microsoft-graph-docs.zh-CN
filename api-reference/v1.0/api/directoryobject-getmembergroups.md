---
title: 获取成员组
description: 返回指定的 user、group 或 directory 对象所属的所有组。此函数是可传递的。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 399868d281b5e4a6eac7ead0ed31209236a26f7f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051485"
---
# <a name="get-member-groups"></a><span data-ttu-id="b3ffa-104">获取成员组</span><span class="sxs-lookup"><span data-stu-id="b3ffa-104">Get member groups</span></span>

<span data-ttu-id="b3ffa-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3ffa-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3ffa-p102">返回指定的 user、group 或 directory 对象所属的所有组。此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-p102">Return all the groups that the specified user, group, or directory object is a member of. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3ffa-108">权限</span><span class="sxs-lookup"><span data-stu-id="b3ffa-108">Permissions</span></span>
<span data-ttu-id="b3ffa-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3ffa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3ffa-111">Permission type</span></span>      | <span data-ttu-id="b3ffa-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3ffa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3ffa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3ffa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b3ffa-114">User.ReadBasic.All 和 GroupMember.Read.All、User.Read.All 和 GroupMember.Read.All、User.ReadBasic.All 和 Group.Read.All、User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3ffa-114">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="b3ffa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3ffa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3ffa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-116">Not supported.</span></span>    |
|<span data-ttu-id="b3ffa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3ffa-117">Application</span></span> | <span data-ttu-id="b3ffa-118">User.Read.All 和 GroupMember.Read.All、User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b3ffa-118">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="b3ffa-119">使用以下方案指南帮助确定要使用哪些权限类型：</span><span class="sxs-lookup"><span data-stu-id="b3ffa-119">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="b3ffa-120">使用 User.Read 和 GroupMember.Read.All 或 User.Read 和 Group.Read.All 权限获取登录用户的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-120">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="b3ffa-121">使用 User.ReadBasic.All 和 GroupMember.Read.All、User.Read.All 和 GroupMember.Read.All、User.ReadBasic.All 和 Group.Read.All 或 User.Read.All 和 Group.Read.All 权限获取任何用户的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-121">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="b3ffa-122">使用 GroupMember.Read.All 或 Group.Read.All 权限获取组的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-122">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="b3ffa-123">使用 Directory.Read.All 权限获取目录对象的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-123">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>


## <a name="http-request"></a><span data-ttu-id="b3ffa-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3ffa-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="b3ffa-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3ffa-125">Request headers</span></span>
| <span data-ttu-id="b3ffa-126">名称</span><span class="sxs-lookup"><span data-stu-id="b3ffa-126">Name</span></span>       | <span data-ttu-id="b3ffa-127">类型</span><span class="sxs-lookup"><span data-stu-id="b3ffa-127">Type</span></span> | <span data-ttu-id="b3ffa-128">说明</span><span class="sxs-lookup"><span data-stu-id="b3ffa-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b3ffa-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3ffa-129">Authorization</span></span>  | <span data-ttu-id="b3ffa-130">string</span><span class="sxs-lookup"><span data-stu-id="b3ffa-130">string</span></span>  | <span data-ttu-id="b3ffa-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3ffa-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3ffa-133">Content-Type</span></span>   | <span data-ttu-id="b3ffa-134">string</span><span class="sxs-lookup"><span data-stu-id="b3ffa-134">string</span></span>  | <span data-ttu-id="b3ffa-135">application/json</span><span class="sxs-lookup"><span data-stu-id="b3ffa-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3ffa-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3ffa-136">Request body</span></span>
<span data-ttu-id="b3ffa-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b3ffa-138">参数</span><span class="sxs-lookup"><span data-stu-id="b3ffa-138">Parameter</span></span>    | <span data-ttu-id="b3ffa-139">类型</span><span class="sxs-lookup"><span data-stu-id="b3ffa-139">Type</span></span>   |<span data-ttu-id="b3ffa-140">说明</span><span class="sxs-lookup"><span data-stu-id="b3ffa-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3ffa-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b3ffa-141">securityEnabledOnly</span></span>|<span data-ttu-id="b3ffa-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3ffa-142">Boolean</span></span>| <span data-ttu-id="b3ffa-p105">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="b3ffa-145">响应</span><span class="sxs-lookup"><span data-stu-id="b3ffa-145">Response</span></span>

<span data-ttu-id="b3ffa-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-146">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3ffa-147">示例</span><span class="sxs-lookup"><span data-stu-id="b3ffa-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b3ffa-148">请求</span><span class="sxs-lookup"><span data-stu-id="b3ffa-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b3ffa-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3ffa-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="b3ffa-150">C#</span><span class="sxs-lookup"><span data-stu-id="b3ffa-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3ffa-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3ffa-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3ffa-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3ffa-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3ffa-153">Java</span><span class="sxs-lookup"><span data-stu-id="b3ffa-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b3ffa-154">响应</span><span class="sxs-lookup"><span data-stu-id="b3ffa-154">Response</span></span>
<span data-ttu-id="b3ffa-155">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b3ffa-155">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

