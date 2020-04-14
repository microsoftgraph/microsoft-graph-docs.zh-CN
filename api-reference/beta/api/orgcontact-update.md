---
title: 更新 orgcontact
description: 更新 orgcontact 对象的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aa9704c44dc8dc7068bf387b97669e2c42aecdd2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403222"
---
# <a name="update-orgcontact"></a><span data-ttu-id="2df03-103">更新 orgcontact</span><span class="sxs-lookup"><span data-stu-id="2df03-103">Update orgcontact</span></span>

<span data-ttu-id="2df03-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2df03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2df03-105">更新 orgcontact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2df03-105">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2df03-106">权限</span><span class="sxs-lookup"><span data-stu-id="2df03-106">Permissions</span></span>
<span data-ttu-id="2df03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2df03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2df03-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2df03-109">Permission type</span></span>      | <span data-ttu-id="2df03-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2df03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2df03-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2df03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2df03-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2df03-112">Not supported.</span></span>    |
|<span data-ttu-id="2df03-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2df03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2df03-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2df03-114">Not supported.</span></span>    |
|<span data-ttu-id="2df03-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2df03-115">Application</span></span> | <span data-ttu-id="2df03-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2df03-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2df03-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2df03-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2df03-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2df03-118">Request headers</span></span>
| <span data-ttu-id="2df03-119">名称</span><span class="sxs-lookup"><span data-stu-id="2df03-119">Name</span></span>       | <span data-ttu-id="2df03-120">类型</span><span class="sxs-lookup"><span data-stu-id="2df03-120">Type</span></span> | <span data-ttu-id="2df03-121">说明</span><span class="sxs-lookup"><span data-stu-id="2df03-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2df03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2df03-122">Authorization</span></span>  | <span data-ttu-id="2df03-123">string</span><span class="sxs-lookup"><span data-stu-id="2df03-123">string</span></span>  | <span data-ttu-id="2df03-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2df03-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2df03-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2df03-126">Request body</span></span>
<span data-ttu-id="2df03-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="2df03-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2df03-130">属性</span><span class="sxs-lookup"><span data-stu-id="2df03-130">Property</span></span>     | <span data-ttu-id="2df03-131">类型</span><span class="sxs-lookup"><span data-stu-id="2df03-131">Type</span></span>   |<span data-ttu-id="2df03-132">说明</span><span class="sxs-lookup"><span data-stu-id="2df03-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2df03-133">city</span><span class="sxs-lookup"><span data-stu-id="2df03-133">city</span></span>|<span data-ttu-id="2df03-134">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-134">String</span></span>||
|<span data-ttu-id="2df03-135">country</span><span class="sxs-lookup"><span data-stu-id="2df03-135">country</span></span>|<span data-ttu-id="2df03-136">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-136">String</span></span>||
|<span data-ttu-id="2df03-137">department</span><span class="sxs-lookup"><span data-stu-id="2df03-137">department</span></span>|<span data-ttu-id="2df03-138">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-138">String</span></span>||
|<span data-ttu-id="2df03-139">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="2df03-139">onPremisesSyncEnabled</span></span>|<span data-ttu-id="2df03-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="2df03-140">Boolean</span></span>||
|<span data-ttu-id="2df03-141">displayName</span><span class="sxs-lookup"><span data-stu-id="2df03-141">displayName</span></span>|<span data-ttu-id="2df03-142">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-142">String</span></span>||
|<span data-ttu-id="2df03-143">givenName</span><span class="sxs-lookup"><span data-stu-id="2df03-143">givenName</span></span>|<span data-ttu-id="2df03-144">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-144">String</span></span>||
|<span data-ttu-id="2df03-145">jobTitle</span><span class="sxs-lookup"><span data-stu-id="2df03-145">jobTitle</span></span>|<span data-ttu-id="2df03-146">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-146">String</span></span>||
|<span data-ttu-id="2df03-147">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2df03-147">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="2df03-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df03-148">DateTimeOffset</span></span>||
|<span data-ttu-id="2df03-149">mail</span><span class="sxs-lookup"><span data-stu-id="2df03-149">mail</span></span>|<span data-ttu-id="2df03-150">String</span><span class="sxs-lookup"><span data-stu-id="2df03-150">String</span></span>||
|<span data-ttu-id="2df03-151">mailNickname</span><span class="sxs-lookup"><span data-stu-id="2df03-151">mailNickname</span></span>|<span data-ttu-id="2df03-152">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-152">String</span></span>||
|<span data-ttu-id="2df03-153">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="2df03-153">mobilePhone</span></span>|<span data-ttu-id="2df03-154">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-154">String</span></span>||
|<span data-ttu-id="2df03-155">officeLocation</span><span class="sxs-lookup"><span data-stu-id="2df03-155">officeLocation</span></span>|<span data-ttu-id="2df03-156">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-156">String</span></span>||
|<span data-ttu-id="2df03-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="2df03-157">postalCode</span></span>|<span data-ttu-id="2df03-158">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-158">String</span></span>||
|<span data-ttu-id="2df03-159">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="2df03-159">proxyAddresses</span></span>|<span data-ttu-id="2df03-160">String</span><span class="sxs-lookup"><span data-stu-id="2df03-160">String</span></span>||
|<span data-ttu-id="2df03-161">state</span><span class="sxs-lookup"><span data-stu-id="2df03-161">state</span></span>|<span data-ttu-id="2df03-162">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-162">String</span></span>||
|<span data-ttu-id="2df03-163">streetAddress</span><span class="sxs-lookup"><span data-stu-id="2df03-163">streetAddress</span></span>|<span data-ttu-id="2df03-164">字符串</span><span class="sxs-lookup"><span data-stu-id="2df03-164">String</span></span>||
|<span data-ttu-id="2df03-165">surname</span><span class="sxs-lookup"><span data-stu-id="2df03-165">surname</span></span>|<span data-ttu-id="2df03-166">String</span><span class="sxs-lookup"><span data-stu-id="2df03-166">String</span></span>||
|<span data-ttu-id="2df03-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="2df03-167">businessPhones</span></span>|<span data-ttu-id="2df03-168">String collection</span><span class="sxs-lookup"><span data-stu-id="2df03-168">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="2df03-169">响应</span><span class="sxs-lookup"><span data-stu-id="2df03-169">Response</span></span>

<span data-ttu-id="2df03-170">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[orgContact](../resources/orgcontact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2df03-170">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2df03-171">示例</span><span class="sxs-lookup"><span data-stu-id="2df03-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2df03-172">请求</span><span class="sxs-lookup"><span data-stu-id="2df03-172">Request</span></span>
<span data-ttu-id="2df03-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2df03-173">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2df03-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="2df03-174">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2df03-175">C#</span><span class="sxs-lookup"><span data-stu-id="2df03-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2df03-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2df03-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2df03-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2df03-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2df03-178">响应</span><span class="sxs-lookup"><span data-stu-id="2df03-178">Response</span></span>
<span data-ttu-id="2df03-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2df03-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
