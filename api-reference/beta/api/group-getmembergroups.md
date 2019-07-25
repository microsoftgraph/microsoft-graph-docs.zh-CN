---
title: 'group: getMemberGroups'
description: 返回指定组是其成员的所有组。 检查是可传递的，这和读取 memberOf 导航属性不同，后者仅返回该组是其直接成员的组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 51ab29cfd44f9812d994cabcfdd5531f03f893cb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858581"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="981f6-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="981f6-104">group: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="981f6-p102">返回指定组所属的所有组。检查是可传递的，这和读取 [memberOf](../api/group-list-memberof.md) 导航属性不同，后者仅返回该组是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="981f6-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="981f6-p103">此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。每个请求可以返回的最大组数为 2046 组。注意：Office 365 组不能包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="981f6-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="981f6-111">权限</span><span class="sxs-lookup"><span data-stu-id="981f6-111">Permissions</span></span>

<span data-ttu-id="981f6-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="981f6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="981f6-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="981f6-114">Permission type</span></span>                        | <span data-ttu-id="981f6-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="981f6-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="981f6-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="981f6-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="981f6-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="981f6-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="981f6-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="981f6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="981f6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="981f6-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="981f6-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="981f6-120">Application</span></span>                            | <span data-ttu-id="981f6-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="981f6-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="981f6-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="981f6-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="981f6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="981f6-123">Request headers</span></span>

| <span data-ttu-id="981f6-124">名称</span><span class="sxs-lookup"><span data-stu-id="981f6-124">Name</span></span>          | <span data-ttu-id="981f6-125">类型</span><span class="sxs-lookup"><span data-stu-id="981f6-125">Type</span></span>   | <span data-ttu-id="981f6-126">说明</span><span class="sxs-lookup"><span data-stu-id="981f6-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="981f6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="981f6-127">Authorization</span></span> | <span data-ttu-id="981f6-128">string</span><span class="sxs-lookup"><span data-stu-id="981f6-128">string</span></span> | <span data-ttu-id="981f6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="981f6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="981f6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="981f6-131">Request body</span></span>

<span data-ttu-id="981f6-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="981f6-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="981f6-133">参数</span><span class="sxs-lookup"><span data-stu-id="981f6-133">Parameter</span></span>           | <span data-ttu-id="981f6-134">类型</span><span class="sxs-lookup"><span data-stu-id="981f6-134">Type</span></span>    | <span data-ttu-id="981f6-135">说明</span><span class="sxs-lookup"><span data-stu-id="981f6-135">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="981f6-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="981f6-136">securityEnabledOnly</span></span> | <span data-ttu-id="981f6-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="981f6-137">Boolean</span></span> | <span data-ttu-id="981f6-p106">设置为 **false**。只支持对用户仅返回启用安全机制的组。</span><span class="sxs-lookup"><span data-stu-id="981f6-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="981f6-140">响应</span><span class="sxs-lookup"><span data-stu-id="981f6-140">Response</span></span>

<span data-ttu-id="981f6-141">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="981f6-141">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="981f6-142">示例</span><span class="sxs-lookup"><span data-stu-id="981f6-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="981f6-143">请求</span><span class="sxs-lookup"><span data-stu-id="981f6-143">Request</span></span>

<span data-ttu-id="981f6-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="981f6-144">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="981f6-145">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="981f6-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="981f6-146">C#</span><span class="sxs-lookup"><span data-stu-id="981f6-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="981f6-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="981f6-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="981f6-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="981f6-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="981f6-149">Java</span><span class="sxs-lookup"><span data-stu-id="981f6-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="981f6-150">响应</span><span class="sxs-lookup"><span data-stu-id="981f6-150">Response</span></span>

<span data-ttu-id="981f6-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="981f6-151">The following is an example of the response.</span></span>

> <span data-ttu-id="981f6-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="981f6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
