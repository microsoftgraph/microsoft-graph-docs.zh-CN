---
title: directoryObject：validateProperties
description: 验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 699175bfd3d51deb07d64722a7196fcf9dcc8880
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436832"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="5d2af-103">directoryObject：validateProperties</span><span class="sxs-lookup"><span data-stu-id="5d2af-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="5d2af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d2af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d2af-105">验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="5d2af-105">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="5d2af-106">客户端可以使用此 API 在尝试创建 Microsoft 365 显示名称或邮件昵称是否有效。</span><span class="sxs-lookup"><span data-stu-id="5d2af-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to **create** a Microsoft 365 group.</span></span> <span data-ttu-id="5d2af-107">若要验证现有组的属性，请对组使用 [validateProperties](group-validateproperties.md) 函数。</span><span class="sxs-lookup"><span data-stu-id="5d2af-107">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="5d2af-108">对邮件和邮件昵称显示名称执行以下验证：</span><span class="sxs-lookup"><span data-stu-id="5d2af-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="5d2af-109">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="5d2af-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="5d2af-110">验证自定义禁止的词语策略</span><span class="sxs-lookup"><span data-stu-id="5d2af-110">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="5d2af-111">验证邮件昵称是否唯一</span><span class="sxs-lookup"><span data-stu-id="5d2af-111">Validate the mail nickname is unique</span></span>

<span data-ttu-id="5d2af-112">此 API 返回遇到的第一个故障。</span><span class="sxs-lookup"><span data-stu-id="5d2af-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="5d2af-113">如果一个或多个属性未能通过多次验证，则仅返回第一个验证失败的属性。</span><span class="sxs-lookup"><span data-stu-id="5d2af-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="5d2af-114">但是，如果仅验证前缀和后缀命名策略显示名称，您可以验证邮件昵称和别名，并接收验证错误集合。</span><span class="sxs-lookup"><span data-stu-id="5d2af-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d2af-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="5d2af-115">Permissions</span></span>
<span data-ttu-id="5d2af-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d2af-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d2af-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d2af-118">Permission type</span></span>      | <span data-ttu-id="5d2af-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d2af-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d2af-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d2af-120">Delegated (work or school account)</span></span> | <span data-ttu-id="5d2af-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5d2af-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="5d2af-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d2af-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d2af-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d2af-123">Not supported.</span></span>    |
|<span data-ttu-id="5d2af-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d2af-124">Application</span></span> | <span data-ttu-id="5d2af-125">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d2af-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d2af-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d2af-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="5d2af-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d2af-127">Request headers</span></span>

