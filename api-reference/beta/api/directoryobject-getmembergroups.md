---
title: 获取成员组
description: 返回指定的用户、组、服务主体或目录对象所属的所有组。 此函数是可传递的。
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 14b9c670c2a01a72ca27ab20c187f1efd7572b84
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963066"
---
# <a name="get-member-groups"></a><span data-ttu-id="fc133-104">获取成员组</span><span class="sxs-lookup"><span data-stu-id="fc133-104">Get member groups</span></span>

<span data-ttu-id="fc133-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc133-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc133-106">返回指定的用户、组、服务主体或目录对象所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="fc133-106">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="fc133-107">此函数是可传递的。</span><span class="sxs-lookup"><span data-stu-id="fc133-107">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc133-108">权限</span><span class="sxs-lookup"><span data-stu-id="fc133-108">Permissions</span></span>
<span data-ttu-id="fc133-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc133-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fc133-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc133-111">Permission type</span></span>      | <span data-ttu-id="fc133-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc133-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc133-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc133-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fc133-114">User.readbasic.all、GroupMember、GroupMember、和 Group。 read. all、user. all 和 Group。 read. all、Directory 中的所有读取。全部，全部读取。全部，Read. All</span><span class="sxs-lookup"><span data-stu-id="fc133-114">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="fc133-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc133-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc133-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc133-116">Not supported.</span></span>    |
|<span data-ttu-id="fc133-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc133-117">Application</span></span> | <span data-ttu-id="fc133-118">User. all 和 GroupMember、User. all 和 Group. all、Read. All： All</span><span class="sxs-lookup"><span data-stu-id="fc133-118">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

<span data-ttu-id="fc133-119">使用下面的方案指南可帮助确定要使用的权限类型：</span><span class="sxs-lookup"><span data-stu-id="fc133-119">Use the follow scenario guidance to help determine which permission types to use:</span></span>
- <span data-ttu-id="fc133-120">使用 User. read 和 GroupMember 或 User. read 和 Group。 Read。获取登录用户的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="fc133-120">Use User.Read and GroupMember.Read.All or User.Read and Group.Read.All permissions to get group memberships for the signed-in user.</span></span>
- <span data-ttu-id="fc133-121">使用 User.readbasic.all 和 GroupMember、GroupMember、、all 和、all 和 group。 read. all 和 Group。 Read。获取任何用户的组成员身份的所有权限的权限的详细权限的概述。</span><span class="sxs-lookup"><span data-stu-id="fc133-121">Use User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All or User.Read.All and Group.Read.All permissions to get group memberships for any user.</span></span>
- <span data-ttu-id="fc133-122">使用 GroupMember 或 Group。读取。获取组的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="fc133-122">Use GroupMember.Read.All or Group.Read.All permission to get group memberships for a group.</span></span>
- <span data-ttu-id="fc133-123">使用 GroupMember 和 Group. all 和 Group。 Read。获取服务主体的组成员身份的所有权限的权限。</span><span class="sxs-lookup"><span data-stu-id="fc133-123">Use Application.ReadWrite.All and GroupMember.Read.All or Application.ReadWrite.All and Group.Read.All permissions to get group memberships for a service principal.</span></span>
- <span data-ttu-id="fc133-124">使用目录读取。获取目录对象的组成员身份的所有权限。</span><span class="sxs-lookup"><span data-stu-id="fc133-124">Use Directory.Read.All permission to get group memberships for a directory object.</span></span>

## <a name="http-request"></a><span data-ttu-id="fc133-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc133-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="fc133-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc133-126">Request headers</span></span>
| <span data-ttu-id="fc133-127">名称</span><span class="sxs-lookup"><span data-stu-id="fc133-127">Name</span></span>       | <span data-ttu-id="fc133-128">类型</span><span class="sxs-lookup"><span data-stu-id="fc133-128">Type</span></span> | <span data-ttu-id="fc133-129">说明</span><span class="sxs-lookup"><span data-stu-id="fc133-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc133-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc133-130">Authorization</span></span>  | <span data-ttu-id="fc133-131">string</span><span class="sxs-lookup"><span data-stu-id="fc133-131">string</span></span>  | <span data-ttu-id="fc133-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc133-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc133-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc133-134">Content-Type</span></span>  | <span data-ttu-id="fc133-135">application/json</span><span class="sxs-lookup"><span data-stu-id="fc133-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc133-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc133-136">Request body</span></span>
<span data-ttu-id="fc133-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fc133-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc133-138">参数</span><span class="sxs-lookup"><span data-stu-id="fc133-138">Parameter</span></span>    | <span data-ttu-id="fc133-139">类型</span><span class="sxs-lookup"><span data-stu-id="fc133-139">Type</span></span>   |<span data-ttu-id="fc133-140">说明</span><span class="sxs-lookup"><span data-stu-id="fc133-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc133-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="fc133-141">securityEnabledOnly</span></span>|<span data-ttu-id="fc133-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc133-142">Boolean</span></span>| <span data-ttu-id="fc133-p105">**true** 指定仅应返回包含实体的安全组； **false** 指定应返回包含实体的所有组和目录角色。 **注意** ：如果参数为 **true** ，只能对一位用户调用此函数。</span><span class="sxs-lookup"><span data-stu-id="fc133-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note** : The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="fc133-145">响应</span><span class="sxs-lookup"><span data-stu-id="fc133-145">Response</span></span>

<span data-ttu-id="fc133-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="fc133-146">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc133-147">示例</span><span class="sxs-lookup"><span data-stu-id="fc133-147">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fc133-148">请求</span><span class="sxs-lookup"><span data-stu-id="fc133-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fc133-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc133-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fc133-150">C#</span><span class="sxs-lookup"><span data-stu-id="fc133-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc133-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc133-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc133-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc133-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc133-153">Java</span><span class="sxs-lookup"><span data-stu-id="fc133-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc133-154">响应</span><span class="sxs-lookup"><span data-stu-id="fc133-154">Response</span></span>
<span data-ttu-id="fc133-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc133-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


