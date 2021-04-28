---
title: 检查成员组
description: 检查指定组列表中的成员身份，然后从该列表返回这些组
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fe90927b01fd7ded6ecbe27c77f24c8dc9a4f822
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053165"
---
# <a name="check-member-groups"></a><span data-ttu-id="6015c-103">检查成员组</span><span class="sxs-lookup"><span data-stu-id="6015c-103">Check member groups</span></span>

<span data-ttu-id="6015c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6015c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6015c-p101">检查特定组列表中的成员资格，并从该列表返回成员为指定的 user、group 或 directory 对象的组。此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="6015c-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="6015c-107">权限</span><span class="sxs-lookup"><span data-stu-id="6015c-107">Permissions</span></span>
<span data-ttu-id="6015c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6015c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6015c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6015c-110">Permission type</span></span>      | <span data-ttu-id="6015c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6015c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6015c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6015c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6015c-113">User.ReadBasic.All、User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6015c-113">User.ReadBasic.All, User.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="6015c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6015c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6015c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6015c-115">Not supported.</span></span>    |
|<span data-ttu-id="6015c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6015c-116">Application</span></span> | <span data-ttu-id="6015c-117">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6015c-117">User.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="6015c-118">使用以下方案指南帮助确定要使用哪些权限类型：</span><span class="sxs-lookup"><span data-stu-id="6015c-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="6015c-119">使用 User.Read 和 GroupMember.Read.All 或 User.Read 和 Group.Read.All 权限获取登录用户的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="6015c-119">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="6015c-120">使用 User.ReadBasic.All 和 GroupMember.Read.All、User.Read.All 和 GroupMember.Read.All、User.ReadBasic.All 和 Group.Read.All 或 User.Read.All 和 Group.Read.All 权限获取任何用户的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="6015c-120">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="6015c-121">使用 GroupMember.Read.All 或 Group.Read.All 权限获取组的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="6015c-121">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="6015c-122">使用 Directory.Read.All 权限检查目录对象的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="6015c-122">Use Directory.Read.All permission to check group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="6015c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6015c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="6015c-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6015c-124">Request headers</span></span>
| <span data-ttu-id="6015c-125">名称</span><span class="sxs-lookup"><span data-stu-id="6015c-125">Name</span></span>       | <span data-ttu-id="6015c-126">类型</span><span class="sxs-lookup"><span data-stu-id="6015c-126">Type</span></span> | <span data-ttu-id="6015c-127">说明</span><span class="sxs-lookup"><span data-stu-id="6015c-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6015c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="6015c-128">Authorization</span></span>  | <span data-ttu-id="6015c-129">string</span><span class="sxs-lookup"><span data-stu-id="6015c-129">string</span></span>  | <span data-ttu-id="6015c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6015c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6015c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6015c-132">Content-Type</span></span>  | <span data-ttu-id="6015c-133">string</span><span class="sxs-lookup"><span data-stu-id="6015c-133">string</span></span> | <span data-ttu-id="6015c-134">application/json</span><span class="sxs-lookup"><span data-stu-id="6015c-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6015c-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="6015c-135">Request body</span></span>
<span data-ttu-id="6015c-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6015c-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6015c-137">参数</span><span class="sxs-lookup"><span data-stu-id="6015c-137">Parameter</span></span>    | <span data-ttu-id="6015c-138">类型</span><span class="sxs-lookup"><span data-stu-id="6015c-138">Type</span></span>   |<span data-ttu-id="6015c-139">说明</span><span class="sxs-lookup"><span data-stu-id="6015c-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6015c-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="6015c-140">groupIds</span></span>|<span data-ttu-id="6015c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6015c-141">String collection</span></span>|<span data-ttu-id="6015c-p104">包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。</span><span class="sxs-lookup"><span data-stu-id="6015c-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="6015c-144">响应</span><span class="sxs-lookup"><span data-stu-id="6015c-144">Response</span></span>

<span data-ttu-id="6015c-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="6015c-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6015c-146">示例</span><span class="sxs-lookup"><span data-stu-id="6015c-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6015c-147">请求</span><span class="sxs-lookup"><span data-stu-id="6015c-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6015c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6015c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{id}/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="6015c-149">C#</span><span class="sxs-lookup"><span data-stu-id="6015c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6015c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6015c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6015c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6015c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6015c-152">Java</span><span class="sxs-lookup"><span data-stu-id="6015c-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6015c-153">响应</span><span class="sxs-lookup"><span data-stu-id="6015c-153">Response</span></span>
<span data-ttu-id="6015c-154">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6015c-154">Note: The response object shown here might be shortened for readability.</span></span>
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
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

