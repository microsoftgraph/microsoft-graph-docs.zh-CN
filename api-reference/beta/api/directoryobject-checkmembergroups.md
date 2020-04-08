---
title: 检查成员组
description: 检查指定组列表中的成员身份，并从该列表返回这些组
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0e5a86cca24b5c804a5a1ba61d7d6bc514f4a6ea
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43180970"
---
# <a name="check-member-groups"></a><span data-ttu-id="21775-103">检查成员组</span><span class="sxs-lookup"><span data-stu-id="21775-103">Check member groups</span></span>

<span data-ttu-id="21775-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21775-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21775-105">检查指定组列表中的成员身份，并从该列表返回指定用户、组、服务主体或目录对象所属的组。</span><span class="sxs-lookup"><span data-stu-id="21775-105">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, service principal or directory object is a member.</span></span> <span data-ttu-id="21775-106">此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="21775-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="21775-107">权限</span><span class="sxs-lookup"><span data-stu-id="21775-107">Permissions</span></span>
<span data-ttu-id="21775-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21775-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="21775-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="21775-110">Permission type</span></span>      | <span data-ttu-id="21775-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21775-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21775-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21775-112">Delegated (work or school account)</span></span> | <span data-ttu-id="21775-113">User.readbasic.all、GroupMember、GroupMember、和 Group。 read. all、user. all 和 Group。 read. all、Directory 中的所有读取。全部，全部读取。全部，Read. All</span><span class="sxs-lookup"><span data-stu-id="21775-113">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="21775-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21775-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21775-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="21775-115">Not supported.</span></span>    |
|<span data-ttu-id="21775-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="21775-116">Application</span></span> | <span data-ttu-id="21775-117">User. all 和 GroupMember、User. all 和 Group. all、Read. All： All</span><span class="sxs-lookup"><span data-stu-id="21775-117">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="21775-118">使用下面的方案指南可帮助确定要使用的权限类型：</span><span class="sxs-lookup"><span data-stu-id="21775-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="21775-119">使用 User. read 和 GroupMember 或 User. read 和 Group。 Read。获取登录用户的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="21775-119">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="21775-120">使用 User.readbasic.all 和 GroupMember、GroupMember、、all 和、all 和 group。 read. all 和 Group。 Read。获取任何用户的组成员身份的所有权限的权限的详细权限的概述。</span><span class="sxs-lookup"><span data-stu-id="21775-120">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="21775-121">使用 GroupMember 或 Group。读取。获取组的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="21775-121">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="21775-122">使用 GroupMember 和 Group. all 和 Group。 Read。获取服务主体的组成员身份的所有权限的权限。</span><span class="sxs-lookup"><span data-stu-id="21775-122">Use Application.ReadWrite.All and GroupMember.Read.All or Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="21775-123">使用目录读取。获取目录对象的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="21775-123">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="21775-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21775-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /servicePrincipals/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="21775-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="21775-125">Request headers</span></span>
| <span data-ttu-id="21775-126">名称</span><span class="sxs-lookup"><span data-stu-id="21775-126">Name</span></span>       | <span data-ttu-id="21775-127">类型</span><span class="sxs-lookup"><span data-stu-id="21775-127">Type</span></span> | <span data-ttu-id="21775-128">说明</span><span class="sxs-lookup"><span data-stu-id="21775-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="21775-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="21775-129">Authorization</span></span>  | <span data-ttu-id="21775-130">string</span><span class="sxs-lookup"><span data-stu-id="21775-130">string</span></span>  | <span data-ttu-id="21775-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="21775-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="21775-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21775-133">Content-Type</span></span>  | <span data-ttu-id="21775-134">application/json</span><span class="sxs-lookup"><span data-stu-id="21775-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21775-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="21775-135">Request body</span></span>
<span data-ttu-id="21775-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="21775-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="21775-137">参数</span><span class="sxs-lookup"><span data-stu-id="21775-137">Parameter</span></span>    | <span data-ttu-id="21775-138">类型</span><span class="sxs-lookup"><span data-stu-id="21775-138">Type</span></span>   |<span data-ttu-id="21775-139">说明</span><span class="sxs-lookup"><span data-stu-id="21775-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21775-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="21775-140">groupIds</span></span>|<span data-ttu-id="21775-141">String collection</span><span class="sxs-lookup"><span data-stu-id="21775-141">String collection</span></span> |<span data-ttu-id="21775-p104">包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。</span><span class="sxs-lookup"><span data-stu-id="21775-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="21775-144">响应</span><span class="sxs-lookup"><span data-stu-id="21775-144">Response</span></span>

<span data-ttu-id="21775-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="21775-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21775-146">示例</span><span class="sxs-lookup"><span data-stu-id="21775-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="21775-147">请求</span><span class="sxs-lookup"><span data-stu-id="21775-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="21775-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="21775-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="21775-149">C#</span><span class="sxs-lookup"><span data-stu-id="21775-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21775-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21775-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21775-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21775-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="21775-152">响应</span><span class="sxs-lookup"><span data-stu-id="21775-152">Response</span></span>
<span data-ttu-id="21775-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21775-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
