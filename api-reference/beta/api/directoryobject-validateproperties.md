---
title: 'directoryObject: validateProperties'
description: 验证如果 Office 365 组的显示名称或邮件昵称符合命名策略。  客户端可以使用 API 以确定是否显示名称或邮件昵称有效，然后尝试**创建**到 Office 365 组。 用于验证的现有组属性，使用组 validateProperties 函数。
localization_priority: Normal
ms.openlocfilehash: 1f38a30d86cf5b28eea6b9891687c4dbca4b78fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879819"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="6bcd8-105">directoryObject: validateProperties</span><span class="sxs-lookup"><span data-stu-id="6bcd8-105">directoryObject: validateProperties</span></span>

<span data-ttu-id="6bcd8-106">验证如果 Office 365 组的显示名称或邮件昵称符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="6bcd8-107">客户端可以使用 API 以确定是否显示名称或邮件昵称有效，然后尝试**创建**到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **create** an Office 365 group.</span></span> <span data-ttu-id="6bcd8-108">用于验证的现有组属性，使用组[validateProperties 函数](group-validateproperties.md)。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-108">For validating properties of an existing group, use the [validateProperties function](group-validateproperties.md) for groups.</span></span>

<span data-ttu-id="6bcd8-109">显示名称和邮件昵称属性执行以下验证：</span><span class="sxs-lookup"><span data-stu-id="6bcd8-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="6bcd8-110">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="6bcd8-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="6bcd8-111">验证自定义禁止的单词策略</span><span class="sxs-lookup"><span data-stu-id="6bcd8-111">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="6bcd8-112">验证邮件昵称是唯一</span><span class="sxs-lookup"><span data-stu-id="6bcd8-112">Validate the mail nickname is unique</span></span>

<span data-ttu-id="6bcd8-113">此 API 返回与第一个遇到故障。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-113">This API returns with the first failure encountered.</span></span> <span data-ttu-id="6bcd8-114">如果一个或多个属性失败多个验证，则返回仅与第一个验证失败的属性。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-114">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="6bcd8-115">但是，您可以验证邮件昵称和显示名称和接收验证错误的集合，如果您仅验证前缀和后缀命名策略。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-115">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bcd8-116">必要条件</span><span class="sxs-lookup"><span data-stu-id="6bcd8-116">Prerequisites</span></span>

<span data-ttu-id="6bcd8-117">执行此 API 所需的以下**权限**： *Group.Read.All*</span><span class="sxs-lookup"><span data-stu-id="6bcd8-117">The following **permission** is required to execute this API: *Group.Read.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="6bcd8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6bcd8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="6bcd8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6bcd8-119">Request headers</span></span>

| <span data-ttu-id="6bcd8-120">名称</span><span class="sxs-lookup"><span data-stu-id="6bcd8-120">Name</span></span>           | <span data-ttu-id="6bcd8-121">说明</span><span class="sxs-lookup"><span data-stu-id="6bcd8-121">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="6bcd8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bcd8-122">Authorization</span></span>  | <span data-ttu-id="6bcd8-123">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="6bcd8-123">Bearer {code}</span></span>    |
| <span data-ttu-id="6bcd8-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6bcd8-124">Content-Type</span></span>   | <span data-ttu-id="6bcd8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6bcd8-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6bcd8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6bcd8-126">Request body</span></span>
<span data-ttu-id="6bcd8-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6bcd8-128">参数</span><span class="sxs-lookup"><span data-stu-id="6bcd8-128">Parameter</span></span>    | <span data-ttu-id="6bcd8-129">类型</span><span class="sxs-lookup"><span data-stu-id="6bcd8-129">Type</span></span>   |<span data-ttu-id="6bcd8-130">Description</span><span class="sxs-lookup"><span data-stu-id="6bcd8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bcd8-131">entityType</span><span class="sxs-lookup"><span data-stu-id="6bcd8-131">entityType</span></span>|<span data-ttu-id="6bcd8-132">字符串</span><span class="sxs-lookup"><span data-stu-id="6bcd8-132">String</span></span>| <span data-ttu-id="6bcd8-133">`Group`是唯一受支持的实体类型。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-133">`Group` is the only supported entity type.</span></span> |
|<span data-ttu-id="6bcd8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6bcd8-134">displayName</span></span>|<span data-ttu-id="6bcd8-135">字符串</span><span class="sxs-lookup"><span data-stu-id="6bcd8-135">String</span></span>| <span data-ttu-id="6bcd8-136">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-136">The display name of the group to validate.</span></span> <span data-ttu-id="6bcd8-137">该属性不是单独必需的。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-137">The property is not individually required.</span></span> <span data-ttu-id="6bcd8-138">但是，至少一个属性 （displayName 或 mailNickname） 是必需的。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-138">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="6bcd8-139">mailNickname</span><span class="sxs-lookup"><span data-stu-id="6bcd8-139">mailNickname</span></span>|<span data-ttu-id="6bcd8-140">字符串</span><span class="sxs-lookup"><span data-stu-id="6bcd8-140">String</span></span>| <span data-ttu-id="6bcd8-141">要验证的组邮件昵称。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-141">The mail nickname of the group to validate.</span></span> <span data-ttu-id="6bcd8-142">该属性不是单独必需的。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-142">The property is not individually required.</span></span> <span data-ttu-id="6bcd8-143">但是，至少一个属性 （displayName 或 mailNickname） 是必需的。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="6bcd8-144">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="6bcd8-144">onBehalfOfUserId</span></span>|<span data-ttu-id="6bcd8-145">Guid</span><span class="sxs-lookup"><span data-stu-id="6bcd8-145">Guid</span></span>| <span data-ttu-id="6bcd8-146">调用 API 时模拟用户对象 ID。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-146">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="6bcd8-147">验证结果是针对 onBehalfOfUserId 的属性和角色。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-147">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="6bcd8-148">响应</span><span class="sxs-lookup"><span data-stu-id="6bcd8-148">Response</span></span>

<span data-ttu-id="6bcd8-149">如果成功，并有没有验证错误，该方法返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-149">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="6bcd8-150">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-150">It does not return anything in the response body.</span></span>

<span data-ttu-id="6bcd8-151">如果请求无效，则该方法返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-151">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="6bcd8-152">响应正文中返回有关无效请求的详细错误消息。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-152">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="6bcd8-153">如果验证错误，则该方法返回`422 Unprocessable Entity`响应代码。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-153">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="6bcd8-154">在响应正文中将返回一条错误消息和错误详细信息的集合。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-154">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6bcd8-155">示例</span><span class="sxs-lookup"><span data-stu-id="6bcd8-155">Examples</span></span>

<span data-ttu-id="6bcd8-156">这是一个成功验证请求示例。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-156">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="6bcd8-157">请求</span><span class="sxs-lookup"><span data-stu-id="6bcd8-157">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="6bcd8-158">响应</span><span class="sxs-lookup"><span data-stu-id="6bcd8-158">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="6bcd8-159">这是一个带有验证错误的请求示例。</span><span class="sxs-lookup"><span data-stu-id="6bcd8-159">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="6bcd8-160">请求</span><span class="sxs-lookup"><span data-stu-id="6bcd8-160">Request</span></span>
```http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a><span data-ttu-id="6bcd8-161">响应</span><span class="sxs-lookup"><span data-stu-id="6bcd8-161">Response</span></span>
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
  "tocPath": ""
}-->
