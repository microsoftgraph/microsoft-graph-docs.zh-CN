---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 49830cfd8669ea44ac386bdc394e5582e5e5e3d3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042147"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="dde29-103">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="dde29-103">group: checkMemberGroups</span></span>

<span data-ttu-id="dde29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dde29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dde29-p101">检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。</span><span class="sxs-lookup"><span data-stu-id="dde29-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="dde29-p102">每个请求最多可检查 20 个组。此功能支持 Microsoft 365 和 Azure AD 中设置的其他类型的组。注意：Microsoft 365 组无法包含组。因此，Microsoft 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="dde29-p102">You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="dde29-111">权限</span><span class="sxs-lookup"><span data-stu-id="dde29-111">Permissions</span></span>

<span data-ttu-id="dde29-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dde29-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dde29-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="dde29-114">Permission type</span></span>                        | <span data-ttu-id="dde29-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dde29-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="dde29-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dde29-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="dde29-117">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dde29-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="dde29-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dde29-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dde29-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="dde29-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="dde29-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="dde29-120">Application</span></span>                            | <span data-ttu-id="dde29-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dde29-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="dde29-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dde29-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="dde29-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="dde29-123">Request headers</span></span>

| <span data-ttu-id="dde29-124">名称</span><span class="sxs-lookup"><span data-stu-id="dde29-124">Name</span></span>          | <span data-ttu-id="dde29-125">类型</span><span class="sxs-lookup"><span data-stu-id="dde29-125">Type</span></span>   | <span data-ttu-id="dde29-126">说明</span><span class="sxs-lookup"><span data-stu-id="dde29-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="dde29-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="dde29-127">Authorization</span></span> | <span data-ttu-id="dde29-128">string</span><span class="sxs-lookup"><span data-stu-id="dde29-128">string</span></span> | <span data-ttu-id="dde29-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dde29-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dde29-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="dde29-131">Request body</span></span>

<span data-ttu-id="dde29-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dde29-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dde29-133">参数</span><span class="sxs-lookup"><span data-stu-id="dde29-133">Parameter</span></span> | <span data-ttu-id="dde29-134">类型</span><span class="sxs-lookup"><span data-stu-id="dde29-134">Type</span></span>   | <span data-ttu-id="dde29-135">说明</span><span class="sxs-lookup"><span data-stu-id="dde29-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="dde29-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="dde29-136">groupIds</span></span>  | <span data-ttu-id="dde29-137">String collection</span><span class="sxs-lookup"><span data-stu-id="dde29-137">String collection</span></span> | <span data-ttu-id="dde29-138">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="dde29-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="dde29-139">响应</span><span class="sxs-lookup"><span data-stu-id="dde29-139">Response</span></span>

<span data-ttu-id="dde29-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="dde29-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dde29-141">示例</span><span class="sxs-lookup"><span data-stu-id="dde29-141">Example</span></span>

<span data-ttu-id="dde29-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="dde29-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="dde29-143">请求</span><span class="sxs-lookup"><span data-stu-id="dde29-143">Request</span></span>

<span data-ttu-id="dde29-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dde29-144">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dde29-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="dde29-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dde29-146">C#</span><span class="sxs-lookup"><span data-stu-id="dde29-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dde29-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dde29-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dde29-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dde29-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dde29-149">Java</span><span class="sxs-lookup"><span data-stu-id="dde29-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dde29-150">响应</span><span class="sxs-lookup"><span data-stu-id="dde29-150">Response</span></span>

<span data-ttu-id="dde29-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dde29-151">Here is an example of the response.</span></span> <span data-ttu-id="dde29-152">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dde29-152">Note: The response object shown here might be shortened for readability.</span></span>

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


