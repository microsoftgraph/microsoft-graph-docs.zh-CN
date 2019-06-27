---
title: checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7d8a017372fde8174f70a5a3f2b6960892b73880
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270481"
---
# <a name="checkmembergroups"></a><span data-ttu-id="29ea9-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="29ea9-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29ea9-p102">检查指定组列表中的成员身份。从列表中返回用户具有直接或可传递成员身份的组。</span><span class="sxs-lookup"><span data-stu-id="29ea9-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="29ea9-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="29ea9-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="29ea9-111">权限</span><span class="sxs-lookup"><span data-stu-id="29ea9-111">Permissions</span></span>

<span data-ttu-id="29ea9-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29ea9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="29ea9-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="29ea9-114">Permission type</span></span>                        | <span data-ttu-id="29ea9-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29ea9-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="29ea9-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29ea9-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="29ea9-117">~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29ea9-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="29ea9-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29ea9-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29ea9-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="29ea9-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="29ea9-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="29ea9-120">Application</span></span>                            | <span data-ttu-id="29ea9-121">~~User.Read.All~~、~~User.ReadWrite.All~~、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29ea9-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="29ea9-122">**注意：** 此 API 当前需要 `Directory.Read.All` 权限或更高权限。</span><span class="sxs-lookup"><span data-stu-id="29ea9-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="29ea9-123">使用 `User.Read.All` 或 `User.ReadWrite.All` 权限将返回错误。</span><span class="sxs-lookup"><span data-stu-id="29ea9-123">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="29ea9-124">这是一个已知 bug。</span><span class="sxs-lookup"><span data-stu-id="29ea9-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="29ea9-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29ea9-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="29ea9-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="29ea9-126">Request headers</span></span>

| <span data-ttu-id="29ea9-127">标头</span><span class="sxs-lookup"><span data-stu-id="29ea9-127">Header</span></span>        | <span data-ttu-id="29ea9-128">值</span><span class="sxs-lookup"><span data-stu-id="29ea9-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="29ea9-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="29ea9-129">Authorization</span></span> | <span data-ttu-id="29ea9-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29ea9-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29ea9-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29ea9-132">Content-Type</span></span>  | <span data-ttu-id="29ea9-133">application/json</span><span class="sxs-lookup"><span data-stu-id="29ea9-133">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="29ea9-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="29ea9-134">Request body</span></span>

<span data-ttu-id="29ea9-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="29ea9-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="29ea9-136">参数</span><span class="sxs-lookup"><span data-stu-id="29ea9-136">Parameter</span></span> | <span data-ttu-id="29ea9-137">类型</span><span class="sxs-lookup"><span data-stu-id="29ea9-137">Type</span></span>   | <span data-ttu-id="29ea9-138">说明</span><span class="sxs-lookup"><span data-stu-id="29ea9-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="29ea9-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="29ea9-139">groupIds</span></span>  | <span data-ttu-id="29ea9-140">String collection</span><span class="sxs-lookup"><span data-stu-id="29ea9-140">String collection</span></span> | <span data-ttu-id="29ea9-141">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="29ea9-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="29ea9-142">响应</span><span class="sxs-lookup"><span data-stu-id="29ea9-142">Response</span></span>

<span data-ttu-id="29ea9-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="29ea9-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29ea9-144">示例</span><span class="sxs-lookup"><span data-stu-id="29ea9-144">Example</span></span>

<span data-ttu-id="29ea9-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="29ea9-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="29ea9-146">请求</span><span class="sxs-lookup"><span data-stu-id="29ea9-146">Request</span></span>

<span data-ttu-id="29ea9-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29ea9-147">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="29ea9-148">响应</span><span class="sxs-lookup"><span data-stu-id="29ea9-148">Response</span></span>

<span data-ttu-id="29ea9-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29ea9-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="29ea9-152">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="29ea9-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="29ea9-153">C#</span><span class="sxs-lookup"><span data-stu-id="29ea9-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_checkmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29ea9-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="29ea9-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_checkmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="29ea9-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="29ea9-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_checkmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-checkmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
