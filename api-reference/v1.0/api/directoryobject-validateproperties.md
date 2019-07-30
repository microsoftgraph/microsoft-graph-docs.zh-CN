---
title: 'directoryObject: validateProperties'
description: 验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f26857514ec180dbbc50c73eeb8eccc4b30185ed
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932200"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="1223f-103">directoryObject: validateProperties</span><span class="sxs-lookup"><span data-stu-id="1223f-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="1223f-104">验证 Office 365 组的显示名称或邮件昵称是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="1223f-104">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="1223f-105">在尝试[创建](group-post-groups.md)Office 365 组之前, 客户端可以使用此 API 来确定显示名称或邮件昵称是否有效。</span><span class="sxs-lookup"><span data-stu-id="1223f-105">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [create](group-post-groups.md) an Office 365 group.</span></span> <span data-ttu-id="1223f-106">若要验证现有组的属性, 请使用[group: validateProperties](group-validateproperties.md)函数。</span><span class="sxs-lookup"><span data-stu-id="1223f-106">To validate the properties of an existing group, use the [group: validateProperties](group-validateproperties.md) function.</span></span>

<span data-ttu-id="1223f-107">将为显示名称和邮件昵称属性执行以下策略验证:</span><span class="sxs-lookup"><span data-stu-id="1223f-107">The following policy validations are performed for the display name and mail nickname properties:</span></span> 
1. <span data-ttu-id="1223f-108">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="1223f-108">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="1223f-109">验证 "自定义禁止的词语" 策略</span><span class="sxs-lookup"><span data-stu-id="1223f-109">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="1223f-110">验证邮件昵称是否唯一</span><span class="sxs-lookup"><span data-stu-id="1223f-110">Validate that the mail nickname is unique</span></span>

