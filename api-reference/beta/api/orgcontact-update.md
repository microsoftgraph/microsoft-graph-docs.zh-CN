---
title: 更新 orgcontact
description: 更新 orgcontact 对象的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c425af3a39a2a9f13a46792d8482d59804c8d37f
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352149"
---
# <a name="update-orgcontact"></a><span data-ttu-id="83a1b-103">更新 orgcontact</span><span class="sxs-lookup"><span data-stu-id="83a1b-103">Update orgcontact</span></span>

<span data-ttu-id="83a1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83a1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83a1b-105">更新 orgcontact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="83a1b-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="83a1b-106">权限</span><span class="sxs-lookup"><span data-stu-id="83a1b-106">Permissions</span></span>
<span data-ttu-id="83a1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83a1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83a1b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83a1b-109">Permission type</span></span>      | <span data-ttu-id="83a1b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83a1b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83a1b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83a1b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="83a1b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="83a1b-112">Not supported.</span></span>    |
|<span data-ttu-id="83a1b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83a1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83a1b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83a1b-114">Not supported.</span></span>    |
|<span data-ttu-id="83a1b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83a1b-115">Application</span></span> | <span data-ttu-id="83a1b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83a1b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83a1b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83a1b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="83a1b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="83a1b-118">Request headers</span></span>
| <span data-ttu-id="83a1b-119">名称</span><span class="sxs-lookup"><span data-stu-id="83a1b-119">Name</span></span>       | <span data-ttu-id="83a1b-120">类型</span><span class="sxs-lookup"><span data-stu-id="83a1b-120">Type</span></span> | <span data-ttu-id="83a1b-121">说明</span><span class="sxs-lookup"><span data-stu-id="83a1b-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="83a1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83a1b-122">Authorization</span></span>  | <span data-ttu-id="83a1b-123">string</span><span class="sxs-lookup"><span data-stu-id="83a1b-123">string</span></span>  | <span data-ttu-id="83a1b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83a1b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83a1b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="83a1b-126">Request body</span></span>
<span data-ttu-id="83a1b-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="83a1b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="83a1b-130">属性</span><span class="sxs-lookup"><span data-stu-id="83a1b-130">Property</span></span>     | <span data-ttu-id="83a1b-131">类型</span><span class="sxs-lookup"><span data-stu-id="83a1b-131">Type</span></span>   |<span data-ttu-id="83a1b-132">Description</span><span class="sxs-lookup"><span data-stu-id="83a1b-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83a1b-133">城市</span><span class="sxs-lookup"><span data-stu-id="83a1b-133">city</span></span>|<span data-ttu-id="83a1b-134">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-134">String</span></span>||
|<span data-ttu-id="83a1b-135">country</span><span class="sxs-lookup"><span data-stu-id="83a1b-135">country</span></span>|<span data-ttu-id="83a1b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="83a1b-136">String</span></span>||
|<span data-ttu-id="83a1b-137">department</span><span class="sxs-lookup"><span data-stu-id="83a1b-137">department</span></span>|<span data-ttu-id="83a1b-138">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-138">String</span></span>||
|<span data-ttu-id="83a1b-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="83a1b-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="83a1b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="83a1b-140">Boolean</span></span>||
|<span data-ttu-id="83a1b-141">displayName</span><span class="sxs-lookup"><span data-stu-id="83a1b-141">displayName</span></span>|<span data-ttu-id="83a1b-142">字符串</span><span class="sxs-lookup"><span data-stu-id="83a1b-142">String</span></span>||
|<span data-ttu-id="83a1b-143">givenName</span><span class="sxs-lookup"><span data-stu-id="83a1b-143">givenName</span></span>|<span data-ttu-id="83a1b-144">字符串</span><span class="sxs-lookup"><span data-stu-id="83a1b-144">String</span></span>||
|<span data-ttu-id="83a1b-145">jobTitle</span><span class="sxs-lookup"><span data-stu-id="83a1b-145">jobTitle</span></span>|<span data-ttu-id="83a1b-146">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-146">String</span></span>||
|<span data-ttu-id="83a1b-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="83a1b-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="83a1b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83a1b-148">DateTimeOffset</span></span>||
|<span data-ttu-id="83a1b-149">mail</span><span class="sxs-lookup"><span data-stu-id="83a1b-149">mail</span></span>|<span data-ttu-id="83a1b-150">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-150">String</span></span>||
|<span data-ttu-id="83a1b-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="83a1b-151">mailNickname</span></span>|<span data-ttu-id="83a1b-152">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-152">String</span></span>||
|<span data-ttu-id="83a1b-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="83a1b-153">mobilePhone</span></span>|<span data-ttu-id="83a1b-154">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-154">String</span></span>||
|<span data-ttu-id="83a1b-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="83a1b-155">officeLocation</span></span>|<span data-ttu-id="83a1b-156">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-156">String</span></span>||
|<span data-ttu-id="83a1b-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="83a1b-157">postalCode</span></span>|<span data-ttu-id="83a1b-158">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-158">String</span></span>||
|<span data-ttu-id="83a1b-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="83a1b-159">proxyAddresses</span></span>|<span data-ttu-id="83a1b-160">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-160">String</span></span>||
|<span data-ttu-id="83a1b-161">state</span><span class="sxs-lookup"><span data-stu-id="83a1b-161">state</span></span>|<span data-ttu-id="83a1b-162">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-162">String</span></span>||
|<span data-ttu-id="83a1b-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="83a1b-163">streetAddress</span></span>|<span data-ttu-id="83a1b-164">String</span><span class="sxs-lookup"><span data-stu-id="83a1b-164">String</span></span>||
|<span data-ttu-id="83a1b-165">surname</span><span class="sxs-lookup"><span data-stu-id="83a1b-165">surname</span></span>|<span data-ttu-id="83a1b-166">字符串</span><span class="sxs-lookup"><span data-stu-id="83a1b-166">String</span></span>||
|<span data-ttu-id="83a1b-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="83a1b-167">businessPhones</span></span>|<span data-ttu-id="83a1b-168">String collection</span><span class="sxs-lookup"><span data-stu-id="83a1b-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="83a1b-169">响应</span><span class="sxs-lookup"><span data-stu-id="83a1b-169">Response</span></span>

<span data-ttu-id="83a1b-170">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="83a1b-170">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="83a1b-171">示例</span><span class="sxs-lookup"><span data-stu-id="83a1b-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83a1b-172">请求</span><span class="sxs-lookup"><span data-stu-id="83a1b-172">Request</span></span>
<span data-ttu-id="83a1b-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="83a1b-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83a1b-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="83a1b-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="83a1b-175">C#</span><span class="sxs-lookup"><span data-stu-id="83a1b-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83a1b-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83a1b-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83a1b-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83a1b-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="83a1b-178">响应</span><span class="sxs-lookup"><span data-stu-id="83a1b-178">Response</span></span>
<span data-ttu-id="83a1b-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="83a1b-179">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact"
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


