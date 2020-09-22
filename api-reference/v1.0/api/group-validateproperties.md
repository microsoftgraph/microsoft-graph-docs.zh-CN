---
title: 组： validateProperties
description: 验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 49d76daed7154eca9764c9ff10a4e148cf62fcff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041937"
---
# <a name="group-validateproperties"></a><span data-ttu-id="1543e-103">组： validateProperties</span><span class="sxs-lookup"><span data-stu-id="1543e-103">group: validateProperties</span></span>

<span data-ttu-id="1543e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1543e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1543e-105">验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="1543e-105">Validate that a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="1543e-106">在尝试 [更新](group-update.md) Microsoft 365 组之前，客户端可以使用此 API 来确定显示名称或邮件昵称是否有效。</span><span class="sxs-lookup"><span data-stu-id="1543e-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [update](group-update.md) a Microsoft 365 group.</span></span> <span data-ttu-id="1543e-107">若要在创建组之前验证属性，请使用 [directoryobject： validateProperties](directoryobject-validateproperties.md) 函数。</span><span class="sxs-lookup"><span data-stu-id="1543e-107">To validate the properties before creating a group, use the [directoryobject:validateProperties](directoryobject-validateproperties.md) function.</span></span>

<span data-ttu-id="1543e-108">将为显示名称和邮件昵称属性执行以下策略验证：</span><span class="sxs-lookup"><span data-stu-id="1543e-108">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="1543e-109">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="1543e-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="1543e-110">验证 "自定义禁止的词语" 策略</span><span class="sxs-lookup"><span data-stu-id="1543e-110">Validate the custom banned words policy</span></span>

<span data-ttu-id="1543e-111">此 API 仅返回遇到的第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="1543e-111">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="1543e-112">如果属性失败多次验证，则仅返回第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="1543e-112">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="1543e-113">但是，如果仅验证前缀和后缀命名策略，则可以验证邮件别名和显示名称，并接收验证错误的集合。</span><span class="sxs-lookup"><span data-stu-id="1543e-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="1543e-114">若要了解有关配置命名策略的详细信息，请参阅 [Configure 命名策略](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)。</span><span class="sxs-lookup"><span data-stu-id="1543e-114">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="1543e-115">权限</span><span class="sxs-lookup"><span data-stu-id="1543e-115">Permissions</span></span>

<span data-ttu-id="1543e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1543e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1543e-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="1543e-118">Permission type</span></span>      | <span data-ttu-id="1543e-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1543e-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1543e-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1543e-120">Delegated (work or school account)</span></span> | <span data-ttu-id="1543e-121">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1543e-121">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1543e-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1543e-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1543e-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="1543e-123">Not supported.</span></span>    |
|<span data-ttu-id="1543e-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="1543e-124">Application</span></span> | <span data-ttu-id="1543e-125">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1543e-125">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1543e-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1543e-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="1543e-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="1543e-127">Request headers</span></span>

| <span data-ttu-id="1543e-128">名称</span><span class="sxs-lookup"><span data-stu-id="1543e-128">Name</span></span>           | <span data-ttu-id="1543e-129">说明</span><span class="sxs-lookup"><span data-stu-id="1543e-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="1543e-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="1543e-130">Authorization</span></span>  | <span data-ttu-id="1543e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1543e-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="1543e-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1543e-133">Content-Type</span></span>   | <span data-ttu-id="1543e-134">application/json</span><span class="sxs-lookup"><span data-stu-id="1543e-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1543e-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="1543e-135">Request body</span></span>

