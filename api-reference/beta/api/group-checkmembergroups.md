---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9235d8b30801c32d2428f4086ab8ce22ed021fa3
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895872"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="6d98d-103">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="6d98d-103">group: checkMemberGroups</span></span>

<span data-ttu-id="6d98d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d98d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d98d-105">Check for membership in the specified list of groups.</span><span class="sxs-lookup"><span data-stu-id="6d98d-105">Check for membership in the specified list of groups.</span></span> <span data-ttu-id="6d98d-106">Returns from the list those groups of which the specified group has a direct or transitive membership.</span><span class="sxs-lookup"><span data-stu-id="6d98d-106">Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="6d98d-107">You can check up to a maximum of 20 groups per request.</span><span class="sxs-lookup"><span data-stu-id="6d98d-107">You can check up to a maximum of 20 groups per request.</span></span> <span data-ttu-id="6d98d-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6d98d-108">This function supports Microsoft 365 and other types of groups provisioned in Azure AD.</span></span> <span data-ttu-id="6d98d-109">Note that Microsoft 365 groups cannot contain groups.</span><span class="sxs-lookup"><span data-stu-id="6d98d-109">Note that Microsoft 365 groups cannot contain groups.</span></span> <span data-ttu-id="6d98d-110">So membership in a Microsoft 365 group is always direct.</span><span class="sxs-lookup"><span data-stu-id="6d98d-110">So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d98d-111">权限</span><span class="sxs-lookup"><span data-stu-id="6d98d-111">Permissions</span></span>

<span data-ttu-id="6d98d-112">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6d98d-112">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6d98d-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d98d-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d98d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d98d-114">Permission type</span></span>                        | <span data-ttu-id="6d98d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d98d-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="6d98d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d98d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d98d-117">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d98d-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="6d98d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d98d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d98d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d98d-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="6d98d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d98d-120">Application</span></span>                            | <span data-ttu-id="6d98d-121">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d98d-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="6d98d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d98d-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="6d98d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d98d-123">Request headers</span></span>

| <span data-ttu-id="6d98d-124">名称</span><span class="sxs-lookup"><span data-stu-id="6d98d-124">Name</span></span>          | <span data-ttu-id="6d98d-125">类型</span><span class="sxs-lookup"><span data-stu-id="6d98d-125">Type</span></span>   | <span data-ttu-id="6d98d-126">说明</span><span class="sxs-lookup"><span data-stu-id="6d98d-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="6d98d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d98d-127">Authorization</span></span> | <span data-ttu-id="6d98d-128">string</span><span class="sxs-lookup"><span data-stu-id="6d98d-128">string</span></span> | <span data-ttu-id="6d98d-129">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6d98d-129">Bearer {token}.</span></span> <span data-ttu-id="6d98d-130">Required.</span><span class="sxs-lookup"><span data-stu-id="6d98d-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d98d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d98d-131">Request body</span></span>

<span data-ttu-id="6d98d-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6d98d-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6d98d-133">参数</span><span class="sxs-lookup"><span data-stu-id="6d98d-133">Parameter</span></span> | <span data-ttu-id="6d98d-134">类型</span><span class="sxs-lookup"><span data-stu-id="6d98d-134">Type</span></span>   | <span data-ttu-id="6d98d-135">说明</span><span class="sxs-lookup"><span data-stu-id="6d98d-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="6d98d-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="6d98d-136">groupIds</span></span>  | <span data-ttu-id="6d98d-137">String collection</span><span class="sxs-lookup"><span data-stu-id="6d98d-137">String collection</span></span> | <span data-ttu-id="6d98d-138">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="6d98d-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="6d98d-139">响应</span><span class="sxs-lookup"><span data-stu-id="6d98d-139">Response</span></span>

<span data-ttu-id="6d98d-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="6d98d-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d98d-141">示例</span><span class="sxs-lookup"><span data-stu-id="6d98d-141">Example</span></span>

<span data-ttu-id="6d98d-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6d98d-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="6d98d-143">请求</span><span class="sxs-lookup"><span data-stu-id="6d98d-143">Request</span></span>

<span data-ttu-id="6d98d-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d98d-144">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6d98d-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d98d-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="6d98d-146">C#</span><span class="sxs-lookup"><span data-stu-id="6d98d-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d98d-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d98d-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d98d-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d98d-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6d98d-149">响应</span><span class="sxs-lookup"><span data-stu-id="6d98d-149">Response</span></span>

<span data-ttu-id="6d98d-150">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="6d98d-150">Here is an example of the response.</span></span> <span data-ttu-id="6d98d-151">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="6d98d-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6d98d-152">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6d98d-152">All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
