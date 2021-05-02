---
title: 'user: getMemberGroups'
description: 返回用户是其成员的所有组。检查是可传递的，不同于读取
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a28a32ce1af781ea2d6eb05e18240067562c179a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055678"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="32548-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="32548-104">user: getMemberGroups</span></span>

<span data-ttu-id="32548-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32548-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32548-p102">返回用户是其成员的所有组。检查是可传递的，这和读取 [memberOf](../api/user-list-memberof.md) 导航属性不同，后者仅返回用户是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="32548-p102">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="32548-p103">此功能支持 Microsoft 365 和 Azure AD 中设置的其他类型的组。每个请求可以返回的最大组数为 2046 组。注意：Microsoft 365 组不能包含组。因此，Microsoft 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="32548-p103">This function supports Microsoft 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="32548-112">权限</span><span class="sxs-lookup"><span data-stu-id="32548-112">Permissions</span></span>

<span data-ttu-id="32548-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="32548-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="32548-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="32548-115">Permission type</span></span>                        | <span data-ttu-id="32548-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="32548-116">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="32548-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="32548-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="32548-118">User.ReadBasic.All、User.Read、User.Read.All、Directory.Read.All、User.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="32548-118">User.ReadBasic.All, User.Read, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="32548-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="32548-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32548-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="32548-120">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="32548-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="32548-121">Application</span></span>                            |  <span data-ttu-id="32548-122">User.Read.All、Directory.Read.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32548-122">User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32548-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="32548-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="32548-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="32548-124">Request headers</span></span>

| <span data-ttu-id="32548-125">标头</span><span class="sxs-lookup"><span data-stu-id="32548-125">Header</span></span>        | <span data-ttu-id="32548-126">值</span><span class="sxs-lookup"><span data-stu-id="32548-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="32548-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="32548-127">Authorization</span></span> | <span data-ttu-id="32548-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="32548-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="32548-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32548-130">Content-Type</span></span>  | <span data-ttu-id="32548-131">application/json</span><span class="sxs-lookup"><span data-stu-id="32548-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="32548-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="32548-132">Request body</span></span>

<span data-ttu-id="32548-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="32548-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="32548-134">参数</span><span class="sxs-lookup"><span data-stu-id="32548-134">Parameter</span></span>           | <span data-ttu-id="32548-135">类型</span><span class="sxs-lookup"><span data-stu-id="32548-135">Type</span></span>    | <span data-ttu-id="32548-136">说明</span><span class="sxs-lookup"><span data-stu-id="32548-136">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="32548-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="32548-137">securityEnabledOnly</span></span> | <span data-ttu-id="32548-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="32548-138">Boolean</span></span> | <span data-ttu-id="32548-p106">**true** 指定仅应返回用户是其成员的安全组；**false** 指定应返回用户是其成员的所有组。注意：仅当对用户调用这个方法时，才支持将此参数设置为 **true**。</span><span class="sxs-lookup"><span data-stu-id="32548-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="32548-141">响应</span><span class="sxs-lookup"><span data-stu-id="32548-141">Response</span></span>

<span data-ttu-id="32548-142">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和字符串集合，响应正文中包括用户是其成员的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="32548-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="32548-143">示例</span><span class="sxs-lookup"><span data-stu-id="32548-143">Example</span></span>

<span data-ttu-id="32548-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="32548-144">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="32548-145">请求</span><span class="sxs-lookup"><span data-stu-id="32548-145">Request</span></span>

<span data-ttu-id="32548-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="32548-146">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="32548-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="32548-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="32548-148">C#</span><span class="sxs-lookup"><span data-stu-id="32548-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32548-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32548-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32548-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32548-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32548-151">Java</span><span class="sxs-lookup"><span data-stu-id="32548-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32548-152">响应</span><span class="sxs-lookup"><span data-stu-id="32548-152">Response</span></span>

<span data-ttu-id="32548-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="32548-153">Here is an example of the response.</span></span> <span data-ttu-id="32548-154">注意：可能缩短此处显示的响应对象以提高可读性。</span><span class="sxs-lookup"><span data-stu-id="32548-154">Note: The response object shown here might be shortened for readability.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

