---
title: 'group: getMemberGroups'
description: 返回指定组是其成员的所有组。 检查是可传递的，这和读取 memberOf 导航属性不同，后者仅返回该组是其直接成员的组。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1e677d3aa033283417bfe6292d801455b425dff6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895844"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="2908e-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="2908e-104">group: getMemberGroups</span></span>

<span data-ttu-id="2908e-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2908e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2908e-106">Return all the groups that the specified group is a member of.</span><span class="sxs-lookup"><span data-stu-id="2908e-106">Return all the groups that the specified group is a member of.</span></span> <span data-ttu-id="2908e-107">The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span><span class="sxs-lookup"><span data-stu-id="2908e-107">The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="2908e-108">此函数支持在 Azure AD 中预配的 Microsoft 365 和其他类型的组。</span><span class="sxs-lookup"><span data-stu-id="2908e-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span></span> <span data-ttu-id="2908e-109">每个请求可以返回的最大组数为 2046 组。</span><span class="sxs-lookup"><span data-stu-id="2908e-109">The maximum number of groups each request can return is 2046.</span></span> <span data-ttu-id="2908e-110">请注意，Microsoft 365 组不能包含组。</span><span class="sxs-lookup"><span data-stu-id="2908e-110">Note that Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="2908e-111">因此，Microsoft 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="2908e-111">So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="2908e-112">权限</span><span class="sxs-lookup"><span data-stu-id="2908e-112">Permissions</span></span>

<span data-ttu-id="2908e-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2908e-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2908e-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2908e-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2908e-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="2908e-115">Permission type</span></span>                        | <span data-ttu-id="2908e-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2908e-116">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="2908e-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2908e-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="2908e-118">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2908e-118">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2908e-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2908e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2908e-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="2908e-120">Not supported.</span></span>                                                                              |
| <span data-ttu-id="2908e-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="2908e-121">Application</span></span>                            | <span data-ttu-id="2908e-122">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2908e-122">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="2908e-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2908e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="2908e-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2908e-124">Request headers</span></span>

| <span data-ttu-id="2908e-125">名称</span><span class="sxs-lookup"><span data-stu-id="2908e-125">Name</span></span>          | <span data-ttu-id="2908e-126">类型</span><span class="sxs-lookup"><span data-stu-id="2908e-126">Type</span></span>   | <span data-ttu-id="2908e-127">说明</span><span class="sxs-lookup"><span data-stu-id="2908e-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="2908e-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2908e-128">Authorization</span></span> | <span data-ttu-id="2908e-129">string</span><span class="sxs-lookup"><span data-stu-id="2908e-129">string</span></span> | <span data-ttu-id="2908e-130">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="2908e-130">Bearer {token}.</span></span> <span data-ttu-id="2908e-131">Required.</span><span class="sxs-lookup"><span data-stu-id="2908e-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2908e-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="2908e-132">Request body</span></span>

<span data-ttu-id="2908e-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2908e-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2908e-134">参数</span><span class="sxs-lookup"><span data-stu-id="2908e-134">Parameter</span></span>           | <span data-ttu-id="2908e-135">类型</span><span class="sxs-lookup"><span data-stu-id="2908e-135">Type</span></span>    | <span data-ttu-id="2908e-136">说明</span><span class="sxs-lookup"><span data-stu-id="2908e-136">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="2908e-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="2908e-137">securityEnabledOnly</span></span> | <span data-ttu-id="2908e-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="2908e-138">Boolean</span></span> | <span data-ttu-id="2908e-139">Set to **false**.</span><span class="sxs-lookup"><span data-stu-id="2908e-139">Set to **false**.</span></span> <span data-ttu-id="2908e-140">Returning only security-enabled groups is supported for users only.</span><span class="sxs-lookup"><span data-stu-id="2908e-140">Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="2908e-141">响应</span><span class="sxs-lookup"><span data-stu-id="2908e-141">Response</span></span>

<span data-ttu-id="2908e-142">如果成功，此方法将在包含该组所属组 ID 的响应正文中返回 `200 OK` 响应代码和字符串集合。</span><span class="sxs-lookup"><span data-stu-id="2908e-142">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="2908e-143">示例</span><span class="sxs-lookup"><span data-stu-id="2908e-143">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2908e-144">请求</span><span class="sxs-lookup"><span data-stu-id="2908e-144">Request</span></span>

<span data-ttu-id="2908e-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2908e-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2908e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="2908e-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2908e-147">C#</span><span class="sxs-lookup"><span data-stu-id="2908e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2908e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2908e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2908e-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2908e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2908e-150">响应</span><span class="sxs-lookup"><span data-stu-id="2908e-150">Response</span></span>

<span data-ttu-id="2908e-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2908e-151">The following is an example of the response.</span></span>

> <span data-ttu-id="2908e-152">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="2908e-152">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2908e-153">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2908e-153">All the properties will be returned from an actual call.</span></span>

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