<span data-ttu-id="1543e-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1543e-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1543e-137">参数</span><span class="sxs-lookup"><span data-stu-id="1543e-137">Parameter</span></span>    | <span data-ttu-id="1543e-138">类型</span><span class="sxs-lookup"><span data-stu-id="1543e-138">Type</span></span>   |<span data-ttu-id="1543e-139">说明</span><span class="sxs-lookup"><span data-stu-id="1543e-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1543e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="1543e-140">displayName</span></span>|<span data-ttu-id="1543e-141">String</span><span class="sxs-lookup"><span data-stu-id="1543e-141">String</span></span>| <span data-ttu-id="1543e-142">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1543e-142">The display name of the group to validate.</span></span> <span data-ttu-id="1543e-143">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="1543e-143">The property is not individually required.</span></span> <span data-ttu-id="1543e-144">但是，至少需要一个属性 (**displayName** 或 **mailNickname**) 。</span><span class="sxs-lookup"><span data-stu-id="1543e-144">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="1543e-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1543e-145">mailNickname</span></span>|<span data-ttu-id="1543e-146">String</span><span class="sxs-lookup"><span data-stu-id="1543e-146">String</span></span>| <span data-ttu-id="1543e-147">要验证的组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="1543e-147">The mail nickname of the group to validate.</span></span> <span data-ttu-id="1543e-148">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="1543e-148">The property is not individually required.</span></span> <span data-ttu-id="1543e-149">但是，至少需要一个属性 (**displayName** 或 **mailNickname**) 。</span><span class="sxs-lookup"><span data-stu-id="1543e-149">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="1543e-150">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="1543e-150">onBehalfOfUserId</span></span>|<span data-ttu-id="1543e-151">Guid</span><span class="sxs-lookup"><span data-stu-id="1543e-151">Guid</span></span>| <span data-ttu-id="1543e-152">调用 API 时要模拟的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="1543e-152">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="1543e-153">验证结果针对的是 **onBehalfOfUserId 的** 属性和角色。</span><span class="sxs-lookup"><span data-stu-id="1543e-153">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="1543e-154">响应</span><span class="sxs-lookup"><span data-stu-id="1543e-154">Response</span></span>
<span data-ttu-id="1543e-155">如果成功且没有验证错误，则该方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1543e-155">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="1543e-156">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1543e-156">It does not return anything in the response body.</span></span>

<span data-ttu-id="1543e-157">如果请求无效，该方法将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1543e-157">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="1543e-158">有关无效请求的详细信息的错误消息将在响应正文中返回。</span><span class="sxs-lookup"><span data-stu-id="1543e-158">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="1543e-159">如果存在验证错误。</span><span class="sxs-lookup"><span data-stu-id="1543e-159">If there is a validation error.</span></span> <span data-ttu-id="1543e-160">此方法返回 `422 Unprocessable Entity` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1543e-160">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="1543e-161">响应正文中返回一条错误消息和一组错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="1543e-161">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1543e-162">示例</span><span class="sxs-lookup"><span data-stu-id="1543e-162">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="1543e-163">示例1：成功的验证请求</span><span class="sxs-lookup"><span data-stu-id="1543e-163">Example 1: Successful validation request</span></span>
<span data-ttu-id="1543e-164">这是一个成功的验证请求的示例。</span><span class="sxs-lookup"><span data-stu-id="1543e-164">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="1543e-165">请求</span><span class="sxs-lookup"><span data-stu-id="1543e-165">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1543e-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="1543e-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1543e-167">C#</span><span class="sxs-lookup"><span data-stu-id="1543e-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1543e-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1543e-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1543e-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1543e-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1543e-170">Java</span><span class="sxs-lookup"><span data-stu-id="1543e-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1543e-171">响应</span><span class="sxs-lookup"><span data-stu-id="1543e-171">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="1543e-172">示例2：包含验证错误的请求</span><span class="sxs-lookup"><span data-stu-id="1543e-172">Example 2: Request with validation errors</span></span>
<span data-ttu-id="1543e-173">这是包含验证错误的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="1543e-173">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="1543e-174">请求</span><span class="sxs-lookup"><span data-stu-id="1543e-174">Request</span></span>
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a><span data-ttu-id="1543e-175">响应</span><span class="sxs-lookup"><span data-stu-id="1543e-175">Response</span></span>
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