| <span data-ttu-id="5d2af-128">名称</span><span class="sxs-lookup"><span data-stu-id="5d2af-128">Name</span></span>           | <span data-ttu-id="5d2af-129">说明</span><span class="sxs-lookup"><span data-stu-id="5d2af-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="5d2af-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d2af-130">Authorization</span></span>  | <span data-ttu-id="5d2af-131">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="5d2af-131">Bearer {code}.</span></span> <span data-ttu-id="5d2af-132">必需。</span><span class="sxs-lookup"><span data-stu-id="5d2af-132">Required.</span></span>   |
| <span data-ttu-id="5d2af-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d2af-133">Content-Type</span></span>   | <span data-ttu-id="5d2af-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5d2af-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d2af-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d2af-136">Request body</span></span>
<span data-ttu-id="5d2af-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5d2af-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d2af-138">参数</span><span class="sxs-lookup"><span data-stu-id="5d2af-138">Parameter</span></span>    | <span data-ttu-id="5d2af-139">类型</span><span class="sxs-lookup"><span data-stu-id="5d2af-139">Type</span></span>   |<span data-ttu-id="5d2af-140">说明</span><span class="sxs-lookup"><span data-stu-id="5d2af-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d2af-141">entityType</span><span class="sxs-lookup"><span data-stu-id="5d2af-141">entityType</span></span>|<span data-ttu-id="5d2af-142">String</span><span class="sxs-lookup"><span data-stu-id="5d2af-142">String</span></span>| <span data-ttu-id="5d2af-143">`Group` 是唯一受支持的实体类型。</span><span class="sxs-lookup"><span data-stu-id="5d2af-143">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="5d2af-144">displayName</span><span class="sxs-lookup"><span data-stu-id="5d2af-144">displayName</span></span>|<span data-ttu-id="5d2af-145">String</span><span class="sxs-lookup"><span data-stu-id="5d2af-145">String</span></span>| <span data-ttu-id="5d2af-146">要显示名称组的成员。</span><span class="sxs-lookup"><span data-stu-id="5d2af-146">The display name of the group to validate.</span></span> <span data-ttu-id="5d2af-147">属性不单独是必需的。</span><span class="sxs-lookup"><span data-stu-id="5d2af-147">The property is not individually required.</span></span> <span data-ttu-id="5d2af-148">但是，至少需要一 (displayName 或 mailNickname) 属性。</span><span class="sxs-lookup"><span data-stu-id="5d2af-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="5d2af-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5d2af-149">mailNickname</span></span>|<span data-ttu-id="5d2af-150">String</span><span class="sxs-lookup"><span data-stu-id="5d2af-150">String</span></span>| <span data-ttu-id="5d2af-151">要验证的组的邮件昵称。</span><span class="sxs-lookup"><span data-stu-id="5d2af-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="5d2af-152">属性不单独是必需的。</span><span class="sxs-lookup"><span data-stu-id="5d2af-152">The property is not individually required.</span></span> <span data-ttu-id="5d2af-153">但是，至少需要一 (displayName 或 mailNickname) 属性。</span><span class="sxs-lookup"><span data-stu-id="5d2af-153">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="5d2af-154">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="5d2af-154">onBehalfOfUserId</span></span>|<span data-ttu-id="5d2af-155">Guid</span><span class="sxs-lookup"><span data-stu-id="5d2af-155">Guid</span></span>| <span data-ttu-id="5d2af-156">调用 API 时要模拟的用户的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="5d2af-156">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="5d2af-157">验证结果适用于 onBehalfOfUserId 的属性和角色。</span><span class="sxs-lookup"><span data-stu-id="5d2af-157">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="5d2af-158">响应</span><span class="sxs-lookup"><span data-stu-id="5d2af-158">Response</span></span>

<span data-ttu-id="5d2af-159">如果成功且没有验证错误，该方法将返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5d2af-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="5d2af-160">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5d2af-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="5d2af-161">如果请求无效，该方法将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5d2af-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="5d2af-162">响应正文中返回一条错误消息，包含有关无效请求的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5d2af-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="5d2af-163">如果存在验证错误，该方法将返回 `422 Unprocessable Entity` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5d2af-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="5d2af-164">响应正文中返回一条错误消息和一组错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="5d2af-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d2af-165">示例</span><span class="sxs-lookup"><span data-stu-id="5d2af-165">Examples</span></span>

<span data-ttu-id="5d2af-166">这是一个成功验证请求的示例。</span><span class="sxs-lookup"><span data-stu-id="5d2af-166">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="5d2af-167">请求</span><span class="sxs-lookup"><span data-stu-id="5d2af-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5d2af-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d2af-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="5d2af-169">C#</span><span class="sxs-lookup"><span data-stu-id="5d2af-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d2af-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d2af-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d2af-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d2af-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d2af-172">Java</span><span class="sxs-lookup"><span data-stu-id="5d2af-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d2af-173">响应</span><span class="sxs-lookup"><span data-stu-id="5d2af-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="5d2af-174">这是一个出现验证错误的请求示例。</span><span class="sxs-lookup"><span data-stu-id="5d2af-174">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="5d2af-175">请求</span><span class="sxs-lookup"><span data-stu-id="5d2af-175">Request</span></span>
```http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="5d2af-176">响应</span><span class="sxs-lookup"><span data-stu-id="5d2af-176">Response</span></span>
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


