---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 9d76df33ac36ef936a1abfa873332c3be3aa0650
ms.sourcegitcommit: 6d8bf390380b9434ba626d6dc5101afcf6ba6f8b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2019
ms.locfileid: "35395182"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="93679-104">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="93679-104">group: checkMemberGroups</span></span>

<span data-ttu-id="93679-p102">检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。</span><span class="sxs-lookup"><span data-stu-id="93679-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="93679-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="93679-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="93679-111">权限</span><span class="sxs-lookup"><span data-stu-id="93679-111">Permissions</span></span>

<span data-ttu-id="93679-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93679-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93679-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="93679-114">Permission type</span></span>                        | <span data-ttu-id="93679-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93679-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="93679-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93679-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="93679-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93679-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="93679-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93679-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93679-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="93679-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="93679-120">Application</span><span class="sxs-lookup"><span data-stu-id="93679-120">Application</span></span>                            | <span data-ttu-id="93679-121">Group.Read.All、Directory.Read.All。</span><span class="sxs-lookup"><span data-stu-id="93679-121">Group.Read.All, Directory.Read.All.</span></span> <span data-ttu-id="93679-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93679-122">Directory.ReadWrite.All</span></span>                               |



## <a name="http-request"></a><span data-ttu-id="93679-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93679-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="93679-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="93679-124">Request headers</span></span>

| <span data-ttu-id="93679-125">名称</span><span class="sxs-lookup"><span data-stu-id="93679-125">Name</span></span>          | <span data-ttu-id="93679-126">类型</span><span class="sxs-lookup"><span data-stu-id="93679-126">Type</span></span>   | <span data-ttu-id="93679-127">说明</span><span class="sxs-lookup"><span data-stu-id="93679-127">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="93679-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="93679-128">Authorization</span></span> | <span data-ttu-id="93679-129">string</span><span class="sxs-lookup"><span data-stu-id="93679-129">string</span></span> | <span data-ttu-id="93679-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93679-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93679-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="93679-132">Request body</span></span>

<span data-ttu-id="93679-133">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="93679-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="93679-134">参数</span><span class="sxs-lookup"><span data-stu-id="93679-134">Parameter</span></span> | <span data-ttu-id="93679-135">类型</span><span class="sxs-lookup"><span data-stu-id="93679-135">Type</span></span>              | <span data-ttu-id="93679-136">说明</span><span class="sxs-lookup"><span data-stu-id="93679-136">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="93679-137">groupIds</span><span class="sxs-lookup"><span data-stu-id="93679-137">groupIds</span></span>  | <span data-ttu-id="93679-138">String collection</span><span class="sxs-lookup"><span data-stu-id="93679-138">String collection</span></span> | <span data-ttu-id="93679-139">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="93679-139">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="93679-140">响应</span><span class="sxs-lookup"><span data-stu-id="93679-140">Response</span></span>

<span data-ttu-id="93679-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="93679-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93679-142">示例</span><span class="sxs-lookup"><span data-stu-id="93679-142">Example</span></span>

<span data-ttu-id="93679-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="93679-143">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="93679-144">请求</span><span class="sxs-lookup"><span data-stu-id="93679-144">Request</span></span>

<span data-ttu-id="93679-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93679-145">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="93679-146">响应</span><span class="sxs-lookup"><span data-stu-id="93679-146">Response</span></span>

<span data-ttu-id="93679-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93679-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="93679-150">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="93679-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="93679-151">C#</span><span class="sxs-lookup"><span data-stu-id="93679-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93679-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="93679-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="93679-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93679-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