<span data-ttu-id="1223f-111">此 API 仅返回遇到的第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="1223f-111">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="1223f-112">如果属性失败多次验证, 则仅返回第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="1223f-112">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="1223f-113">但是, 如果仅验证前缀和后缀命名策略, 则可以验证邮件别名和显示名称, 并接收验证错误的集合。</span><span class="sxs-lookup"><span data-stu-id="1223f-113">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="1223f-114">若要了解有关配置命名策略的详细信息, 请参阅[Configure 命名策略](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)。</span><span class="sxs-lookup"><span data-stu-id="1223f-114">To learn more about configuring naming policies, see [Configure naming policy](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="1223f-115">权限</span><span class="sxs-lookup"><span data-stu-id="1223f-115">Permissions</span></span>
<span data-ttu-id="1223f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1223f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1223f-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="1223f-118">Permission type</span></span>      | <span data-ttu-id="1223f-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1223f-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1223f-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1223f-120">Delegated (work or school account)</span></span> | <span data-ttu-id="1223f-121">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1223f-121">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1223f-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1223f-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1223f-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="1223f-123">Not supported.</span></span>    |
|<span data-ttu-id="1223f-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="1223f-124">Application</span></span> | <span data-ttu-id="1223f-125">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1223f-125">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1223f-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1223f-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="1223f-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="1223f-127">Request headers</span></span>

| <span data-ttu-id="1223f-128">名称</span><span class="sxs-lookup"><span data-stu-id="1223f-128">Name</span></span>           | <span data-ttu-id="1223f-129">说明</span><span class="sxs-lookup"><span data-stu-id="1223f-129">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="1223f-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="1223f-130">Authorization</span></span>  | <span data-ttu-id="1223f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1223f-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="1223f-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1223f-133">Content-Type</span></span>   | <span data-ttu-id="1223f-134">application/json</span><span class="sxs-lookup"><span data-stu-id="1223f-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1223f-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="1223f-135">Request body</span></span>
<span data-ttu-id="1223f-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1223f-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1223f-137">参数</span><span class="sxs-lookup"><span data-stu-id="1223f-137">Parameter</span></span>    | <span data-ttu-id="1223f-138">类型</span><span class="sxs-lookup"><span data-stu-id="1223f-138">Type</span></span>   |<span data-ttu-id="1223f-139">说明</span><span class="sxs-lookup"><span data-stu-id="1223f-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1223f-140">entityType</span><span class="sxs-lookup"><span data-stu-id="1223f-140">entityType</span></span>|<span data-ttu-id="1223f-141">String</span><span class="sxs-lookup"><span data-stu-id="1223f-141">String</span></span>| <span data-ttu-id="1223f-142">Group 是唯一受支持的实体类型。</span><span class="sxs-lookup"><span data-stu-id="1223f-142">Group is the only supported entity type.</span></span> |
|<span data-ttu-id="1223f-143">displayName</span><span class="sxs-lookup"><span data-stu-id="1223f-143">displayName</span></span>|<span data-ttu-id="1223f-144">String</span><span class="sxs-lookup"><span data-stu-id="1223f-144">String</span></span>| <span data-ttu-id="1223f-145">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1223f-145">The display name of the group to validate.</span></span> <span data-ttu-id="1223f-146">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="1223f-146">The property is not individually required.</span></span> <span data-ttu-id="1223f-147">但是, 至少需要一个属性 (**displayName**或**mailNickname**)。</span><span class="sxs-lookup"><span data-stu-id="1223f-147">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="1223f-148">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1223f-148">mailNickname</span></span>|<span data-ttu-id="1223f-149">String</span><span class="sxs-lookup"><span data-stu-id="1223f-149">String</span></span>| <span data-ttu-id="1223f-150">要验证的组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="1223f-150">The mail nickname of the group to validate.</span></span> <span data-ttu-id="1223f-151">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="1223f-151">The property is not individually required.</span></span> <span data-ttu-id="1223f-152">但是, 至少需要一个属性 (**displayName**或**mailNickname**)。</span><span class="sxs-lookup"><span data-stu-id="1223f-152">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="1223f-153">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="1223f-153">onBehalfOfUserId</span></span>|<span data-ttu-id="1223f-154">Guid</span><span class="sxs-lookup"><span data-stu-id="1223f-154">Guid</span></span>| <span data-ttu-id="1223f-155">调用 API 时要模拟的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="1223f-155">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="1223f-156">验证结果针对的是**onBehalfOfUserId 的**属性和角色。</span><span class="sxs-lookup"><span data-stu-id="1223f-156">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="1223f-157">响应</span><span class="sxs-lookup"><span data-stu-id="1223f-157">Response</span></span>

<span data-ttu-id="1223f-158">如果成功且没有验证错误, 则该方法返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="1223f-158">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="1223f-159">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1223f-159">It does not return anything in the response body.</span></span>

<span data-ttu-id="1223f-160">如果请求无效, 该方法将返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="1223f-160">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="1223f-161">有关无效请求的详细信息的错误消息将在响应正文中返回。</span><span class="sxs-lookup"><span data-stu-id="1223f-161">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="1223f-162">如果存在验证错误, 该方法将返回`422 Unprocessable Entity`响应代码。</span><span class="sxs-lookup"><span data-stu-id="1223f-162">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="1223f-163">响应正文中返回一条错误消息和一组错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="1223f-163">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1223f-164">示例</span><span class="sxs-lookup"><span data-stu-id="1223f-164">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="1223f-165">示例 1: 成功的验证请求</span><span class="sxs-lookup"><span data-stu-id="1223f-165">Example 1: Successful validation request</span></span>
<span data-ttu-id="1223f-166">这是一个成功的验证请求的示例。</span><span class="sxs-lookup"><span data-stu-id="1223f-166">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="1223f-167">请求</span><span class="sxs-lookup"><span data-stu-id="1223f-167">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1223f-168">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1223f-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1223f-169">C#</span><span class="sxs-lookup"><span data-stu-id="1223f-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1223f-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="1223f-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1223f-171">目标-C</span><span class="sxs-lookup"><span data-stu-id="1223f-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1223f-172">Java</span><span class="sxs-lookup"><span data-stu-id="1223f-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1223f-173">响应</span><span class="sxs-lookup"><span data-stu-id="1223f-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="1223f-174">示例 2: 包含验证错误的请求</span><span class="sxs-lookup"><span data-stu-id="1223f-174">Example 2: Request with validation errors</span></span>
<span data-ttu-id="1223f-175">这是包含验证错误的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="1223f-175">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="1223f-176">请求</span><span class="sxs-lookup"><span data-stu-id="1223f-176">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

#### <a name="response"></a><span data-ttu-id="1223f-177">响应</span><span class="sxs-lookup"><span data-stu-id="1223f-177">Response</span></span>
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
