---
title: 更新 orgcontact
description: 更新 orgcontact 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99cc8b77dcb3fcbea9e1e22bd4a04e7f68b8f3c4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877827"
---
# <a name="update-orgcontact"></a><span data-ttu-id="d7b62-103">更新 orgcontact</span><span class="sxs-lookup"><span data-stu-id="d7b62-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7b62-104">更新 orgcontact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d7b62-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7b62-105">权限</span><span class="sxs-lookup"><span data-stu-id="d7b62-105">Permissions</span></span>
<span data-ttu-id="d7b62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7b62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7b62-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7b62-108">Permission type</span></span>      | <span data-ttu-id="d7b62-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7b62-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7b62-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7b62-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7b62-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7b62-111">Not supported.</span></span>    |
|<span data-ttu-id="d7b62-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7b62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7b62-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7b62-113">Not supported.</span></span>    |
|<span data-ttu-id="d7b62-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7b62-114">Application</span></span> | <span data-ttu-id="d7b62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7b62-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7b62-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7b62-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d7b62-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7b62-117">Request headers</span></span>
| <span data-ttu-id="d7b62-118">名称</span><span class="sxs-lookup"><span data-stu-id="d7b62-118">Name</span></span>       | <span data-ttu-id="d7b62-119">类型</span><span class="sxs-lookup"><span data-stu-id="d7b62-119">Type</span></span> | <span data-ttu-id="d7b62-120">说明</span><span class="sxs-lookup"><span data-stu-id="d7b62-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d7b62-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7b62-121">Authorization</span></span>  | <span data-ttu-id="d7b62-122">string</span><span class="sxs-lookup"><span data-stu-id="d7b62-122">string</span></span>  | <span data-ttu-id="d7b62-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7b62-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7b62-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7b62-125">Request body</span></span>
<span data-ttu-id="d7b62-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d7b62-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d7b62-129">属性</span><span class="sxs-lookup"><span data-stu-id="d7b62-129">Property</span></span>     | <span data-ttu-id="d7b62-130">类型</span><span class="sxs-lookup"><span data-stu-id="d7b62-130">Type</span></span>   |<span data-ttu-id="d7b62-131">说明</span><span class="sxs-lookup"><span data-stu-id="d7b62-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7b62-132">city</span><span class="sxs-lookup"><span data-stu-id="d7b62-132">city</span></span>|<span data-ttu-id="d7b62-133">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-133">String</span></span>||
|<span data-ttu-id="d7b62-134">country</span><span class="sxs-lookup"><span data-stu-id="d7b62-134">country</span></span>|<span data-ttu-id="d7b62-135">字符串</span><span class="sxs-lookup"><span data-stu-id="d7b62-135">String</span></span>||
|<span data-ttu-id="d7b62-136">department</span><span class="sxs-lookup"><span data-stu-id="d7b62-136">department</span></span>|<span data-ttu-id="d7b62-137">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-137">String</span></span>||
|<span data-ttu-id="d7b62-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="d7b62-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="d7b62-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7b62-139">Boolean</span></span>||
|<span data-ttu-id="d7b62-140">displayName</span><span class="sxs-lookup"><span data-stu-id="d7b62-140">displayName</span></span>|<span data-ttu-id="d7b62-141">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-141">String</span></span>||
|<span data-ttu-id="d7b62-142">givenName</span><span class="sxs-lookup"><span data-stu-id="d7b62-142">givenName</span></span>|<span data-ttu-id="d7b62-143">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-143">String</span></span>||
|<span data-ttu-id="d7b62-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="d7b62-144">jobTitle</span></span>|<span data-ttu-id="d7b62-145">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-145">String</span></span>||
|<span data-ttu-id="d7b62-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d7b62-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="d7b62-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7b62-147">DateTimeOffset</span></span>||
|<span data-ttu-id="d7b62-148">mail</span><span class="sxs-lookup"><span data-stu-id="d7b62-148">mail</span></span>|<span data-ttu-id="d7b62-149">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-149">String</span></span>||
|<span data-ttu-id="d7b62-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d7b62-150">mailNickname</span></span>|<span data-ttu-id="d7b62-151">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-151">String</span></span>||
|<span data-ttu-id="d7b62-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="d7b62-152">mobilePhone</span></span>|<span data-ttu-id="d7b62-153">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-153">String</span></span>||
|<span data-ttu-id="d7b62-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="d7b62-154">officeLocation</span></span>|<span data-ttu-id="d7b62-155">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-155">String</span></span>||
|<span data-ttu-id="d7b62-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="d7b62-156">postalCode</span></span>|<span data-ttu-id="d7b62-157">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-157">String</span></span>||
|<span data-ttu-id="d7b62-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="d7b62-158">proxyAddresses</span></span>|<span data-ttu-id="d7b62-159">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-159">String</span></span>||
|<span data-ttu-id="d7b62-160">state</span><span class="sxs-lookup"><span data-stu-id="d7b62-160">state</span></span>|<span data-ttu-id="d7b62-161">字符串</span><span class="sxs-lookup"><span data-stu-id="d7b62-161">String</span></span>||
|<span data-ttu-id="d7b62-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="d7b62-162">streetAddress</span></span>|<span data-ttu-id="d7b62-163">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-163">String</span></span>||
|<span data-ttu-id="d7b62-164">surname</span><span class="sxs-lookup"><span data-stu-id="d7b62-164">surname</span></span>|<span data-ttu-id="d7b62-165">String</span><span class="sxs-lookup"><span data-stu-id="d7b62-165">String</span></span>||
|<span data-ttu-id="d7b62-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="d7b62-166">businessPhones</span></span>|<span data-ttu-id="d7b62-167">String collection</span><span class="sxs-lookup"><span data-stu-id="d7b62-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="d7b62-168">响应</span><span class="sxs-lookup"><span data-stu-id="d7b62-168">Response</span></span>

<span data-ttu-id="d7b62-169">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[orgContact](../resources/orgcontact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7b62-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7b62-170">示例</span><span class="sxs-lookup"><span data-stu-id="d7b62-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7b62-171">请求</span><span class="sxs-lookup"><span data-stu-id="d7b62-171">Request</span></span>
<span data-ttu-id="d7b62-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7b62-172">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d7b62-173">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d7b62-173">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7b62-174">C#</span><span class="sxs-lookup"><span data-stu-id="d7b62-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7b62-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="d7b62-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7b62-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="d7b62-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d7b62-177">Java</span><span class="sxs-lookup"><span data-stu-id="d7b62-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d7b62-178">响应</span><span class="sxs-lookup"><span data-stu-id="d7b62-178">Response</span></span>
<span data-ttu-id="d7b62-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7b62-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
