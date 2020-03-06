---
title: directoryObject： validateProperties
description: 验证 Office 365 组的显示名称或邮件别名是否符合命名策略。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bcee27c646831f414fdba18c67176073a7b61d48
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517970"
---
# <a name="directoryobject-validateproperties"></a><span data-ttu-id="eb670-103">directoryObject： validateProperties</span><span class="sxs-lookup"><span data-stu-id="eb670-103">directoryObject: validateProperties</span></span>

<span data-ttu-id="eb670-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb670-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eb670-105">验证 Office 365 组的显示名称或邮件别名是否符合命名策略。</span><span class="sxs-lookup"><span data-stu-id="eb670-105">Validate that an Office 365 group's display name or mail nickname complies with naming policies.</span></span>  <span data-ttu-id="eb670-106">在尝试[创建](group-post-groups.md)Office 365 组之前，客户端可以使用此 API 来确定显示名称或邮件昵称是否有效。</span><span class="sxs-lookup"><span data-stu-id="eb670-106">Clients can use this API to determine whether a display name or mail nickname is valid before trying to [create](group-post-groups.md) an Office 365 group.</span></span> <span data-ttu-id="eb670-107">若要验证现有组的属性，请使用[group： validateProperties](group-validateproperties.md)函数。</span><span class="sxs-lookup"><span data-stu-id="eb670-107">To validate the properties of an existing group, use the [group: validateProperties](group-validateproperties.md) function.</span></span>

<span data-ttu-id="eb670-108">将为显示名称和邮件昵称属性执行以下策略验证：</span><span class="sxs-lookup"><span data-stu-id="eb670-108">The following policy validations are performed for the display name and mail nickname properties:</span></span>
1. <span data-ttu-id="eb670-109">验证前缀和后缀命名策略</span><span class="sxs-lookup"><span data-stu-id="eb670-109">Validate the prefix and suffix naming policy</span></span>
2. <span data-ttu-id="eb670-110">验证 "自定义禁止的词语" 策略</span><span class="sxs-lookup"><span data-stu-id="eb670-110">Validate the custom banned words policy</span></span>
3. <span data-ttu-id="eb670-111">验证邮件昵称是否唯一</span><span class="sxs-lookup"><span data-stu-id="eb670-111">Validate that the mail nickname is unique</span></span>

