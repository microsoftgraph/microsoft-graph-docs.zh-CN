---
title: 组： validateProperties
description: 验证如果 Office 365 组的显示名称或邮件昵称符合命名策略。 客户端可以使用 API 以确定是否显示名称或邮件昵称有效，然后尝试**更新**到 Office 365 组。 用于创建组之前验证属性，将 validateProperties 函数用于目录对象。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5361e05d2a58e2d4c27bd662f158d4f185c447fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990886"
---
# <a name="group-validateproperties"></a><span data-ttu-id="c3224-105">组： validateProperties</span><span class="sxs-lookup"><span data-stu-id="c3224-105">group: validateProperties</span></span>

<span data-ttu-id="c3224-106">验证如果 Office 365 组的显示名称或邮件昵称符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="c3224-106">Validate if an Office 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="c3224-107">客户端可以使用 API 以确定是否显示名称或邮件昵称有效，然后尝试**更新**到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="c3224-107">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** an Office 365 group.</span></span> <span data-ttu-id="c3224-108">用于创建组之前验证属性，将[validateProperties 函数](directoryobject-validateproperties.md)用于目录对象。</span><span class="sxs-lookup"><span data-stu-id="c3224-108">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="c3224-109">显示名称和邮件昵称属性执行以下验证：</span><span class="sxs-lookup"><span data-stu-id="c3224-109">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="c3224-110">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="c3224-110">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="c3224-111">验证自定义禁止的单词策略</span><span class="sxs-lookup"><span data-stu-id="c3224-111">Validate the custom banned words policy</span></span>

<span data-ttu-id="c3224-112">此 API 返回与第一个遇到故障。</span><span class="sxs-lookup"><span data-stu-id="c3224-112">This API returns with the first failure encountered.</span></span> <span data-ttu-id="c3224-113">如果一个或多个属性失败多个验证，则返回仅与第一个验证失败的属性。</span><span class="sxs-lookup"><span data-stu-id="c3224-113">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="c3224-114">但是，您可以验证邮件昵称和显示名称和接收验证错误的集合，如果您仅验证前缀和后缀命名策略。</span><span class="sxs-lookup"><span data-stu-id="c3224-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3224-115">权限</span><span class="sxs-lookup"><span data-stu-id="c3224-115">Permissions</span></span>

<span data-ttu-id="c3224-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3224-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3224-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3224-118">Permission type</span></span>      | <span data-ttu-id="c3224-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3224-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3224-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3224-120">Delegated (work or school account)</span></span> | <span data-ttu-id="c3224-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3224-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3224-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3224-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3224-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3224-123">Not supported.</span></span>    |
|<span data-ttu-id="c3224-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3224-124">Application</span></span> | <span data-ttu-id="c3224-125">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3224-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3224-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3224-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="c3224-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3224-127">Request headers</span></span>

| <span data-ttu-id="c3224-128">名称</span><span class="sxs-lookup"><span data-stu-id="c3224-128">Name</span></span>           | <span data-ttu-id="c3224-129">说明</span><span class="sxs-lookup"><span data-stu-id="c3224-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="c3224-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3224-130">Authorization</span></span>  | <span data-ttu-id="c3224-131">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="c3224-131">Bearer {code}</span></span>    |
| <span data-ttu-id="c3224-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3224-132">Content-Type</span></span>   | <span data-ttu-id="c3224-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c3224-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3224-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3224-134">Request body</span></span>

<span data-ttu-id="c3224-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c3224-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c3224-136">参数</span><span class="sxs-lookup"><span data-stu-id="c3224-136">Parameter</span></span>    | <span data-ttu-id="c3224-137">类型</span><span class="sxs-lookup"><span data-stu-id="c3224-137">Type</span></span>   |<span data-ttu-id="c3224-138">说明</span><span class="sxs-lookup"><span data-stu-id="c3224-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3224-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c3224-139">displayName</span></span>|<span data-ttu-id="c3224-140">字符串</span><span class="sxs-lookup"><span data-stu-id="c3224-140">String</span></span>| <span data-ttu-id="c3224-141">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c3224-141">The display name of the group to validate.</span></span> <span data-ttu-id="c3224-142">该属性不是单独必需的。</span><span class="sxs-lookup"><span data-stu-id="c3224-142">The property is not individually required.</span></span> <span data-ttu-id="c3224-143">但是，至少一个属性 （displayName 或 mailNickname） 是必需的。</span><span class="sxs-lookup"><span data-stu-id="c3224-143">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="c3224-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c3224-144">mailNickname</span></span>|<span data-ttu-id="c3224-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c3224-145">String</span></span>| <span data-ttu-id="c3224-146">要验证的组邮件昵称。</span><span class="sxs-lookup"><span data-stu-id="c3224-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="c3224-147">该属性不是单独必需的。</span><span class="sxs-lookup"><span data-stu-id="c3224-147">The property is not individually required.</span></span> <span data-ttu-id="c3224-148">但是，至少一个属性 （displayName 或 mailNickname） 是必需的。</span><span class="sxs-lookup"><span data-stu-id="c3224-148">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="c3224-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="c3224-149">onBehalfOfUserId</span></span>|<span data-ttu-id="c3224-150">Guid</span><span class="sxs-lookup"><span data-stu-id="c3224-150">Guid</span></span>| <span data-ttu-id="c3224-151">调用 API 时模拟用户对象 ID。</span><span class="sxs-lookup"><span data-stu-id="c3224-151">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="c3224-152">验证结果是针对 onBehalfOfUserId 的属性和角色。</span><span class="sxs-lookup"><span data-stu-id="c3224-152">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="c3224-153">响应</span><span class="sxs-lookup"><span data-stu-id="c3224-153">Response</span></span>
<span data-ttu-id="c3224-154">如果成功，并有没有验证错误，该方法返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="c3224-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="c3224-155">它不返回任何响应正文中。</span><span class="sxs-lookup"><span data-stu-id="c3224-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="c3224-156">如果请求无效，则该方法返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="c3224-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="c3224-157">响应正文中返回有关无效请求的详细错误消息。</span><span class="sxs-lookup"><span data-stu-id="c3224-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="c3224-158">如果没有验证错误。</span><span class="sxs-lookup"><span data-stu-id="c3224-158">If there is a validation error.</span></span> <span data-ttu-id="c3224-159">该方法返回`422 Unprocessable Entity`响应代码。</span><span class="sxs-lookup"><span data-stu-id="c3224-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="c3224-160">在响应正文中将返回一条错误消息和错误详细信息的集合。</span><span class="sxs-lookup"><span data-stu-id="c3224-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3224-161">示例</span><span class="sxs-lookup"><span data-stu-id="c3224-161">Examples</span></span>

<span data-ttu-id="c3224-162">这是一个成功验证请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3224-162">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="c3224-163">请求</span><span class="sxs-lookup"><span data-stu-id="c3224-163">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="c3224-164">响应</span><span class="sxs-lookup"><span data-stu-id="c3224-164">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="c3224-165">这是一个带有验证错误的请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3224-165">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="c3224-166">请求</span><span class="sxs-lookup"><span data-stu-id="c3224-166">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="c3224-167">响应</span><span class="sxs-lookup"><span data-stu-id="c3224-167">Response</span></span>
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
  "tocPath": ""
}-->
