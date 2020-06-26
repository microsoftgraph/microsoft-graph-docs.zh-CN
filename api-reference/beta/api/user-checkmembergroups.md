---
title: checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: e5559e2c581e573e8154168ba5bd1db39cdb536e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896474"
---
# <a name="checkmembergroups"></a><span data-ttu-id="ba4e4-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ba4e4-104">checkMemberGroups</span></span>

<span data-ttu-id="ba4e4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba4e4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba4e4-106">Check for membership in the specified list of groups.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-106">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="ba4e4-107">Returns from the list those groups of which the user has a direct or transitive membership.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-107">Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="ba4e4-108">You can check up to a maximum of 20 groups per request.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-108">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="ba4e4-109">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-109">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span></span> <span data-ttu-id="ba4e4-110">Note that Microsoft 365 groups cannot contain groups.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-110">Note that Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="ba4e4-111">So membership in a Microsoft 365 group is always direct.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-111">So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba4e4-112">权限</span><span class="sxs-lookup"><span data-stu-id="ba4e4-112">Permissions</span></span>

<span data-ttu-id="ba4e4-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ba4e4-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba4e4-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba4e4-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba4e4-115">Permission type</span></span>                        | <span data-ttu-id="ba4e4-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba4e4-116">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ba4e4-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba4e4-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba4e4-118">User.ReadBasic.All 和 GroupMember.Read.All、User.Read.All 和 GroupMember.Read.All、User.ReadBasic.All 和 Group.Read.All、User.Read.All 和 Group.Read.All、User.ReadWrite.All 和 GroupMember.Read.All、User.ReadWrite.All 和 Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba4e4-118">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ba4e4-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba4e4-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba4e4-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba4e4-120">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="ba4e4-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba4e4-121">Application</span></span>                            | <span data-ttu-id="ba4e4-122">GroupMember、user. all 和 Group. all、user. all 和 group. all、all 和 Group。 all，all，Read. all，all，all，all： all，all： all，all： all</span><span class="sxs-lookup"><span data-stu-id="ba4e4-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba4e4-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba4e4-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="ba4e4-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba4e4-124">Request headers</span></span>

| <span data-ttu-id="ba4e4-125">标头</span><span class="sxs-lookup"><span data-stu-id="ba4e4-125">Header</span></span>        | <span data-ttu-id="ba4e4-126">值</span><span class="sxs-lookup"><span data-stu-id="ba4e4-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ba4e4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba4e4-127">Authorization</span></span> | <span data-ttu-id="ba4e4-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-128">Bearer {token}.</span></span> <span data-ttu-id="ba4e4-129">Required.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-129">Required.</span></span> |
| <span data-ttu-id="ba4e4-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba4e4-130">Content-Type</span></span>  | <span data-ttu-id="ba4e4-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ba4e4-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="ba4e4-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba4e4-132">Request body</span></span>

<span data-ttu-id="ba4e4-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ba4e4-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ba4e4-134">参数</span><span class="sxs-lookup"><span data-stu-id="ba4e4-134">Parameter</span></span> | <span data-ttu-id="ba4e4-135">类型</span><span class="sxs-lookup"><span data-stu-id="ba4e4-135">Type</span></span>   | <span data-ttu-id="ba4e4-136">说明</span><span class="sxs-lookup"><span data-stu-id="ba4e4-136">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="ba4e4-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="ba4e4-137">groupIds</span></span>  | <span data-ttu-id="ba4e4-138">String collection</span><span class="sxs-lookup"><span data-stu-id="ba4e4-138">String collection</span></span> | <span data-ttu-id="ba4e4-139">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="ba4e4-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="ba4e4-140">响应</span><span class="sxs-lookup"><span data-stu-id="ba4e4-140">Response</span></span>

<span data-ttu-id="ba4e4-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="ba4e4-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba4e4-142">示例</span><span class="sxs-lookup"><span data-stu-id="ba4e4-142">Example</span></span>

<span data-ttu-id="ba4e4-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ba4e4-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ba4e4-144">请求</span><span class="sxs-lookup"><span data-stu-id="ba4e4-144">Request</span></span>

<span data-ttu-id="ba4e4-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba4e4-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba4e4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba4e4-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ba4e4-147">C#</span><span class="sxs-lookup"><span data-stu-id="ba4e4-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba4e4-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba4e4-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba4e4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba4e4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ba4e4-150">响应</span><span class="sxs-lookup"><span data-stu-id="ba4e4-150">Response</span></span>

<span data-ttu-id="ba4e4-151">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-151">Here is an example of the response.</span></span> <span data-ttu-id="ba4e4-152">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ba4e4-153">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ba4e4-153">All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