<span data-ttu-id="eb670-112">此 API 仅返回遇到的第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="eb670-112">This API only returns the first validation failure that is encountered.</span></span> <span data-ttu-id="eb670-113">如果属性失败多次验证，则仅返回第一个验证失败。</span><span class="sxs-lookup"><span data-stu-id="eb670-113">If the properties fail multiple validations, only the first validation failure is returned.</span></span> <span data-ttu-id="eb670-114">但是，如果仅验证前缀和后缀命名策略，则可以验证邮件别名和显示名称，并接收验证错误的集合。</span><span class="sxs-lookup"><span data-stu-id="eb670-114">However, you can validate both the mail nickname and the display name and receive a collection of validation errors if you are only validating the prefix and suffix naming policy.</span></span> <span data-ttu-id="eb670-115">若要了解有关配置命名策略的详细信息，请参阅[Configure 命名策略](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell)。</span><span class="sxs-lookup"><span data-stu-id="eb670-115">To learn more about configuring naming policies, see [Configure naming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb670-116">权限</span><span class="sxs-lookup"><span data-stu-id="eb670-116">Permissions</span></span>
<span data-ttu-id="eb670-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb670-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb670-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb670-119">Permission type</span></span>      | <span data-ttu-id="eb670-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb670-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb670-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb670-121">Delegated (work or school account)</span></span> | <span data-ttu-id="eb670-122">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eb670-122">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="eb670-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb670-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb670-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb670-124">Not supported.</span></span>    |
|<span data-ttu-id="eb670-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb670-125">Application</span></span> | <span data-ttu-id="eb670-126">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb670-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb670-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb670-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a><span data-ttu-id="eb670-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb670-128">Request headers</span></span>

| <span data-ttu-id="eb670-129">名称</span><span class="sxs-lookup"><span data-stu-id="eb670-129">Name</span></span>           | <span data-ttu-id="eb670-130">说明</span><span class="sxs-lookup"><span data-stu-id="eb670-130">Description</span></span>      |
|:---------------|:-----------------|
| <span data-ttu-id="eb670-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb670-131">Authorization</span></span>  | <span data-ttu-id="eb670-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb670-p104">Bearer {token}. Required.</span></span>    |
| <span data-ttu-id="eb670-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eb670-134">Content-Type</span></span>   | <span data-ttu-id="eb670-135">application/json</span><span class="sxs-lookup"><span data-stu-id="eb670-135">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb670-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb670-136">Request body</span></span>
<span data-ttu-id="eb670-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="eb670-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eb670-138">参数</span><span class="sxs-lookup"><span data-stu-id="eb670-138">Parameter</span></span>    | <span data-ttu-id="eb670-139">类型</span><span class="sxs-lookup"><span data-stu-id="eb670-139">Type</span></span>   |<span data-ttu-id="eb670-140">说明</span><span class="sxs-lookup"><span data-stu-id="eb670-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb670-141">entityType</span><span class="sxs-lookup"><span data-stu-id="eb670-141">entityType</span></span>|<span data-ttu-id="eb670-142">字符串</span><span class="sxs-lookup"><span data-stu-id="eb670-142">String</span></span>| <span data-ttu-id="eb670-143">Group 是唯一受支持的实体类型。</span><span class="sxs-lookup"><span data-stu-id="eb670-143">Group is the only supported entity type.</span></span> |
|<span data-ttu-id="eb670-144">displayName</span><span class="sxs-lookup"><span data-stu-id="eb670-144">displayName</span></span>|<span data-ttu-id="eb670-145">String</span><span class="sxs-lookup"><span data-stu-id="eb670-145">String</span></span>| <span data-ttu-id="eb670-146">要验证的组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="eb670-146">The display name of the group to validate.</span></span> <span data-ttu-id="eb670-147">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="eb670-147">The property is not individually required.</span></span> <span data-ttu-id="eb670-148">但是，至少需要一个属性（**displayName**或**mailNickname**）。</span><span class="sxs-lookup"><span data-stu-id="eb670-148">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="eb670-149">mailNickname</span><span class="sxs-lookup"><span data-stu-id="eb670-149">mailNickname</span></span>|<span data-ttu-id="eb670-150">String</span><span class="sxs-lookup"><span data-stu-id="eb670-150">String</span></span>| <span data-ttu-id="eb670-151">要验证的组的邮件别名。</span><span class="sxs-lookup"><span data-stu-id="eb670-151">The mail nickname of the group to validate.</span></span> <span data-ttu-id="eb670-152">属性不是单独需要的。</span><span class="sxs-lookup"><span data-stu-id="eb670-152">The property is not individually required.</span></span> <span data-ttu-id="eb670-153">但是，至少需要一个属性（**displayName**或**mailNickname**）。</span><span class="sxs-lookup"><span data-stu-id="eb670-153">However, at least one property (**displayName** or **mailNickname**) is required.</span></span> |
|<span data-ttu-id="eb670-154">onBehalfOfUserId</span><span class="sxs-lookup"><span data-stu-id="eb670-154">onBehalfOfUserId</span></span>|<span data-ttu-id="eb670-155">Guid</span><span class="sxs-lookup"><span data-stu-id="eb670-155">Guid</span></span>| <span data-ttu-id="eb670-156">调用 API 时要模拟的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="eb670-156">The ID of the user to impersonate when calling the API.</span></span> <span data-ttu-id="eb670-157">验证结果针对的是**onBehalfOfUserId 的**属性和角色。</span><span class="sxs-lookup"><span data-stu-id="eb670-157">The validation results are for the **onBehalfOfUserId's** attributes and roles.</span></span> |

## <a name="response"></a><span data-ttu-id="eb670-158">响应</span><span class="sxs-lookup"><span data-stu-id="eb670-158">Response</span></span>

<span data-ttu-id="eb670-159">如果成功且没有验证错误，则该方法返回`204 No Content`响应代码。</span><span class="sxs-lookup"><span data-stu-id="eb670-159">If successful and there are no validation errors, the method returns `204 No Content` response code.</span></span> <span data-ttu-id="eb670-160">它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eb670-160">It does not return anything in the response body.</span></span>

<span data-ttu-id="eb670-161">如果请求无效，该方法将返回`400 Bad Request`响应代码。</span><span class="sxs-lookup"><span data-stu-id="eb670-161">If the request is invalid, the method returns `400 Bad Request` response code.</span></span> <span data-ttu-id="eb670-162">有关无效请求的详细信息的错误消息将在响应正文中返回。</span><span class="sxs-lookup"><span data-stu-id="eb670-162">An error message with details about the invalid request is returned in the response body.</span></span>

<span data-ttu-id="eb670-163">如果存在验证错误，该方法将返回`422 Unprocessable Entity`响应代码。</span><span class="sxs-lookup"><span data-stu-id="eb670-163">If there is a validation error, the method returns `422 Unprocessable Entity` response code.</span></span> <span data-ttu-id="eb670-164">响应正文中返回一条错误消息和一组错误详细信息。</span><span class="sxs-lookup"><span data-stu-id="eb670-164">An error message and a collection of error details is returned in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb670-165">示例</span><span class="sxs-lookup"><span data-stu-id="eb670-165">Examples</span></span>

### <a name="example-1-successful-validation-request"></a><span data-ttu-id="eb670-166">示例1：成功的验证请求</span><span class="sxs-lookup"><span data-stu-id="eb670-166">Example 1: Successful validation request</span></span>
<span data-ttu-id="eb670-167">这是一个成功的验证请求的示例。</span><span class="sxs-lookup"><span data-stu-id="eb670-167">This is an example of a successful validation request.</span></span>

#### <a name="request"></a><span data-ttu-id="eb670-168">请求</span><span class="sxs-lookup"><span data-stu-id="eb670-168">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eb670-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb670-169">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="eb670-170">C#</span><span class="sxs-lookup"><span data-stu-id="eb670-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb670-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb670-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb670-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb670-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eb670-173">Java</span><span class="sxs-lookup"><span data-stu-id="eb670-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="eb670-174">响应</span><span class="sxs-lookup"><span data-stu-id="eb670-174">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


### <a name="example-2-request-with-validation-errors"></a><span data-ttu-id="eb670-175">示例2：包含验证错误的请求</span><span class="sxs-lookup"><span data-stu-id="eb670-175">Example 2: Request with validation errors</span></span>
<span data-ttu-id="eb670-176">这是包含验证错误的请求的示例。</span><span class="sxs-lookup"><span data-stu-id="eb670-176">This is an example of a request with validation errors.</span></span>

#### <a name="request"></a><span data-ttu-id="eb670-177">请求</span><span class="sxs-lookup"><span data-stu-id="eb670-177">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="eb670-178">响应</span><span class="sxs-lookup"><span data-stu-id="eb670-178">Response</span></span>
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
