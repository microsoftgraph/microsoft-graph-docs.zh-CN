---
title: 检查成员组
description: 检查指定组列表中的成员身份, 并从该列表返回这些组
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99bcebbb6f7c94e67fea8dfc3f88269c80e568ea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455930"
---
# <a name="check-member-groups"></a><span data-ttu-id="b84fb-103">检查成员组</span><span class="sxs-lookup"><span data-stu-id="b84fb-103">Check member groups</span></span>

<span data-ttu-id="b84fb-p101">检查特定组列表中的成员资格，并从该列表返回成员为指定的 user、group 或 directory 对象的组。此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="b84fb-p101">Check for membership in a specified list of groups, and returns from that list those groups of which the specified user, group, or directory object is a member. This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="b84fb-106">权限</span><span class="sxs-lookup"><span data-stu-id="b84fb-106">Permissions</span></span>
<span data-ttu-id="b84fb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b84fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b84fb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b84fb-109">Permission type</span></span>      | <span data-ttu-id="b84fb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b84fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b84fb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b84fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b84fb-112">User.readbasic.all 和 group. all、User. all 和 Group。 all, read. All, All</span><span class="sxs-lookup"><span data-stu-id="b84fb-112">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="b84fb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b84fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b84fb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b84fb-114">Not supported.</span></span>    |
|<span data-ttu-id="b84fb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b84fb-115">Application</span></span> | <span data-ttu-id="b84fb-116">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b84fb-116">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="b84fb-117">使用下面的方案指南可帮助确定要使用的权限类型:</span><span class="sxs-lookup"><span data-stu-id="b84fb-117">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="b84fb-118">使用 User. Read 和 Group。所有权限, 用于检查登录用户的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="b84fb-118">Use User.Read and Group.Read.All permissions to check group memberships for the signed-in user.</span></span>
- <span data-ttu-id="b84fb-119">使用 User.readbasic.all 和 Group。 read. all 和 Group。 Read。所有权限, 用于检查任何用户的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="b84fb-119">Use User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to check group memberships for any user.</span></span>
- <span data-ttu-id="b84fb-120">使用 Group. Read。检查组的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="b84fb-120">Use Group.Read.All permission to check group memberships for a group.</span></span>
- <span data-ttu-id="b84fb-121">使用目录。查看目录对象的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="b84fb-121">Use Directory.Read.All permission to check group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="b84fb-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b84fb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
POST /groups/{id}/checkMemberGroups
POST /directoryObjects/{id}/checkMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="b84fb-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b84fb-123">Request headers</span></span>
| <span data-ttu-id="b84fb-124">名称</span><span class="sxs-lookup"><span data-stu-id="b84fb-124">Name</span></span>       | <span data-ttu-id="b84fb-125">类型</span><span class="sxs-lookup"><span data-stu-id="b84fb-125">Type</span></span> | <span data-ttu-id="b84fb-126">说明</span><span class="sxs-lookup"><span data-stu-id="b84fb-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b84fb-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b84fb-127">Authorization</span></span>  | <span data-ttu-id="b84fb-128">string</span><span class="sxs-lookup"><span data-stu-id="b84fb-128">string</span></span>  | <span data-ttu-id="b84fb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b84fb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b84fb-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b84fb-131">Content-Type</span></span>  | <span data-ttu-id="b84fb-132">string</span><span class="sxs-lookup"><span data-stu-id="b84fb-132">string</span></span> | <span data-ttu-id="b84fb-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b84fb-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b84fb-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="b84fb-134">Request body</span></span>
<span data-ttu-id="b84fb-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b84fb-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b84fb-136">参数</span><span class="sxs-lookup"><span data-stu-id="b84fb-136">Parameter</span></span>    | <span data-ttu-id="b84fb-137">类型</span><span class="sxs-lookup"><span data-stu-id="b84fb-137">Type</span></span>   |<span data-ttu-id="b84fb-138">说明</span><span class="sxs-lookup"><span data-stu-id="b84fb-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b84fb-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="b84fb-139">groupIds</span></span>|<span data-ttu-id="b84fb-140">String collection</span><span class="sxs-lookup"><span data-stu-id="b84fb-140">String collection</span></span>|<span data-ttu-id="b84fb-p104">包含检查成员身份的组中的对象 ID 的集合。可以指定多达 20 个组。</span><span class="sxs-lookup"><span data-stu-id="b84fb-p104">A collection that contains the object IDs of the groups in which to check membership. Up to 20 groups may be specified.</span></span>|

## <a name="response"></a><span data-ttu-id="b84fb-143">响应</span><span class="sxs-lookup"><span data-stu-id="b84fb-143">Response</span></span>

<span data-ttu-id="b84fb-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="b84fb-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b84fb-145">示例</span><span class="sxs-lookup"><span data-stu-id="b84fb-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b84fb-146">请求</span><span class="sxs-lookup"><span data-stu-id="b84fb-146">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b84fb-147">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b84fb-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b84fb-148">C#</span><span class="sxs-lookup"><span data-stu-id="b84fb-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b84fb-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="b84fb-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b84fb-150">目标-C</span><span class="sxs-lookup"><span data-stu-id="b84fb-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b84fb-151">响应</span><span class="sxs-lookup"><span data-stu-id="b84fb-151">Response</span></span>
<span data-ttu-id="b84fb-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b84fb-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
