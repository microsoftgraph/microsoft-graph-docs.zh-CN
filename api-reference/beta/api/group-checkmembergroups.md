---
title: 组：checkMemberGroups
description: 检查指定组列表中的成员身份。 从列表返回这些组
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b0919d702df6747f73643ee7b8f50a7538f5856f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326476"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="d8178-104">组：checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="d8178-104">group: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8178-p102">检查指定组列表中的成员身份。将列表中具有直接或可传递成员身份的指定组返回。</span><span class="sxs-lookup"><span data-stu-id="d8178-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="d8178-p103">每个请求最多可检查 20 个组。此功能支持 Office 365 和 Azure AD 中设置的其他类型的组。注意：Office 365 组无法包含组。因此，Office 365 组中的成员身份始终是直接的。</span><span class="sxs-lookup"><span data-stu-id="d8178-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8178-111">权限</span><span class="sxs-lookup"><span data-stu-id="d8178-111">Permissions</span></span>

<span data-ttu-id="d8178-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8178-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8178-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8178-114">Permission type</span></span>                        | <span data-ttu-id="d8178-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8178-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="d8178-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8178-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8178-117">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d8178-117">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="d8178-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8178-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8178-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8178-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="d8178-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8178-120">Application</span></span>                            | <span data-ttu-id="d8178-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8178-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

## <a name="http-request"></a><span data-ttu-id="d8178-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8178-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="d8178-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8178-123">Request headers</span></span>

| <span data-ttu-id="d8178-124">名称</span><span class="sxs-lookup"><span data-stu-id="d8178-124">Name</span></span>          | <span data-ttu-id="d8178-125">类型</span><span class="sxs-lookup"><span data-stu-id="d8178-125">Type</span></span>   | <span data-ttu-id="d8178-126">说明</span><span class="sxs-lookup"><span data-stu-id="d8178-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="d8178-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8178-127">Authorization</span></span> | <span data-ttu-id="d8178-128">string</span><span class="sxs-lookup"><span data-stu-id="d8178-128">string</span></span> | <span data-ttu-id="d8178-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d8178-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8178-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8178-131">Request body</span></span>

<span data-ttu-id="d8178-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d8178-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d8178-133">参数</span><span class="sxs-lookup"><span data-stu-id="d8178-133">Parameter</span></span> | <span data-ttu-id="d8178-134">类型</span><span class="sxs-lookup"><span data-stu-id="d8178-134">Type</span></span>   | <span data-ttu-id="d8178-135">说明</span><span class="sxs-lookup"><span data-stu-id="d8178-135">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="d8178-136">groupIds</span><span class="sxs-lookup"><span data-stu-id="d8178-136">groupIds</span></span>  | <span data-ttu-id="d8178-137">String collection</span><span class="sxs-lookup"><span data-stu-id="d8178-137">String collection</span></span> | <span data-ttu-id="d8178-138">组 ID 的数组</span><span class="sxs-lookup"><span data-stu-id="d8178-138">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="d8178-139">响应</span><span class="sxs-lookup"><span data-stu-id="d8178-139">Response</span></span>

<span data-ttu-id="d8178-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 String 集合对象。</span><span class="sxs-lookup"><span data-stu-id="d8178-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8178-141">示例</span><span class="sxs-lookup"><span data-stu-id="d8178-141">Example</span></span>

<span data-ttu-id="d8178-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d8178-142">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d8178-143">请求</span><span class="sxs-lookup"><span data-stu-id="d8178-143">Request</span></span>

<span data-ttu-id="d8178-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8178-144">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d8178-145">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d8178-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d8178-146">C#</span><span class="sxs-lookup"><span data-stu-id="d8178-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8178-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8178-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d8178-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="d8178-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d8178-149">Java</span><span class="sxs-lookup"><span data-stu-id="d8178-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8178-150">响应</span><span class="sxs-lookup"><span data-stu-id="d8178-150">Response</span></span>

<span data-ttu-id="d8178-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8178-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
