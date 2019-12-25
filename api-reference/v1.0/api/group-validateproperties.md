---
title: 组： validateProperties
description: 验证 Office 365 组的显示名称或邮件别名是否符合命名策略。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 53705781c8e9465b06199ba3c7714d29a416ee47
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864717"
---
# <a name="group-validateproperties"></a><span data-ttu-id="acf6c-103">组： validateProperties</span><span class="sxs-lookup"><span data-stu-id="acf6c-103">group: validateProperties</span></span>

<span data-ttu-id="acf6c-104">验证 Office 365 组的显示名称或邮件别名是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="acf6c-104">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="acf6c-105">在尝试[更新](group-update.md)Office 365 组之前，客户端可以使用此 API 来确定显示名称或邮件昵称是否有效。</span><span class="sxs-lookup"><span data-stu-id="acf6c-105">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [update](group-update.md) an Office 365 group.</span></span> <span data-ttu-id="acf6c-106">若要在创建组之前验证属性，请使用[directoryobject： validateProperties](directoryobject-validateproperties.md)函数。</span><span class="sxs-lookup"><span data-stu-id="acf6c-106">To validate the properties before creating a group, use the [directoryobject:validateProperties](directoryobject-validateproperties.md) function.</span></span>

<span data-ttu-id="acf6c-107">将为显示名称和邮件昵称属性执行以下策略验证：</span><span class="sxs-lookup"><span data-stu-id="acf6c-107">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="acf6c-108">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="acf6c-108">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="acf6c-109">验证 "自定义禁止的词语" 策略</span><span class="sxs-lookup"><span data-stu-id="acf6c-109">Validate the custom banned words policy</span></span>

<span data-ttu-id="acf6c-110">此 API 仅返回遇到的第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="acf6c-110">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="acf6c-111">如果属性失败多次验证，则仅返回第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="acf6c-111">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="acf6c-112">但是，如果仅验证前缀和后缀命名策略，则可以验证邮件别名和显示名称，并接收验证错误的集合。</span><span class="sxs-lookup"><span data-stu-id="acf6c-112">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="acf6c-113">若要了解有关配置命名策略的详细信息，请参阅[Configure 命名策略](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)。</span><span class="sxs-lookup"><span data-stu-id="acf6c-113">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="acf6c-114">权限</span><span class="sxs-lookup"><span data-stu-id="acf6c-114">Permissions</span></span>

<span data-ttu-id="acf6c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="acf6c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acf6c-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="acf6c-117">Permission type</span></span>      | <span data-ttu-id="acf6c-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="acf6c-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acf6c-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acf6c-119">Delegated (work or school account)</span></span> | <span data-ttu-id="acf6c-120">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acf6c-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="acf6c-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="acf6c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acf6c-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="acf6c-122">Not supported.</span></span>    |
|<span data-ttu-id="acf6c-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="acf6c-123">Application</span></span> | <span data-ttu-id="acf6c-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acf6c-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acf6c-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acf6c-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="acf6c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="acf6c-126">Request headers</span></span>

| <span data-ttu-id="acf6c-127">名称</span><span class="sxs-lookup"><span data-stu-id="acf6c-127">Name</span></span>           | <span data-ttu-id="acf6c-128">说明</span><span class="sxs-lookup"><span data-stu-id="acf6c-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="acf6c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="acf6c-129">Authorization</span></span>  | <span data-ttu-id="acf6c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="acf6c-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="acf6c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="acf6c-132">Content-Type</span></span>   | <span data-ttu-id="acf6c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="acf6c-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="acf6c-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="acf6c-134">Request body</span></span>

