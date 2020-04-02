---
title: checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: d26b28a0b94d4316271a217a0e9d73b2d4e78125
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107967"
---
# <a name="checkmembergroups"></a><span data-ttu-id="ba355-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="ba355-104">checkMemberGroups</span></span>

<span data-ttu-id="ba355-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba355-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba355-p102">检查指定组列表中的成员身份。从列表中返回用户具有直接或可传递成员身份的组。</span><span class="sxs-lookup"><span data-stu-id="ba355-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="ba355-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="ba355-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba355-112">权限</span><span class="sxs-lookup"><span data-stu-id="ba355-112">Permissions</span></span>

<span data-ttu-id="ba355-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba355-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba355-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba355-115">Permission type</span></span>                        | <span data-ttu-id="ba355-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba355-116">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ba355-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba355-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba355-118">User.ReadBasic.All 和 GroupMember.Read.All、User.Read.All 和 GroupMember.Read.All、User.ReadBasic.All 和 Group.Read.All、User.Read.All 和 Group.Read.All、User.ReadWrite.All 和 GroupMember.Read.All、User.ReadWrite.All 和 Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba355-118">User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="ba355-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba355-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba355-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba355-120">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="ba355-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba355-121">Application</span></span>                            | <span data-ttu-id="ba355-122">GroupMember、user. all 和 Group. all、user. all 和 group. all、all 和 Group。 all，all，Read. all，all，all，all： all，all： all，all： all</span><span class="sxs-lookup"><span data-stu-id="ba355-122">User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, User.ReadWrite.All and GroupMember.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba355-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba355-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="ba355-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba355-124">Request headers</span></span>

| <span data-ttu-id="ba355-125">标头</span><span class="sxs-lookup"><span data-stu-id="ba355-125">Header</span></span>        | <span data-ttu-id="ba355-126">值</span><span class="sxs-lookup"><span data-stu-id="ba355-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="ba355-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba355-127">Authorization</span></span> | <span data-ttu-id="ba355-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba355-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba355-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba355-130">Content-Type</span></span>  | <span data-ttu-id="ba355-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ba355-131">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="ba355-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba355-132">Request body</span></span>

<span data-ttu-id="ba355-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ba355-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ba355-134">参数</span><span class="sxs-lookup"><span data-stu-id="ba355-134">Parameter</span></span> | <span data-ttu-id="ba355-135">类型</span><span class="sxs-lookup"><span data-stu-id="ba355-135">Type</span></span>   | <span data-ttu-id="ba355-136">说明</span><span class="sxs-lookup"><span data-stu-id="ba355-136">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="ba355-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="ba355-137">groupIds</span></span>  | <span data-ttu-id="ba355-138">String collection</span><span class="sxs-lookup"><span data-stu-id="ba355-138">String collection</span></span> | <span data-ttu-id="ba355-139">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="ba355-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="ba355-140">响应</span><span class="sxs-lookup"><span data-stu-id="ba355-140">Response</span></span>

<span data-ttu-id="ba355-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="ba355-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba355-142">示例</span><span class="sxs-lookup"><span data-stu-id="ba355-142">Example</span></span>

<span data-ttu-id="ba355-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ba355-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="ba355-144">请求</span><span class="sxs-lookup"><span data-stu-id="ba355-144">Request</span></span>

<span data-ttu-id="ba355-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ba355-145">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba355-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba355-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ba355-147">C#</span><span class="sxs-lookup"><span data-stu-id="ba355-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba355-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba355-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba355-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba355-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ba355-150">响应</span><span class="sxs-lookup"><span data-stu-id="ba355-150">Response</span></span>

<span data-ttu-id="ba355-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ba355-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
