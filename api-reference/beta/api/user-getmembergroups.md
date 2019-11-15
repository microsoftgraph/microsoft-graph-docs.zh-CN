---
title: 'user: getMemberGroups'
description: 返回用户是其成员的所有组。 检查是可传递的，这不同于读取
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8d044c4e158986a8154c0c118973edcc6ee84a1b
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38657820"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="9cd8a-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="9cd8a-104">user: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cd8a-p102">返回用户是其成员的所有组。检查是可传递的，这和读取 [memberOf](../api/user-list-memberof.md) 导航属性不同，后者仅返回用户是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="9cd8a-p103">此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。每个请求可以返回的最大组数为 2046 组。注意：Office 365 组不能包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="9cd8a-111">权限</span><span class="sxs-lookup"><span data-stu-id="9cd8a-111">Permissions</span></span>

<span data-ttu-id="9cd8a-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9cd8a-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cd8a-114">Permission type</span></span>                        | <span data-ttu-id="9cd8a-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cd8a-115">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9cd8a-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cd8a-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="9cd8a-117">User.readbasic.all、GroupMember 和 GroupMember，all，user. all 和 group。 read. all、user. read 和 Group。 read. all、user. read. all 和 group。 Read. all、read. all 和 group。 Read. all、read. all 和 group。 Read. all，Directory. all，Directory.accessasuser.all 的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-117">User.ReadBasic.All and GroupMember.Read.All, User.Read and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="9cd8a-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cd8a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cd8a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-119">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="9cd8a-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cd8a-120">Application</span></span>                            | <span data-ttu-id="9cd8a-121">"GroupMember"、"all" 和 "Group"、"all" 和 "Group"、"全部"、"全部"、"全部"、"所有"</span><span class="sxs-lookup"><span data-stu-id="9cd8a-121">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>            |

## <a name="http-request"></a><span data-ttu-id="9cd8a-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cd8a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="9cd8a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cd8a-123">Request headers</span></span>

| <span data-ttu-id="9cd8a-124">标头</span><span class="sxs-lookup"><span data-stu-id="9cd8a-124">Header</span></span>        | <span data-ttu-id="9cd8a-125">值</span><span class="sxs-lookup"><span data-stu-id="9cd8a-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="9cd8a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cd8a-126">Authorization</span></span> | <span data-ttu-id="9cd8a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9cd8a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9cd8a-129">Content-Type</span></span>  | <span data-ttu-id="9cd8a-130">application/json</span><span class="sxs-lookup"><span data-stu-id="9cd8a-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="9cd8a-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cd8a-131">Request body</span></span>

<span data-ttu-id="9cd8a-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9cd8a-133">参数</span><span class="sxs-lookup"><span data-stu-id="9cd8a-133">Parameter</span></span>           | <span data-ttu-id="9cd8a-134">类型</span><span class="sxs-lookup"><span data-stu-id="9cd8a-134">Type</span></span>    | <span data-ttu-id="9cd8a-135">说明</span><span class="sxs-lookup"><span data-stu-id="9cd8a-135">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9cd8a-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="9cd8a-136">securityEnabledOnly</span></span> | <span data-ttu-id="9cd8a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="9cd8a-137">Boolean</span></span> | <span data-ttu-id="9cd8a-p106">**true** 指定仅应返回用户是其成员的安全组；**false** 指定应返回用户是其成员的所有组。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="9cd8a-140">响应</span><span class="sxs-lookup"><span data-stu-id="9cd8a-140">Response</span></span>

<span data-ttu-id="9cd8a-141">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和字符串集合，响应正文中包括用户是其成员的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="9cd8a-142">示例</span><span class="sxs-lookup"><span data-stu-id="9cd8a-142">Example</span></span>

<span data-ttu-id="9cd8a-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9cd8a-144">请求</span><span class="sxs-lookup"><span data-stu-id="9cd8a-144">Request</span></span>

<span data-ttu-id="9cd8a-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-145">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9cd8a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cd8a-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9cd8a-147">C#</span><span class="sxs-lookup"><span data-stu-id="9cd8a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9cd8a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cd8a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9cd8a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cd8a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9cd8a-150">响应</span><span class="sxs-lookup"><span data-stu-id="9cd8a-150">Response</span></span>

<span data-ttu-id="9cd8a-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9cd8a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
