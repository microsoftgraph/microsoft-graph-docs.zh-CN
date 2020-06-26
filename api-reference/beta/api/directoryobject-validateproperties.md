---
title: directoryObject： validateProperties
description: 验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 45178491bb6ae451cb1ee39a182263a3d99ce59f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895746"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="23524-103">directoryObject： validateProperties</span><span class="sxs-lookup"><span data-stu-id="23524-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="23524-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23524-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23524-105">验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="23524-105">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="23524-106">在尝试**创建**Microsoft 365 组之前，客户端可以使用此 API 来确定显示名称或邮件昵称是否有效。</span><span class="sxs-lookup"><span data-stu-id="23524-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to **create** a Microsoft 365 group.</span></span> <span data-ttu-id="23524-107">若要验证现有组的属性，请使用组的[validateProperties 函数](group-validateproperties.md)。</span><span class="sxs-lookup"><span data-stu-id="23524-107">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="23524-108">将为显示名称和邮件昵称属性执行以下验证：</span><span class="sxs-lookup"><span data-stu-id="23524-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="23524-109">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="23524-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="23524-110">验证 "自定义禁止的词语" 策略</span><span class="sxs-lookup"><span data-stu-id="23524-110">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="23524-111">验证邮件昵称是否唯一</span><span class="sxs-lookup"><span data-stu-id="23524-111">Validate the mail nickname is unique</span></span>

<span data-ttu-id="23524-112">此 API 在遇到第一次失败时返回。</span><span class="sxs-lookup"><span data-stu-id="23524-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="23524-113">如果一个或多个属性失败多次验证，则仅返回第一个验证失败的属性。</span><span class="sxs-lookup"><span data-stu-id="23524-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="23524-114">但是，如果仅验证前缀和后缀命名策略，则可以验证邮件别名和显示名称，并接收验证错误的集合。</span><span class="sxs-lookup"><span data-stu-id="23524-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="23524-115">权限</span><span class="sxs-lookup"><span data-stu-id="23524-115">Permissions</span></span>
<span data-ttu-id="23524-116">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="23524-116">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="23524-117">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23524-117">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23524-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="23524-118">Permission type</span></span>      | <span data-ttu-id="23524-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23524-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23524-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23524-120">Delegated (work or school account)</span></span> | <span data-ttu-id="23524-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23524-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="23524-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23524-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23524-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="23524-123">Not supported.</span></span>    |
|<span data-ttu-id="23524-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="23524-124">Application</span></span> | <span data-ttu-id="23524-125">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23524-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23524-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23524-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="23524-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="23524-127">Request headers</span></span>

| <span data-ttu-id="23524-128">名称</span><span class="sxs-lookup"><span data-stu-id="23524-128">Name</span></span>           | <span data-ttu-id="23524-129">说明</span><span class="sxs-lookup"><span data-stu-id="23524-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="23524-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="23524-130">Authorization</span></span>  | <span data-ttu-id="23524-131">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="23524-131">Bearer {code}.</span></span> <span data-ttu-id="23524-132">必需。</span><span class="sxs-lookup"><span data-stu-id="23524-132">Required.</span></span>   |
| <span data-ttu-id="23524-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23524-133">Content-Type</span></span>   | <span data-ttu-id="23524-134">application/json.</span><span class="sxs-lookup"><span data-stu-id="23524-134">application/json.</span></span> <span data-ttu-id="23524-135">Required.</span><span class="sxs-lookup"><span data-stu-id="23524-135">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23524-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="23524-136">Request body</span></span>
<span data-ttu-id="23524-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="23524-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="23524-138">参数</span><span class="sxs-lookup"><span data-stu-id="23524-138">Parameter</span></span>    | <span data-ttu-id="23524-139">类型</span><span class="sxs-lookup"><span data-stu-id="23524-139">Type</span></span>   |<span data-ttu-id="23524-140">说明</span><span class="sxs-lookup"><span data-stu-id="23524-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23524-141">entityType</span><span class="sxs-lookup"><span data-stu-id="23524-141">entityType</span></span>|<span data-ttu-id="23524-142">String</span><span class="sxs-lookup"><span data-stu-id="23524-142">String</span></span>| <span data-ttu-id="23524-143">`Group`是唯一受支持的实体类型。</span><span class="sxs-lookup"><span data-stu-id="23524-143">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="23524-144">displayName</span><span class="sxs-lookup"><span data-stu-id="23524-144">displayName</span></span>|<span data-ttu-id="23524-145">String</span><span class="sxs-lookup"><span data-stu-id="23524-145">String</span></span>| <span data-ttu-id="23524-146">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="23524-146">The display name of the group to validate.</span></span> <span data-ttu-id="23524-147">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="23524-147">The property is not individually required.</span></span> <span data-ttu-id="23524-148">但是，至少需要一个属性（displayName 或 mailNickname）。</span><span class="sxs-lookup"><span data-stu-id="23524-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="23524-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="23524-149">mailNickname</span></span>|<span data-ttu-id="23524-150">String</span><span class="sxs-lookup"><span data-stu-id="23524-150">String</span></span>| <span data-ttu-id="23524-151">要验证的组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="23524-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="23524-152">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="23524-152">The property is not individually required.</span></span> <span data-ttu-id="23524-153">但是，至少需要一个属性（displayName 或 mailNickname）。</span><span class="sxs-lookup"><span data-stu-id="23524-153">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="23524-154">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="23524-154">onBehalfOfUserId</span></span>|<span data-ttu-id="23524-155">Guid</span><span class="sxs-lookup"><span data-stu-id="23524-155">Guid</span></span>| <span data-ttu-id="23524-156">调用 API 时要模拟的用户的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="23524-156">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="23524-157">验证结果针对的是 onBehalfOfUserId 的属性和角色。</span><span class="sxs-lookup"><span data-stu-id="23524-157">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="23524-158">响应</span><span class="sxs-lookup"><span data-stu-id="23524-158">Response</span></span>

<span data-ttu-id="23524-159">如果成功且没有验证错误，则该方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="23524-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="23524-160">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="23524-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="23524-161">如果请求无效，该方法将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="23524-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="23524-162">有关无效请求的详细信息的错误消息将在响应正文中返回。</span><span class="sxs-lookup"><span data-stu-id="23524-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="23524-163">如果存在验证错误，该方法将返回 `422 Unprocessable Entity` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="23524-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="23524-164">响应正文中返回一条错误消息和一组错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="23524-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23524-165">示例</span><span class="sxs-lookup"><span data-stu-id="23524-165">Examples</span></span>

<span data-ttu-id="23524-166">这是一个成功的验证请求的示例。</span><span class="sxs-lookup"><span data-stu-id="23524-166">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="23524-167">请求</span><span class="sxs-lookup"><span data-stu-id="23524-167">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="23524-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="23524-168">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="23524-169">C#</span><span class="sxs-lookup"><span data-stu-id="23524-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23524-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23524-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23524-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23524-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="23524-172">响应</span><span class="sxs-lookup"><span data-stu-id="23524-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="23524-173">这是包含验证错误的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="23524-173">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="23524-174">请求</span><span class="sxs-lookup"><span data-stu-id="23524-174">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="23524-175">响应</span><span class="sxs-lookup"><span data-stu-id="23524-175">Response</span></span>
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
