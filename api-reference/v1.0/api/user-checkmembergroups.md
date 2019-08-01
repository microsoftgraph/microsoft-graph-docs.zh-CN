---
title: checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 78fd3bb0ef74a9c55c67964c1164b509ecc9a096
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027158"
---
# <a name="checkmembergroups"></a><span data-ttu-id="f9283-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f9283-104">checkMemberGroups</span></span>

<span data-ttu-id="f9283-p102">检查指定组列表中的成员身份。从列表中返回用户具有直接或可传递成员身份的组。</span><span class="sxs-lookup"><span data-stu-id="f9283-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="f9283-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="f9283-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9283-111">权限</span><span class="sxs-lookup"><span data-stu-id="f9283-111">Permissions</span></span>

<span data-ttu-id="f9283-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9283-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f9283-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9283-114">Permission type</span></span>                        | <span data-ttu-id="f9283-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9283-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f9283-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9283-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="f9283-117">User.ReadBasic.All 和 Group.Read.All、User.Read.All 和 Group.Read.All、User.ReadWrite.All 和 Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9283-117">User.Read and Group.Read.All, User.ReadBasic.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="f9283-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9283-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9283-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9283-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="f9283-120">Application</span><span class="sxs-lookup"><span data-stu-id="f9283-120">Application</span></span>                            | <span data-ttu-id="f9283-121">User.Read.All 和 Group.Read.All、User.ReadWrite.All 和 Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9283-121">User.Read.All and Group.Read.All, User.ReadWrite.All and Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9283-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9283-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="f9283-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9283-123">Request headers</span></span>

| <span data-ttu-id="f9283-124">标头</span><span class="sxs-lookup"><span data-stu-id="f9283-124">Header</span></span>        | <span data-ttu-id="f9283-125">值</span><span class="sxs-lookup"><span data-stu-id="f9283-125">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="f9283-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9283-126">Authorization</span></span> | <span data-ttu-id="f9283-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9283-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f9283-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9283-129">Content-Type</span></span>  | <span data-ttu-id="f9283-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f9283-130">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="f9283-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9283-131">Request body</span></span>

<span data-ttu-id="f9283-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f9283-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f9283-133">参数</span><span class="sxs-lookup"><span data-stu-id="f9283-133">Parameter</span></span> | <span data-ttu-id="f9283-134">类型</span><span class="sxs-lookup"><span data-stu-id="f9283-134">Type</span></span>              | <span data-ttu-id="f9283-135">说明</span><span class="sxs-lookup"><span data-stu-id="f9283-135">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="f9283-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="f9283-136">groupIds</span></span>  | <span data-ttu-id="f9283-137">String collection</span><span class="sxs-lookup"><span data-stu-id="f9283-137">String collection</span></span> | <span data-ttu-id="f9283-138">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="f9283-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="f9283-139">响应</span><span class="sxs-lookup"><span data-stu-id="f9283-139">Response</span></span>

<span data-ttu-id="f9283-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="f9283-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9283-141">示例</span><span class="sxs-lookup"><span data-stu-id="f9283-141">Example</span></span>

<span data-ttu-id="f9283-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f9283-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="f9283-143">请求</span><span class="sxs-lookup"><span data-stu-id="f9283-143">Request</span></span>

<span data-ttu-id="f9283-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9283-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f9283-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9283-145">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f9283-146">C#</span><span class="sxs-lookup"><span data-stu-id="f9283-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9283-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="f9283-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f9283-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9283-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f9283-149">Java</span><span class="sxs-lookup"><span data-stu-id="f9283-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9283-150">响应</span><span class="sxs-lookup"><span data-stu-id="f9283-150">Response</span></span>

<span data-ttu-id="f9283-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9283-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
