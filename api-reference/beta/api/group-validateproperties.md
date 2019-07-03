---
title: '组: validateProperties'
description: 验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。 在尝试**更新**Office 365 组之前, 客户端可以使用 API 来确定显示名称或邮件昵称是否有效。 若要在创建组之前验证属性, 请使用目录对象的 validateProperties 函数。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7da24d3a28c8640f231b9d94c295e6a16abe040b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442669"
---
# <a name="group-validateproperties"></a><span data-ttu-id="57165-105">组: validateProperties</span><span class="sxs-lookup"><span data-stu-id="57165-105">group: validateProperties</span></span>

<span data-ttu-id="57165-106">验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="57165-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="57165-107">在尝试**更新**Office 365 组之前, 客户端可以使用 API 来确定显示名称或邮件昵称是否有效。</span><span class="sxs-lookup"><span data-stu-id="57165-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="57165-108">若要在创建组之前验证属性, 请使用目录对象的[validateProperties 函数](directoryobject-validateproperties.md)。</span><span class="sxs-lookup"><span data-stu-id="57165-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="57165-109">将为显示名称和邮件昵称属性执行以下验证:</span><span class="sxs-lookup"><span data-stu-id="57165-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="57165-110">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="57165-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="57165-111">验证 "自定义禁止的词语" 策略</span><span class="sxs-lookup"><span data-stu-id="57165-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="57165-112">此 API 在遇到第一次失败时返回。</span><span class="sxs-lookup"><span data-stu-id="57165-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="57165-113">如果一个或多个属性失败多次验证, 则仅返回第一个验证失败的属性。</span><span class="sxs-lookup"><span data-stu-id="57165-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="57165-114">但是, 如果仅验证前缀和后缀命名策略, 则可以验证邮件别名和显示名称, 并接收验证错误的集合。</span><span class="sxs-lookup"><span data-stu-id="57165-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="57165-115">权限</span><span class="sxs-lookup"><span data-stu-id="57165-115">Permissions</span></span>

<span data-ttu-id="57165-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57165-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57165-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="57165-118">Permission type</span></span>      | <span data-ttu-id="57165-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57165-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57165-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57165-120">Delegated (work or school account)</span></span> | <span data-ttu-id="57165-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57165-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="57165-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57165-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57165-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="57165-123">Not supported.</span></span>    |
|<span data-ttu-id="57165-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="57165-124">Application</span></span> | <span data-ttu-id="57165-125">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57165-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57165-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57165-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="57165-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="57165-127">Request headers</span></span>

| <span data-ttu-id="57165-128">名称</span><span class="sxs-lookup"><span data-stu-id="57165-128">Name</span></span>           | <span data-ttu-id="57165-129">说明</span><span class="sxs-lookup"><span data-stu-id="57165-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="57165-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="57165-130">Authorization</span></span>  | <span data-ttu-id="57165-131">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="57165-131">Bearer {code}</span></span>    |
| <span data-ttu-id="57165-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57165-132">Content-Type</span></span>   | <span data-ttu-id="57165-133">application/json</span><span class="sxs-lookup"><span data-stu-id="57165-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="57165-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="57165-134">Request body</span></span>

<span data-ttu-id="57165-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="57165-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57165-136">参数</span><span class="sxs-lookup"><span data-stu-id="57165-136">Parameter</span></span>    | <span data-ttu-id="57165-137">类型</span><span class="sxs-lookup"><span data-stu-id="57165-137">Type</span></span>   |<span data-ttu-id="57165-138">说明</span><span class="sxs-lookup"><span data-stu-id="57165-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57165-139">displayName</span><span class="sxs-lookup"><span data-stu-id="57165-139">displayName</span></span>|<span data-ttu-id="57165-140">String</span><span class="sxs-lookup"><span data-stu-id="57165-140">String</span></span>| <span data-ttu-id="57165-141">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="57165-141">The display name of the group to validate.</span></span> <span data-ttu-id="57165-142">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="57165-142">The property is not individually required.</span></span> <span data-ttu-id="57165-143">但是, 至少需要一个属性 (displayName 或 mailNickname)。</span><span class="sxs-lookup"><span data-stu-id="57165-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="57165-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="57165-144">mailNickname</span></span>|<span data-ttu-id="57165-145">String</span><span class="sxs-lookup"><span data-stu-id="57165-145">String</span></span>| <span data-ttu-id="57165-146">要验证的组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="57165-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="57165-147">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="57165-147">The property is not individually required.</span></span> <span data-ttu-id="57165-148">但是, 至少需要一个属性 (displayName 或 mailNickname)。</span><span class="sxs-lookup"><span data-stu-id="57165-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="57165-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="57165-149">onBehalfOfUserId</span></span>|<span data-ttu-id="57165-150">Guid</span><span class="sxs-lookup"><span data-stu-id="57165-150">Guid</span></span>| <span data-ttu-id="57165-151">调用 API 时要模拟的用户的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="57165-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="57165-152">验证结果针对的是 onBehalfOfUserId 的属性和角色。</span><span class="sxs-lookup"><span data-stu-id="57165-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="57165-153">响应</span><span class="sxs-lookup"><span data-stu-id="57165-153">Response</span></span>
<span data-ttu-id="57165-154">如果成功且没有验证错误, 则该方法返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="57165-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="57165-155">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="57165-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="57165-156">如果请求无效, 该方法将返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="57165-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="57165-157">有关无效请求的详细信息的错误消息将在响应正文中返回。</span><span class="sxs-lookup"><span data-stu-id="57165-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="57165-158">如果存在验证错误。</span><span class="sxs-lookup"><span data-stu-id="57165-158">If there is a validation error.</span></span> <span data-ttu-id="57165-159">此方法返回`422 Unprocessable Entity`响应代码。</span><span class="sxs-lookup"><span data-stu-id="57165-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="57165-160">响应正文中返回一条错误消息和一组错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="57165-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57165-161">示例</span><span class="sxs-lookup"><span data-stu-id="57165-161">Examples</span></span>

<span data-ttu-id="57165-162">这是一个成功的验证请求的示例。</span><span class="sxs-lookup"><span data-stu-id="57165-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="57165-163">请求</span><span class="sxs-lookup"><span data-stu-id="57165-163">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="57165-164">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="57165-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="57165-165">C#</span><span class="sxs-lookup"><span data-stu-id="57165-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57165-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="57165-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="57165-167">目标-C</span><span class="sxs-lookup"><span data-stu-id="57165-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57165-168">响应</span><span class="sxs-lookup"><span data-stu-id="57165-168">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="57165-169">这是包含验证错误的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="57165-169">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="57165-170">请求</span><span class="sxs-lookup"><span data-stu-id="57165-170">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="57165-171">响应</span><span class="sxs-lookup"><span data-stu-id="57165-171">Response</span></span>
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
