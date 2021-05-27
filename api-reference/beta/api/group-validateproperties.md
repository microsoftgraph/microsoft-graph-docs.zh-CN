---
title: group： validateProperties
description: 验证组Microsoft 365或邮件昵显示名称是否符合命名策略。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6f41ee4f9ae52133d3c7611b52b42997480dfc40
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681219"
---
# <a name="group-validateproperties"></a><span data-ttu-id="5f279-103">group： validateProperties</span><span class="sxs-lookup"><span data-stu-id="5f279-103">group: validateProperties</span></span>

<span data-ttu-id="5f279-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f279-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f279-105">验证组Microsoft 365或邮件昵显示名称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="5f279-105">Validate if a Microsoft 365 group's display name or mail nickname complies with naming policies.</span></span> <span data-ttu-id="5f279-106">客户端可以使用 API 确定显示名称或邮件昵称是否有效，然后再尝试更新Microsoft 365组。 </span><span class="sxs-lookup"><span data-stu-id="5f279-106">Clients can use the API to determine if a display name or mail nickname is valid before trying to **update** a Microsoft 365 group.</span></span> <span data-ttu-id="5f279-107">若要在创建组之前验证属性，请使用目录对象的 [validateProperties](directoryobject-validateproperties.md) 函数。</span><span class="sxs-lookup"><span data-stu-id="5f279-107">For validating properties before creating a group, use the [validateProperties function](directoryobject-validateproperties.md) for directory objects.</span></span>

<span data-ttu-id="5f279-108">对别名和邮件昵称显示名称执行以下验证：</span><span class="sxs-lookup"><span data-stu-id="5f279-108">The following validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="5f279-109">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="5f279-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="5f279-110">验证自定义禁止字策略</span><span class="sxs-lookup"><span data-stu-id="5f279-110">Validate the custom banned words policy</span></span>

<span data-ttu-id="5f279-111">此 API 返回遇到的第一个故障。</span><span class="sxs-lookup"><span data-stu-id="5f279-111">This API returns with the first failure encountered.</span></span> <span data-ttu-id="5f279-112">如果一个或多个属性未能通过多次验证，则仅返回第一个验证失败的属性。</span><span class="sxs-lookup"><span data-stu-id="5f279-112">If one or more properties fail multiple validations, only the property with the first validation failure is returned.</span></span> <span data-ttu-id="5f279-113">但是，如果您仅验证前缀和后缀命名策略，您可以验证邮件昵称和显示名称并接收验证错误集合。</span><span class="sxs-lookup"><span data-stu-id="5f279-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f279-114">权限</span><span class="sxs-lookup"><span data-stu-id="5f279-114">Permissions</span></span>

<span data-ttu-id="5f279-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f279-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f279-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f279-117">Permission type</span></span>      | <span data-ttu-id="5f279-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f279-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f279-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f279-119">Delegated (work or school account)</span></span> | <span data-ttu-id="5f279-120">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f279-120">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5f279-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f279-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f279-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f279-122">Not supported.</span></span>    |
|<span data-ttu-id="5f279-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f279-123">Application</span></span> | <span data-ttu-id="5f279-124">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f279-124">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f279-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f279-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="5f279-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f279-126">Request headers</span></span>

| <span data-ttu-id="5f279-127">名称</span><span class="sxs-lookup"><span data-stu-id="5f279-127">Name</span></span>           | <span data-ttu-id="5f279-128">说明</span><span class="sxs-lookup"><span data-stu-id="5f279-128">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="5f279-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f279-129">Authorization</span></span>  | <span data-ttu-id="5f279-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5f279-130">Bearer {code}</span></span>    |
| <span data-ttu-id="5f279-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f279-131">Content-Type</span></span>   | <span data-ttu-id="5f279-132">application/json</span><span class="sxs-lookup"><span data-stu-id="5f279-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f279-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f279-133">Request body</span></span>

