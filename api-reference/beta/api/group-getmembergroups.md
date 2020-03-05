---
title: 'group: getMemberGroups'
description: 返回指定组是其成员的所有组。 检查是可传递的，这和读取 memberOf 导航属性不同，后者仅返回该组是其直接成员的组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b51ada7c1b9afde46401cb7bac04bd536088ac51
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419896"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="b40b7-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b40b7-104">group: getMemberGroups</span></span>

<span data-ttu-id="b40b7-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b40b7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b40b7-p102">返回指定组所属的所有组。检查是可传递的，这和读取 [memberOf](../api/group-list-memberof.md) 导航属性不同，后者仅返回该组是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="b40b7-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="b40b7-p103">此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。每个请求可以返回的最大组数为 2046 组。注意：Office 365 组不能包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="b40b7-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="b40b7-112">权限</span><span class="sxs-lookup"><span data-stu-id="b40b7-112">Permissions</span></span>

<span data-ttu-id="b40b7-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b40b7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b40b7-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="b40b7-115">Permission type</span></span>                        | <span data-ttu-id="b40b7-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b40b7-116">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="b40b7-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b40b7-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="b40b7-118">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b40b7-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="b40b7-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b40b7-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b40b7-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="b40b7-120">Not supported.</span></span>                                                                              |
| <span data-ttu-id="b40b7-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="b40b7-121">Application</span></span>                            | <span data-ttu-id="b40b7-122">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b40b7-122">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="b40b7-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b40b7-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="b40b7-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="b40b7-124">Request headers</span></span>

| <span data-ttu-id="b40b7-125">名称</span><span class="sxs-lookup"><span data-stu-id="b40b7-125">Name</span></span>          | <span data-ttu-id="b40b7-126">类型</span><span class="sxs-lookup"><span data-stu-id="b40b7-126">Type</span></span>   | <span data-ttu-id="b40b7-127">说明</span><span class="sxs-lookup"><span data-stu-id="b40b7-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="b40b7-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b40b7-128">Authorization</span></span> | <span data-ttu-id="b40b7-129">string</span><span class="sxs-lookup"><span data-stu-id="b40b7-129">string</span></span> | <span data-ttu-id="b40b7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b40b7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b40b7-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b40b7-132">Request body</span></span>

<span data-ttu-id="b40b7-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b40b7-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b40b7-134">参数</span><span class="sxs-lookup"><span data-stu-id="b40b7-134">Parameter</span></span>           | <span data-ttu-id="b40b7-135">类型</span><span class="sxs-lookup"><span data-stu-id="b40b7-135">Type</span></span>    | <span data-ttu-id="b40b7-136">说明</span><span class="sxs-lookup"><span data-stu-id="b40b7-136">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="b40b7-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="b40b7-137">securityEnabledOnly</span></span> | <span data-ttu-id="b40b7-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="b40b7-138">Boolean</span></span> | <span data-ttu-id="b40b7-p106">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="b40b7-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="b40b7-141">响应</span><span class="sxs-lookup"><span data-stu-id="b40b7-141">Response</span></span>

<span data-ttu-id="b40b7-142">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="b40b7-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="b40b7-143">示例</span><span class="sxs-lookup"><span data-stu-id="b40b7-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b40b7-144">请求</span><span class="sxs-lookup"><span data-stu-id="b40b7-144">Request</span></span>

<span data-ttu-id="b40b7-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b40b7-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b40b7-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b40b7-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="b40b7-147">C#</span><span class="sxs-lookup"><span data-stu-id="b40b7-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b40b7-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b40b7-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b40b7-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b40b7-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b40b7-150">响应</span><span class="sxs-lookup"><span data-stu-id="b40b7-150">Response</span></span>

<span data-ttu-id="b40b7-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b40b7-151">The following is an example of the response.</span></span>

> <span data-ttu-id="b40b7-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b40b7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