<span data-ttu-id="acf6c-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="acf6c-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="acf6c-136">参数</span><span class="sxs-lookup"><span data-stu-id="acf6c-136">Parameter</span></span>    | <span data-ttu-id="acf6c-137">类型</span><span class="sxs-lookup"><span data-stu-id="acf6c-137">Type</span></span>   |<span data-ttu-id="acf6c-138">说明</span><span class="sxs-lookup"><span data-stu-id="acf6c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acf6c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="acf6c-139">displayName</span></span>|<span data-ttu-id="acf6c-140">String</span><span class="sxs-lookup"><span data-stu-id="acf6c-140">String</span></span>| <span data-ttu-id="acf6c-141">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="acf6c-141">The display name of the group to validate.</span></span> <span data-ttu-id="acf6c-142">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="acf6c-142">The property is not individually required.</span></span> <span data-ttu-id="acf6c-143">但是，至少需要一个属性（**displayName**或**mailNickname**）。</span><span class="sxs-lookup"><span data-stu-id="acf6c-143">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="acf6c-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="acf6c-144">mailNickname</span></span>|<span data-ttu-id="acf6c-145">String</span><span class="sxs-lookup"><span data-stu-id="acf6c-145">String</span></span>| <span data-ttu-id="acf6c-146">要验证的组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="acf6c-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="acf6c-147">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="acf6c-147">The property is not individually required.</span></span> <span data-ttu-id="acf6c-148">但是，至少需要一个属性（**displayName**或**mailNickname**）。</span><span class="sxs-lookup"><span data-stu-id="acf6c-148">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="acf6c-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="acf6c-149">onBehalfOfUserId</span></span>|<span data-ttu-id="acf6c-150">Guid</span><span class="sxs-lookup"><span data-stu-id="acf6c-150">Guid</span></span>| <span data-ttu-id="acf6c-151">调用 API 时要模拟的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="acf6c-151">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="acf6c-152">验证结果针对的是**onBehalfOfUserId 的**属性和角色。</span><span class="sxs-lookup"><span data-stu-id="acf6c-152">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="acf6c-153">响应</span><span class="sxs-lookup"><span data-stu-id="acf6c-153">Response</span></span>
<span data-ttu-id="acf6c-154">如果成功且没有验证错误，则该方法返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="acf6c-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="acf6c-155">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="acf6c-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="acf6c-156">如果请求无效，该方法将返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="acf6c-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="acf6c-157">有关无效请求的详细信息的错误消息将在响应正文中返回。</span><span class="sxs-lookup"><span data-stu-id="acf6c-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="acf6c-158">如果存在验证错误。</span><span class="sxs-lookup"><span data-stu-id="acf6c-158">If there is a validation error.</span></span> <span data-ttu-id="acf6c-159">此方法返回`422 Unprocessable Entity`响应代码。</span><span class="sxs-lookup"><span data-stu-id="acf6c-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="acf6c-160">响应正文中返回一条错误消息和一组错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="acf6c-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="acf6c-161">示例</span><span class="sxs-lookup"><span data-stu-id="acf6c-161">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="acf6c-162">示例1：成功的验证请求</span><span class="sxs-lookup"><span data-stu-id="acf6c-162">Example 1: Successful validation request</span></span>
<span data-ttu-id="acf6c-163">这是一个成功的验证请求的示例。</span><span class="sxs-lookup"><span data-stu-id="acf6c-163">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="acf6c-164">请求</span><span class="sxs-lookup"><span data-stu-id="acf6c-164">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="acf6c-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="acf6c-165">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="acf6c-166">C#</span><span class="sxs-lookup"><span data-stu-id="acf6c-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="acf6c-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acf6c-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="acf6c-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acf6c-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="acf6c-169">Java</span><span class="sxs-lookup"><span data-stu-id="acf6c-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="acf6c-170">响应</span><span class="sxs-lookup"><span data-stu-id="acf6c-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="acf6c-171">示例2：包含验证错误的请求</span><span class="sxs-lookup"><span data-stu-id="acf6c-171">Example 2: Request with validation errors</span></span>
<span data-ttu-id="acf6c-172">这是包含验证错误的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="acf6c-172">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="acf6c-173">请求</span><span class="sxs-lookup"><span data-stu-id="acf6c-173">Request</span></span>
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a><span data-ttu-id="acf6c-174">响应</span><span class="sxs-lookup"><span data-stu-id="acf6c-174">Response</span></span>
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
