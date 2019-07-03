---
title: 'directoryObject: validateProperties'
description: 验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。  在尝试**创建**Office 365 组之前, 客户端可以使用 API 来确定显示名称或邮件昵称是否有效。 若要验证现有组的属性, 请使用组的 validateProperties 函数。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3b9d8b5211628e017da2ecc35aaea5b28d77b3d5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436982"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="3c2dc-105">directoryObject: validateProperties</span><span class="sxs-lookup"><span data-stu-id="3c2dc-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="3c2dc-106">验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="3c2dc-107">在尝试**创建**Office 365 组之前, 客户端可以使用 API 来确定显示名称或邮件昵称是否有效。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="3c2dc-108">若要验证现有组的属性, 请使用组的[validateProperties 函数](group-validateproperties.md)。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-108">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="3c2dc-109">将为显示名称和邮件昵称属性执行以下验证:</span><span class="sxs-lookup"><span data-stu-id="3c2dc-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="3c2dc-110">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="3c2dc-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="3c2dc-111">验证 "自定义禁止的词语" 策略</span><span class="sxs-lookup"><span data-stu-id="3c2dc-111">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="3c2dc-112">验证邮件昵称是否唯一</span><span class="sxs-lookup"><span data-stu-id="3c2dc-112">Validate the mail nickname is unique</span></span>

<span data-ttu-id="3c2dc-113">此 API 在遇到第一次失败时返回。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="3c2dc-114">如果一个或多个属性失败多次验证, 则仅返回第一个验证失败的属性。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="3c2dc-115">但是, 如果仅验证前缀和后缀命名策略, 则可以验证邮件别名和显示名称, 并接收验证错误的集合。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c2dc-116">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c2dc-116">Prerequisites</span></span>

<span data-ttu-id="3c2dc-117">若要执行此 API, 需要以下**权限**: *Group. All*</span><span class="sxs-lookup"><span data-stu-id="3c2dc-117">The following **permission** is required to execute this API: *Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="3c2dc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c2dc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="3c2dc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c2dc-119">Request headers</span></span>

| <span data-ttu-id="3c2dc-120">名称</span><span class="sxs-lookup"><span data-stu-id="3c2dc-120">Name</span></span>           | <span data-ttu-id="3c2dc-121">说明</span><span class="sxs-lookup"><span data-stu-id="3c2dc-121">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="3c2dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c2dc-122">Authorization</span></span>  | <span data-ttu-id="3c2dc-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3c2dc-123">Bearer {code}</span></span>    |
| <span data-ttu-id="3c2dc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c2dc-124">Content-Type</span></span>   | <span data-ttu-id="3c2dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c2dc-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c2dc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c2dc-126">Request body</span></span>
<span data-ttu-id="3c2dc-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3c2dc-128">参数</span><span class="sxs-lookup"><span data-stu-id="3c2dc-128">Parameter</span></span>    | <span data-ttu-id="3c2dc-129">类型</span><span class="sxs-lookup"><span data-stu-id="3c2dc-129">Type</span></span>   |<span data-ttu-id="3c2dc-130">说明</span><span class="sxs-lookup"><span data-stu-id="3c2dc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c2dc-131">entityType</span><span class="sxs-lookup"><span data-stu-id="3c2dc-131">entityType</span></span>|<span data-ttu-id="3c2dc-132">String</span><span class="sxs-lookup"><span data-stu-id="3c2dc-132">String</span></span>| <span data-ttu-id="3c2dc-133">`Group`是唯一受支持的实体类型。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-133">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="3c2dc-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3c2dc-134">displayName</span></span>|<span data-ttu-id="3c2dc-135">String</span><span class="sxs-lookup"><span data-stu-id="3c2dc-135">String</span></span>| <span data-ttu-id="3c2dc-136">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-136">The display name of the group to validate.</span></span> <span data-ttu-id="3c2dc-137">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-137">The property is not individually required.</span></span> <span data-ttu-id="3c2dc-138">但是, 至少需要一个属性 (displayName 或 mailNickname)。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-138">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="3c2dc-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3c2dc-139">mailNickname</span></span>|<span data-ttu-id="3c2dc-140">String</span><span class="sxs-lookup"><span data-stu-id="3c2dc-140">String</span></span>| <span data-ttu-id="3c2dc-141">要验证的组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-141">The mail nickname of the group to validate.</span></span> <span data-ttu-id="3c2dc-142">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-142">The property is not individually required.</span></span> <span data-ttu-id="3c2dc-143">但是, 至少需要一个属性 (displayName 或 mailNickname)。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="3c2dc-144">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="3c2dc-144">onBehalfOfUserId</span></span>|<span data-ttu-id="3c2dc-145">Guid</span><span class="sxs-lookup"><span data-stu-id="3c2dc-145">Guid</span></span>| <span data-ttu-id="3c2dc-146">调用 API 时要模拟的用户的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-146">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="3c2dc-147">验证结果针对的是 onBehalfOfUserId 的属性和角色。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-147">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="3c2dc-148">响应</span><span class="sxs-lookup"><span data-stu-id="3c2dc-148">Response</span></span>

<span data-ttu-id="3c2dc-149">如果成功且没有验证错误, 则该方法返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-149">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="3c2dc-150">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-150">It does not return anything in the response body.</span></span>

<span data-ttu-id="3c2dc-151">如果请求无效, 该方法将返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-151">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="3c2dc-152">有关无效请求的详细信息的错误消息将在响应正文中返回。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-152">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="3c2dc-153">如果存在验证错误, 该方法将返回`422 Unprocessable Entity`响应代码。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-153">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="3c2dc-154">响应正文中返回一条错误消息和一组错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-154">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c2dc-155">示例</span><span class="sxs-lookup"><span data-stu-id="3c2dc-155">Examples</span></span>

<span data-ttu-id="3c2dc-156">这是一个成功的验证请求的示例。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-156">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="3c2dc-157">请求</span><span class="sxs-lookup"><span data-stu-id="3c2dc-157">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3c2dc-158">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3c2dc-158">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c2dc-159">C#</span><span class="sxs-lookup"><span data-stu-id="3c2dc-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c2dc-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="3c2dc-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c2dc-161">目标-C</span><span class="sxs-lookup"><span data-stu-id="3c2dc-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c2dc-162">响应</span><span class="sxs-lookup"><span data-stu-id="3c2dc-162">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="3c2dc-163">这是包含验证错误的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="3c2dc-163">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="3c2dc-164">请求</span><span class="sxs-lookup"><span data-stu-id="3c2dc-164">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="3c2dc-165">响应</span><span class="sxs-lookup"><span data-stu-id="3c2dc-165">Response</span></span>
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
