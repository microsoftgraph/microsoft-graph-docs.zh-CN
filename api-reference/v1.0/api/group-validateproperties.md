---
title: '组: validateProperties'
description: 验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e2699e50012f92d8a776fcce20c5cd3d87be83d6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373303"
---
# <a name="group-validateproperties"></a><span data-ttu-id="c2984-103">组: validateProperties</span><span class="sxs-lookup"><span data-stu-id="c2984-103">group: validateProperties</span></span>

<span data-ttu-id="c2984-104">验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="c2984-104">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="c2984-105">在尝试[更新](group-update.md)Office 365 组之前, 客户端可以使用此 API 来确定显示名称或邮件昵称是否有效。</span><span class="sxs-lookup"><span data-stu-id="c2984-105">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [update](group-update.md) an Office 365 group.</span></span> <span data-ttu-id="c2984-106">若要在创建组之前验证属性, 请使用[directoryobject: validateProperties](directoryobject-validateproperties.md)函数。</span><span class="sxs-lookup"><span data-stu-id="c2984-106">To validate the properties before creating a group, use the [directoryobject:validateProperties](directoryobject-validateproperties.md) function.</span></span>

<span data-ttu-id="c2984-107">将为显示名称和邮件昵称属性执行以下策略验证:</span><span class="sxs-lookup"><span data-stu-id="c2984-107">The following policy validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="c2984-108">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="c2984-108">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="c2984-109">验证 "自定义禁止的词语" 策略</span><span class="sxs-lookup"><span data-stu-id="c2984-109">Validate the custom banned words policy</span></span>

