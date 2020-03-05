---
title: 更新 orgcontact
description: 更新 orgcontact 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c56ab5562e9b242819d7110914329996e64596a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456232"
---
# <a name="update-orgcontact"></a><span data-ttu-id="2e923-103">更新 orgcontact</span><span class="sxs-lookup"><span data-stu-id="2e923-103">Update orgcontact</span></span>

<span data-ttu-id="2e923-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2e923-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e923-105">更新 orgcontact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2e923-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2e923-106">权限</span><span class="sxs-lookup"><span data-stu-id="2e923-106">Permissions</span></span>
<span data-ttu-id="2e923-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e923-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e923-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e923-109">Permission type</span></span>      | <span data-ttu-id="2e923-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e923-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e923-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e923-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e923-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e923-112">Not supported.</span></span>    |
|<span data-ttu-id="2e923-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e923-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e923-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e923-114">Not supported.</span></span>    |
|<span data-ttu-id="2e923-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e923-115">Application</span></span> | <span data-ttu-id="2e923-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e923-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e923-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e923-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2e923-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e923-118">Request headers</span></span>
| <span data-ttu-id="2e923-119">名称</span><span class="sxs-lookup"><span data-stu-id="2e923-119">Name</span></span>       | <span data-ttu-id="2e923-120">类型</span><span class="sxs-lookup"><span data-stu-id="2e923-120">Type</span></span> | <span data-ttu-id="2e923-121">说明</span><span class="sxs-lookup"><span data-stu-id="2e923-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2e923-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e923-122">Authorization</span></span>  | <span data-ttu-id="2e923-123">string</span><span class="sxs-lookup"><span data-stu-id="2e923-123">string</span></span>  | <span data-ttu-id="2e923-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e923-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e923-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e923-126">Request body</span></span>
<span data-ttu-id="2e923-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2e923-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2e923-130">属性</span><span class="sxs-lookup"><span data-stu-id="2e923-130">Property</span></span>     | <span data-ttu-id="2e923-131">类型</span><span class="sxs-lookup"><span data-stu-id="2e923-131">Type</span></span>   |<span data-ttu-id="2e923-132">说明</span><span class="sxs-lookup"><span data-stu-id="2e923-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e923-133">城市</span><span class="sxs-lookup"><span data-stu-id="2e923-133">city</span></span>|<span data-ttu-id="2e923-134">String</span><span class="sxs-lookup"><span data-stu-id="2e923-134">String</span></span>||
|<span data-ttu-id="2e923-135">country</span><span class="sxs-lookup"><span data-stu-id="2e923-135">country</span></span>|<span data-ttu-id="2e923-136">字符串</span><span class="sxs-lookup"><span data-stu-id="2e923-136">String</span></span>||
|<span data-ttu-id="2e923-137">department</span><span class="sxs-lookup"><span data-stu-id="2e923-137">department</span></span>|<span data-ttu-id="2e923-138">String</span><span class="sxs-lookup"><span data-stu-id="2e923-138">String</span></span>||
|<span data-ttu-id="2e923-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="2e923-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="2e923-140">布尔</span><span class="sxs-lookup"><span data-stu-id="2e923-140">Boolean</span></span>||
|<span data-ttu-id="2e923-141">displayName</span><span class="sxs-lookup"><span data-stu-id="2e923-141">displayName</span></span>|<span data-ttu-id="2e923-142">String</span><span class="sxs-lookup"><span data-stu-id="2e923-142">String</span></span>||
|<span data-ttu-id="2e923-143">givenName</span><span class="sxs-lookup"><span data-stu-id="2e923-143">givenName</span></span>|<span data-ttu-id="2e923-144">String</span><span class="sxs-lookup"><span data-stu-id="2e923-144">String</span></span>||
|<span data-ttu-id="2e923-145">jobTitle</span><span class="sxs-lookup"><span data-stu-id="2e923-145">jobTitle</span></span>|<span data-ttu-id="2e923-146">String</span><span class="sxs-lookup"><span data-stu-id="2e923-146">String</span></span>||
|<span data-ttu-id="2e923-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2e923-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="2e923-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e923-148">DateTimeOffset</span></span>||
|<span data-ttu-id="2e923-149">mail</span><span class="sxs-lookup"><span data-stu-id="2e923-149">mail</span></span>|<span data-ttu-id="2e923-150">String</span><span class="sxs-lookup"><span data-stu-id="2e923-150">String</span></span>||
|<span data-ttu-id="2e923-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2e923-151">mailNickname</span></span>|<span data-ttu-id="2e923-152">String</span><span class="sxs-lookup"><span data-stu-id="2e923-152">String</span></span>||
|<span data-ttu-id="2e923-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="2e923-153">mobilePhone</span></span>|<span data-ttu-id="2e923-154">String</span><span class="sxs-lookup"><span data-stu-id="2e923-154">String</span></span>||
|<span data-ttu-id="2e923-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="2e923-155">officeLocation</span></span>|<span data-ttu-id="2e923-156">String</span><span class="sxs-lookup"><span data-stu-id="2e923-156">String</span></span>||
|<span data-ttu-id="2e923-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="2e923-157">postalCode</span></span>|<span data-ttu-id="2e923-158">String</span><span class="sxs-lookup"><span data-stu-id="2e923-158">String</span></span>||
|<span data-ttu-id="2e923-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="2e923-159">proxyAddresses</span></span>|<span data-ttu-id="2e923-160">String</span><span class="sxs-lookup"><span data-stu-id="2e923-160">String</span></span>||
|<span data-ttu-id="2e923-161">state</span><span class="sxs-lookup"><span data-stu-id="2e923-161">state</span></span>|<span data-ttu-id="2e923-162">字符串</span><span class="sxs-lookup"><span data-stu-id="2e923-162">String</span></span>||
|<span data-ttu-id="2e923-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="2e923-163">streetAddress</span></span>|<span data-ttu-id="2e923-164">String</span><span class="sxs-lookup"><span data-stu-id="2e923-164">String</span></span>||
|<span data-ttu-id="2e923-165">surname</span><span class="sxs-lookup"><span data-stu-id="2e923-165">surname</span></span>|<span data-ttu-id="2e923-166">String</span><span class="sxs-lookup"><span data-stu-id="2e923-166">String</span></span>||
|<span data-ttu-id="2e923-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="2e923-167">businessPhones</span></span>|<span data-ttu-id="2e923-168">String collection</span><span class="sxs-lookup"><span data-stu-id="2e923-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="2e923-169">响应</span><span class="sxs-lookup"><span data-stu-id="2e923-169">Response</span></span>

<span data-ttu-id="2e923-170">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[orgContact](../resources/orgcontact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2e923-170">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e923-171">示例</span><span class="sxs-lookup"><span data-stu-id="2e923-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e923-172">请求</span><span class="sxs-lookup"><span data-stu-id="2e923-172">Request</span></span>
<span data-ttu-id="2e923-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e923-173">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e923-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e923-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2e923-175">C#</span><span class="sxs-lookup"><span data-stu-id="2e923-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e923-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e923-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e923-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e923-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2e923-178">响应</span><span class="sxs-lookup"><span data-stu-id="2e923-178">Response</span></span>
<span data-ttu-id="2e923-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e923-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
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
