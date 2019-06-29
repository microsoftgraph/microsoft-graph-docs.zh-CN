---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 524cfeff7a01de50d33224089557ecd62081dc77
ms.sourcegitcommit: 6d8bf390380b9434ba626d6dc5101afcf6ba6f8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2019
ms.locfileid: "35395147"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="f7c9f-104">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f7c9f-104">group: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c9f-p102">检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="f7c9f-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7c9f-111">权限</span><span class="sxs-lookup"><span data-stu-id="f7c9f-111">Permissions</span></span>

<span data-ttu-id="f7c9f-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7c9f-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7c9f-114">Permission type</span></span>                        | <span data-ttu-id="f7c9f-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7c9f-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="f7c9f-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c9f-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7c9f-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7c9f-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f7c9f-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c9f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7c9f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="f7c9f-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7c9f-120">Application</span></span>                            | <span data-ttu-id="f7c9f-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7c9f-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="f7c9f-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7c9f-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="f7c9f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7c9f-123">Request headers</span></span>

| <span data-ttu-id="f7c9f-124">名称</span><span class="sxs-lookup"><span data-stu-id="f7c9f-124">Name</span></span>          | <span data-ttu-id="f7c9f-125">类型</span><span class="sxs-lookup"><span data-stu-id="f7c9f-125">Type</span></span>   | <span data-ttu-id="f7c9f-126">说明</span><span class="sxs-lookup"><span data-stu-id="f7c9f-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="f7c9f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7c9f-127">Authorization</span></span> | <span data-ttu-id="f7c9f-128">string</span><span class="sxs-lookup"><span data-stu-id="f7c9f-128">string</span></span> | <span data-ttu-id="f7c9f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7c9f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7c9f-131">Request body</span></span>

<span data-ttu-id="f7c9f-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7c9f-133">参数</span><span class="sxs-lookup"><span data-stu-id="f7c9f-133">Parameter</span></span> | <span data-ttu-id="f7c9f-134">类型</span><span class="sxs-lookup"><span data-stu-id="f7c9f-134">Type</span></span>   | <span data-ttu-id="f7c9f-135">说明</span><span class="sxs-lookup"><span data-stu-id="f7c9f-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="f7c9f-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="f7c9f-136">groupIds</span></span>  | <span data-ttu-id="f7c9f-137">String collection</span><span class="sxs-lookup"><span data-stu-id="f7c9f-137">String collection</span></span> | <span data-ttu-id="f7c9f-138">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="f7c9f-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="f7c9f-139">响应</span><span class="sxs-lookup"><span data-stu-id="f7c9f-139">Response</span></span>

<span data-ttu-id="f7c9f-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c9f-141">示例</span><span class="sxs-lookup"><span data-stu-id="f7c9f-141">Example</span></span>

<span data-ttu-id="f7c9f-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f7c9f-143">请求</span><span class="sxs-lookup"><span data-stu-id="f7c9f-143">Request</span></span>

<span data-ttu-id="f7c9f-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-144">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="f7c9f-145">响应</span><span class="sxs-lookup"><span data-stu-id="f7c9f-145">Response</span></span>

<span data-ttu-id="f7c9f-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7c9f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f7c9f-149">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f7c9f-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f7c9f-150">C#</span><span class="sxs-lookup"><span data-stu-id="f7c9f-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7c9f-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7c9f-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f7c9f-152">目标-C</span><span class="sxs-lookup"><span data-stu-id="f7c9f-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
