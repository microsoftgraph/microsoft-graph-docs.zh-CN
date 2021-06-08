---
title: 更新 orgcontact
description: 更新 orgcontact 对象的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 26396518b40023e7a4b5666fb1d00b4effd83546
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785240"
---
# <a name="update-orgcontact"></a><span data-ttu-id="bbf39-103">更新 orgcontact</span><span class="sxs-lookup"><span data-stu-id="bbf39-103">Update orgcontact</span></span>

<span data-ttu-id="bbf39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbf39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbf39-105">更新 orgcontact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bbf39-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bbf39-106">权限</span><span class="sxs-lookup"><span data-stu-id="bbf39-106">Permissions</span></span>
<span data-ttu-id="bbf39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbf39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbf39-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbf39-109">Permission type</span></span>      | <span data-ttu-id="bbf39-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbf39-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbf39-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbf39-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bbf39-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbf39-112">Not supported.</span></span>    |
|<span data-ttu-id="bbf39-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbf39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbf39-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbf39-114">Not supported.</span></span>    |
|<span data-ttu-id="bbf39-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbf39-115">Application</span></span> | <span data-ttu-id="bbf39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbf39-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbf39-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbf39-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bbf39-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbf39-118">Request headers</span></span>
| <span data-ttu-id="bbf39-119">名称</span><span class="sxs-lookup"><span data-stu-id="bbf39-119">Name</span></span>       | <span data-ttu-id="bbf39-120">类型</span><span class="sxs-lookup"><span data-stu-id="bbf39-120">Type</span></span> | <span data-ttu-id="bbf39-121">说明</span><span class="sxs-lookup"><span data-stu-id="bbf39-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bbf39-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbf39-122">Authorization</span></span>  | <span data-ttu-id="bbf39-123">string</span><span class="sxs-lookup"><span data-stu-id="bbf39-123">string</span></span>  | <span data-ttu-id="bbf39-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbf39-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbf39-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbf39-126">Request body</span></span>
<span data-ttu-id="bbf39-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bbf39-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bbf39-130">属性</span><span class="sxs-lookup"><span data-stu-id="bbf39-130">Property</span></span>     | <span data-ttu-id="bbf39-131">类型</span><span class="sxs-lookup"><span data-stu-id="bbf39-131">Type</span></span>   |<span data-ttu-id="bbf39-132">说明</span><span class="sxs-lookup"><span data-stu-id="bbf39-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbf39-133">城市</span><span class="sxs-lookup"><span data-stu-id="bbf39-133">city</span></span>|<span data-ttu-id="bbf39-134">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-134">String</span></span>||
|<span data-ttu-id="bbf39-135">country</span><span class="sxs-lookup"><span data-stu-id="bbf39-135">country</span></span>|<span data-ttu-id="bbf39-136">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-136">String</span></span>||
|<span data-ttu-id="bbf39-137">department</span><span class="sxs-lookup"><span data-stu-id="bbf39-137">department</span></span>|<span data-ttu-id="bbf39-138">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-138">String</span></span>||
|<span data-ttu-id="bbf39-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="bbf39-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="bbf39-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbf39-140">Boolean</span></span>||
|<span data-ttu-id="bbf39-141">displayName</span><span class="sxs-lookup"><span data-stu-id="bbf39-141">displayName</span></span>|<span data-ttu-id="bbf39-142">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-142">String</span></span>||
|<span data-ttu-id="bbf39-143">givenName</span><span class="sxs-lookup"><span data-stu-id="bbf39-143">givenName</span></span>|<span data-ttu-id="bbf39-144">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-144">String</span></span>||
|<span data-ttu-id="bbf39-145">jobTitle</span><span class="sxs-lookup"><span data-stu-id="bbf39-145">jobTitle</span></span>|<span data-ttu-id="bbf39-146">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-146">String</span></span>||
|<span data-ttu-id="bbf39-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="bbf39-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="bbf39-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbf39-148">DateTimeOffset</span></span>||
|<span data-ttu-id="bbf39-149">mail</span><span class="sxs-lookup"><span data-stu-id="bbf39-149">mail</span></span>|<span data-ttu-id="bbf39-150">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-150">String</span></span>||
|<span data-ttu-id="bbf39-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="bbf39-151">mailNickname</span></span>|<span data-ttu-id="bbf39-152">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-152">String</span></span>||
|<span data-ttu-id="bbf39-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="bbf39-153">mobilePhone</span></span>|<span data-ttu-id="bbf39-154">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-154">String</span></span>||
|<span data-ttu-id="bbf39-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="bbf39-155">officeLocation</span></span>|<span data-ttu-id="bbf39-156">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-156">String</span></span>||
|<span data-ttu-id="bbf39-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="bbf39-157">postalCode</span></span>|<span data-ttu-id="bbf39-158">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-158">String</span></span>||
|<span data-ttu-id="bbf39-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="bbf39-159">proxyAddresses</span></span>|<span data-ttu-id="bbf39-160">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-160">String</span></span>||
|<span data-ttu-id="bbf39-161">state</span><span class="sxs-lookup"><span data-stu-id="bbf39-161">state</span></span>|<span data-ttu-id="bbf39-162">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-162">String</span></span>||
|<span data-ttu-id="bbf39-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="bbf39-163">streetAddress</span></span>|<span data-ttu-id="bbf39-164">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-164">String</span></span>||
|<span data-ttu-id="bbf39-165">surname</span><span class="sxs-lookup"><span data-stu-id="bbf39-165">surname</span></span>|<span data-ttu-id="bbf39-166">String</span><span class="sxs-lookup"><span data-stu-id="bbf39-166">String</span></span>||
|<span data-ttu-id="bbf39-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="bbf39-167">businessPhones</span></span>|<span data-ttu-id="bbf39-168">String collection</span><span class="sxs-lookup"><span data-stu-id="bbf39-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="bbf39-169">响应</span><span class="sxs-lookup"><span data-stu-id="bbf39-169">Response</span></span>

<span data-ttu-id="bbf39-170">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bbf39-170">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bbf39-171">示例</span><span class="sxs-lookup"><span data-stu-id="bbf39-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbf39-172">请求</span><span class="sxs-lookup"><span data-stu-id="bbf39-172">Request</span></span>
<span data-ttu-id="bbf39-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bbf39-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bbf39-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbf39-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_orgcontact"
}-->
```http
PATCH https://graph.microsoft.com/beta/contacts/{id}
Content-type: application/json
Content-length: 222

{
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value",
  "country": "country-value",
  "department": "department-value",
  "displayName": "displayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="bbf39-175">C#</span><span class="sxs-lookup"><span data-stu-id="bbf39-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbf39-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbf39-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbf39-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbf39-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bbf39-178">响应</span><span class="sxs-lookup"><span data-stu-id="bbf39-178">Response</span></span>
<span data-ttu-id="bbf39-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bbf39-179">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update orgcontact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