<span data-ttu-id="c2984-110">此 API 仅返回遇到的第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="c2984-110">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="c2984-111">如果属性失败多次验证, 则仅返回第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="c2984-111">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="c2984-112">但是, 如果仅验证前缀和后缀命名策略, 则可以验证邮件别名和显示名称, 并接收验证错误的集合。</span><span class="sxs-lookup"><span data-stu-id="c2984-112">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="c2984-113">若要了解有关配置命名策略的详细信息, 请参阅[Configure 命名策略](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)。</span><span class="sxs-lookup"><span data-stu-id="c2984-113">To learn more about configuring naming policies, see [Configure naming policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2984-114">权限</span><span class="sxs-lookup"><span data-stu-id="c2984-114">Permissions</span></span>

<span data-ttu-id="c2984-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2984-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2984-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2984-117">Permission type</span></span>      | <span data-ttu-id="c2984-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2984-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2984-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2984-119">Delegated (work or school account)</span></span> | <span data-ttu-id="c2984-120">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2984-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2984-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2984-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2984-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2984-122">Not supported.</span></span>    |
|<span data-ttu-id="c2984-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2984-123">Application</span></span> | <span data-ttu-id="c2984-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2984-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2984-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2984-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="c2984-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2984-126">Request headers</span></span>

| <span data-ttu-id="c2984-127">名称</span><span class="sxs-lookup"><span data-stu-id="c2984-127">Name</span></span>           | <span data-ttu-id="c2984-128">说明</span><span class="sxs-lookup"><span data-stu-id="c2984-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="c2984-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2984-129">Authorization</span></span>  | <span data-ttu-id="c2984-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2984-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="c2984-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c2984-132">Content-Type</span></span>   | <span data-ttu-id="c2984-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c2984-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2984-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2984-134">Request body</span></span>

<span data-ttu-id="c2984-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c2984-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c2984-136">参数</span><span class="sxs-lookup"><span data-stu-id="c2984-136">Parameter</span></span>    | <span data-ttu-id="c2984-137">类型</span><span class="sxs-lookup"><span data-stu-id="c2984-137">Type</span></span>   |<span data-ttu-id="c2984-138">说明</span><span class="sxs-lookup"><span data-stu-id="c2984-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2984-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c2984-139">displayName</span></span>|<span data-ttu-id="c2984-140">String</span><span class="sxs-lookup"><span data-stu-id="c2984-140">String</span></span>| <span data-ttu-id="c2984-141">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c2984-141">The display name of the group to validate.</span></span> <span data-ttu-id="c2984-142">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="c2984-142">The property is not individually required.</span></span> <span data-ttu-id="c2984-143">但是, 至少需要一个属性 (**displayName**或**mailNickname**)。</span><span class="sxs-lookup"><span data-stu-id="c2984-143">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="c2984-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="c2984-144">mailNickname</span></span>|<span data-ttu-id="c2984-145">String</span><span class="sxs-lookup"><span data-stu-id="c2984-145">String</span></span>| <span data-ttu-id="c2984-146">要验证的组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="c2984-146">The mail nickname of the group to validate.</span></span> <span data-ttu-id="c2984-147">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="c2984-147">The property is not individually required.</span></span> <span data-ttu-id="c2984-148">但是, 至少需要一个属性 (**displayName**或**mailNickname**)。</span><span class="sxs-lookup"><span data-stu-id="c2984-148">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="c2984-149">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="c2984-149">onBehalfOfUserId</span></span>|<span data-ttu-id="c2984-150">Guid</span><span class="sxs-lookup"><span data-stu-id="c2984-150">Guid</span></span>| <span data-ttu-id="c2984-151">调用 API 时要模拟的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="c2984-151">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="c2984-152">验证结果针对的是**onBehalfOfUserId 的**属性和角色。</span><span class="sxs-lookup"><span data-stu-id="c2984-152">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="c2984-153">响应</span><span class="sxs-lookup"><span data-stu-id="c2984-153">Response</span></span>
<span data-ttu-id="c2984-154">如果成功且没有验证错误, 则该方法返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="c2984-154">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="c2984-155">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c2984-155">It does not return anything in the response body.</span></span>

<span data-ttu-id="c2984-156">如果请求无效, 该方法将返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="c2984-156">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="c2984-157">有关无效请求的详细信息的错误消息将在响应正文中返回。</span><span class="sxs-lookup"><span data-stu-id="c2984-157">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="c2984-158">如果存在验证错误。</span><span class="sxs-lookup"><span data-stu-id="c2984-158">If there is a validation error.</span></span> <span data-ttu-id="c2984-159">此方法返回`422 Unprocessable Entity`响应代码。</span><span class="sxs-lookup"><span data-stu-id="c2984-159">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="c2984-160">响应正文中返回一条错误消息和一组错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="c2984-160">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2984-161">示例</span><span class="sxs-lookup"><span data-stu-id="c2984-161">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="c2984-162">示例 1: 成功的验证请求</span><span class="sxs-lookup"><span data-stu-id="c2984-162">Example 1: Successful validation request</span></span>
<span data-ttu-id="c2984-163">这是一个成功的验证请求的示例。</span><span class="sxs-lookup"><span data-stu-id="c2984-163">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="c2984-164">请求</span><span class="sxs-lookup"><span data-stu-id="c2984-164">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2984-165">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c2984-165">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2984-166">C#</span><span class="sxs-lookup"><span data-stu-id="c2984-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2984-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2984-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2984-168">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2984-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2984-169">Java</span><span class="sxs-lookup"><span data-stu-id="c2984-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c2984-170">响应</span><span class="sxs-lookup"><span data-stu-id="c2984-170">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="c2984-171">示例 2: 包含验证错误的请求</span><span class="sxs-lookup"><span data-stu-id="c2984-171">Example 2: Request with validation errors</span></span>
<span data-ttu-id="c2984-172">这是包含验证错误的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="c2984-172">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="c2984-173">请求</span><span class="sxs-lookup"><span data-stu-id="c2984-173">Request</span></span>
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a><span data-ttu-id="c2984-174">响应</span><span class="sxs-lookup"><span data-stu-id="c2984-174">Response</span></span>
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
