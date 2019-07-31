---
title: 获取成员组
description: 返回指定的用户、组、服务主体或目录对象所属的所有组。 此函数是可传递的。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 847d3978aa346752d949cc5e82f390827d7639b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957785"
---
# <a name="get-member-groups"></a><span data-ttu-id="daacb-104">获取成员组</span><span class="sxs-lookup"><span data-stu-id="daacb-104">Get member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daacb-105">返回指定的用户、组、服务主体或目录对象所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="daacb-105">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="daacb-106">此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="daacb-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="daacb-107">权限</span><span class="sxs-lookup"><span data-stu-id="daacb-107">Permissions</span></span>
<span data-ttu-id="daacb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="daacb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="daacb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="daacb-110">Permission type</span></span>      | <span data-ttu-id="daacb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="daacb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="daacb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="daacb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="daacb-113">User.readbasic.all 和 group. all、User. all 和 Group。 all, read. All, All</span><span class="sxs-lookup"><span data-stu-id="daacb-113">User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="daacb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="daacb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daacb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="daacb-115">Not supported.</span></span>    |
|<span data-ttu-id="daacb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="daacb-116">Application</span></span> | <span data-ttu-id="daacb-117">User.Read.All 和 Group.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="daacb-117">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="daacb-118">使用下面的方案指南可帮助确定要使用的权限类型:</span><span class="sxs-lookup"><span data-stu-id="daacb-118">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="daacb-119">使用 User. Read 和 Group。读取。获取登录用户的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="daacb-119">Use User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="daacb-120">使用 User.readbasic.all 和 Group. all 或 User. read. all 和 Group。 Read。获取任何用户的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="daacb-120">Use User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="daacb-121">使用 Group. Read。获取组的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="daacb-121">Use Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="daacb-122">使用 Application. All 和 Group。读取。获取服务主体的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="daacb-122">Use Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="daacb-123">使用目录读取。获取目录对象的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="daacb-123">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="daacb-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="daacb-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="daacb-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="daacb-125">Request headers</span></span>
| <span data-ttu-id="daacb-126">名称</span><span class="sxs-lookup"><span data-stu-id="daacb-126">Name</span></span>       | <span data-ttu-id="daacb-127">类型</span><span class="sxs-lookup"><span data-stu-id="daacb-127">Type</span></span> | <span data-ttu-id="daacb-128">说明</span><span class="sxs-lookup"><span data-stu-id="daacb-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="daacb-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="daacb-129">Authorization</span></span>  | <span data-ttu-id="daacb-130">string</span><span class="sxs-lookup"><span data-stu-id="daacb-130">string</span></span>  | <span data-ttu-id="daacb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="daacb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="daacb-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="daacb-133">Content-Type</span></span>  | <span data-ttu-id="daacb-134">application/json</span><span class="sxs-lookup"><span data-stu-id="daacb-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="daacb-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="daacb-135">Request body</span></span>
<span data-ttu-id="daacb-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="daacb-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="daacb-137">参数</span><span class="sxs-lookup"><span data-stu-id="daacb-137">Parameter</span></span>    | <span data-ttu-id="daacb-138">类型</span><span class="sxs-lookup"><span data-stu-id="daacb-138">Type</span></span>   |<span data-ttu-id="daacb-139">说明</span><span class="sxs-lookup"><span data-stu-id="daacb-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daacb-140">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="daacb-140">securityEnabledOnly</span></span>|<span data-ttu-id="daacb-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="daacb-141">Boolean</span></span>| <span data-ttu-id="daacb-p105">**true** 指定仅应返回包含实体的安全组；**false** 指定应返回包含实体的所有组和目录角色。**注意**：如果参数为 **true**，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="daacb-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="daacb-144">响应</span><span class="sxs-lookup"><span data-stu-id="daacb-144">Response</span></span>

<span data-ttu-id="daacb-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="daacb-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daacb-146">示例</span><span class="sxs-lookup"><span data-stu-id="daacb-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="daacb-147">请求</span><span class="sxs-lookup"><span data-stu-id="daacb-147">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="daacb-148">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="daacb-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="daacb-149">C#</span><span class="sxs-lookup"><span data-stu-id="daacb-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="daacb-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="daacb-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="daacb-151">目标-C</span><span class="sxs-lookup"><span data-stu-id="daacb-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="daacb-152">Java</span><span class="sxs-lookup"><span data-stu-id="daacb-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="daacb-153">响应</span><span class="sxs-lookup"><span data-stu-id="daacb-153">Response</span></span>
<span data-ttu-id="daacb-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="daacb-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
