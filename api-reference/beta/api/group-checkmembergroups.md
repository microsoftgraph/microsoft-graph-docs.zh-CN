---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d85fd53a9639637c30646186c2cf8422272fe7d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990940"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="2f658-103">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="2f658-103">group: checkMemberGroups</span></span>

<span data-ttu-id="2f658-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f658-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f658-p101">检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。</span><span class="sxs-lookup"><span data-stu-id="2f658-p101">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="2f658-p102">每个请求最多可检查20个组。此函数支持在 Azure AD 中预配的 Microsoft 365 和其他类型的组。请注意，Microsoft 365 组不能包含组。因此，Microsoft 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="2f658-p102">You can check up to a maximum of 20 groups per request. This function supports Microsoft 365 and other types of groups provisioned in Azure AD. Note that Microsoft 365 groups cannot contain groups. So membership in a Microsoft 365 group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f658-111">权限</span><span class="sxs-lookup"><span data-stu-id="2f658-111">Permissions</span></span>

<span data-ttu-id="2f658-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f658-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f658-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f658-114">Permission type</span></span>                        | <span data-ttu-id="2f658-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f658-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="2f658-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f658-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f658-117">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2f658-117">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2f658-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f658-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f658-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f658-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="2f658-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f658-120">Application</span></span>                            | <span data-ttu-id="2f658-121">GroupMember.Read.All、Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f658-121">GroupMember.Read.All, Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="2f658-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f658-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="2f658-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f658-123">Request headers</span></span>

| <span data-ttu-id="2f658-124">名称</span><span class="sxs-lookup"><span data-stu-id="2f658-124">Name</span></span>          | <span data-ttu-id="2f658-125">类型</span><span class="sxs-lookup"><span data-stu-id="2f658-125">Type</span></span>   | <span data-ttu-id="2f658-126">说明</span><span class="sxs-lookup"><span data-stu-id="2f658-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="2f658-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f658-127">Authorization</span></span> | <span data-ttu-id="2f658-128">string</span><span class="sxs-lookup"><span data-stu-id="2f658-128">string</span></span> | <span data-ttu-id="2f658-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f658-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f658-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f658-131">Request body</span></span>

<span data-ttu-id="2f658-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2f658-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f658-133">参数</span><span class="sxs-lookup"><span data-stu-id="2f658-133">Parameter</span></span> | <span data-ttu-id="2f658-134">类型</span><span class="sxs-lookup"><span data-stu-id="2f658-134">Type</span></span>   | <span data-ttu-id="2f658-135">说明</span><span class="sxs-lookup"><span data-stu-id="2f658-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="2f658-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="2f658-136">groupIds</span></span>  | <span data-ttu-id="2f658-137">String collection</span><span class="sxs-lookup"><span data-stu-id="2f658-137">String collection</span></span> | <span data-ttu-id="2f658-138">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="2f658-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="2f658-139">响应</span><span class="sxs-lookup"><span data-stu-id="2f658-139">Response</span></span>

<span data-ttu-id="2f658-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="2f658-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f658-141">示例</span><span class="sxs-lookup"><span data-stu-id="2f658-141">Example</span></span>

<span data-ttu-id="2f658-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2f658-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2f658-143">请求</span><span class="sxs-lookup"><span data-stu-id="2f658-143">Request</span></span>

<span data-ttu-id="2f658-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2f658-144">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2f658-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f658-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2f658-146">C#</span><span class="sxs-lookup"><span data-stu-id="2f658-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f658-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f658-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f658-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f658-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2f658-149">响应</span><span class="sxs-lookup"><span data-stu-id="2f658-149">Response</span></span>

<span data-ttu-id="2f658-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2f658-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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