<span data-ttu-id="5f279-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5f279-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5f279-135">参数</span><span class="sxs-lookup"><span data-stu-id="5f279-135">Parameter</span></span>    | <span data-ttu-id="5f279-136">类型</span><span class="sxs-lookup"><span data-stu-id="5f279-136">Type</span></span>   |<span data-ttu-id="5f279-137">说明</span><span class="sxs-lookup"><span data-stu-id="5f279-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f279-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5f279-138">displayName</span></span>|<span data-ttu-id="5f279-139">String</span><span class="sxs-lookup"><span data-stu-id="5f279-139">String</span></span>| <span data-ttu-id="5f279-140">要显示名称组的成员。</span><span class="sxs-lookup"><span data-stu-id="5f279-140">The display name of the group to validate.</span></span> <span data-ttu-id="5f279-141">属性不单独是必需的。</span><span class="sxs-lookup"><span data-stu-id="5f279-141">The property is not individually required.</span></span> <span data-ttu-id="5f279-142">但是，至少需要一 (displayName 或 mailNickname) 属性。</span><span class="sxs-lookup"><span data-stu-id="5f279-142">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="5f279-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="5f279-143">mailNickname</span></span>|<span data-ttu-id="5f279-144">String</span><span class="sxs-lookup"><span data-stu-id="5f279-144">String</span></span>| <span data-ttu-id="5f279-145">要验证的组的邮件昵称。</span><span class="sxs-lookup"><span data-stu-id="5f279-145">The mail nickname of the group to validate.</span></span> <span data-ttu-id="5f279-146">属性不单独是必需的。</span><span class="sxs-lookup"><span data-stu-id="5f279-146">The property is not individually required.</span></span> <span data-ttu-id="5f279-147">但是，至少需要一 (displayName 或 mailNickname) 属性。</span><span class="sxs-lookup"><span data-stu-id="5f279-147">However, at least one property (displayName or mailNickname) is required.</span></span> |
|<span data-ttu-id="5f279-148">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="5f279-148">onBehalfOfUserId</span></span>|<span data-ttu-id="5f279-149">Guid</span><span class="sxs-lookup"><span data-stu-id="5f279-149">Guid</span></span>| <span data-ttu-id="5f279-150">调用 API 时要模拟的用户的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="5f279-150">The object ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="5f279-151">验证结果适用于 onBehalfOfUserId 的属性和角色。</span><span class="sxs-lookup"><span data-stu-id="5f279-151">The validation results are for the onBehalfOfUserId's attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="5f279-152">响应</span><span class="sxs-lookup"><span data-stu-id="5f279-152">Response</span></span>
<span data-ttu-id="5f279-153">如果成功且没有验证错误，该方法将返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5f279-153">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="5f279-154">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5f279-154">It does not return anything in the response body.</span></span>

<span data-ttu-id="5f279-155">如果请求无效，该方法将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5f279-155">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="5f279-156">响应正文中返回一条错误消息，包含有关无效请求的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5f279-156">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="5f279-157">如果存在验证错误。</span><span class="sxs-lookup"><span data-stu-id="5f279-157">If there is a validation error.</span></span> <span data-ttu-id="5f279-158">方法返回 `422 Unprocessable Entity` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5f279-158">The method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="5f279-159">响应正文中返回错误消息和错误详细信息集合。</span><span class="sxs-lookup"><span data-stu-id="5f279-159">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f279-160">示例</span><span class="sxs-lookup"><span data-stu-id="5f279-160">Examples</span></span>

<span data-ttu-id="5f279-161">这是成功验证请求的一个示例。</span><span class="sxs-lookup"><span data-stu-id="5f279-161">This is an example of a successful validation request.</span></span>

### <a name="request"></a><span data-ttu-id="5f279-162">请求</span><span class="sxs-lookup"><span data-stu-id="5f279-162">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5f279-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f279-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5f279-164">C#</span><span class="sxs-lookup"><span data-stu-id="5f279-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f279-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f279-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f279-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f279-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f279-167">Java</span><span class="sxs-lookup"><span data-stu-id="5f279-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f279-168">响应</span><span class="sxs-lookup"><span data-stu-id="5f279-168">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="5f279-169">这是一个出现验证错误的请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f279-169">This is an example of a request with validation errors.</span></span>

### <a name="request"></a><span data-ttu-id="5f279-170">请求</span><span class="sxs-lookup"><span data-stu-id="5f279-170">Request</span></span>
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a><span data-ttu-id="5f279-171">响应</span><span class="sxs-lookup"><span data-stu-id="5f279-171">Response</span></span>
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


