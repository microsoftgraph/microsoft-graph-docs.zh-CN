---
title: 更新 orgcontact
description: 更新 orgcontact 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ab7064a899fcb4aba051dd0aa0046fc0aee9ecd2
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657103"
---
# <a name="update-orgcontact"></a><span data-ttu-id="40ec3-103">更新 orgcontact</span><span class="sxs-lookup"><span data-stu-id="40ec3-103">Update orgcontact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40ec3-104">更新 orgcontact 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="40ec3-104">Update the properties of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="40ec3-105">权限</span><span class="sxs-lookup"><span data-stu-id="40ec3-105">Permissions</span></span>
<span data-ttu-id="40ec3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40ec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ec3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="40ec3-108">Permission type</span></span>      | <span data-ttu-id="40ec3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40ec3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40ec3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40ec3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="40ec3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="40ec3-111">Not supported.</span></span>    |
|<span data-ttu-id="40ec3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40ec3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40ec3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="40ec3-113">Not supported.</span></span>    |
|<span data-ttu-id="40ec3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="40ec3-114">Application</span></span> | <span data-ttu-id="40ec3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="40ec3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40ec3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40ec3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="40ec3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="40ec3-117">Request headers</span></span>
| <span data-ttu-id="40ec3-118">名称</span><span class="sxs-lookup"><span data-stu-id="40ec3-118">Name</span></span>       | <span data-ttu-id="40ec3-119">类型</span><span class="sxs-lookup"><span data-stu-id="40ec3-119">Type</span></span> | <span data-ttu-id="40ec3-120">说明</span><span class="sxs-lookup"><span data-stu-id="40ec3-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="40ec3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="40ec3-121">Authorization</span></span>  | <span data-ttu-id="40ec3-122">string</span><span class="sxs-lookup"><span data-stu-id="40ec3-122">string</span></span>  | <span data-ttu-id="40ec3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40ec3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40ec3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="40ec3-125">Request body</span></span>
<span data-ttu-id="40ec3-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="40ec3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="40ec3-129">属性</span><span class="sxs-lookup"><span data-stu-id="40ec3-129">Property</span></span>     | <span data-ttu-id="40ec3-130">类型</span><span class="sxs-lookup"><span data-stu-id="40ec3-130">Type</span></span>   |<span data-ttu-id="40ec3-131">说明</span><span class="sxs-lookup"><span data-stu-id="40ec3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40ec3-132">city</span><span class="sxs-lookup"><span data-stu-id="40ec3-132">city</span></span>|<span data-ttu-id="40ec3-133">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-133">String</span></span>||
|<span data-ttu-id="40ec3-134">country</span><span class="sxs-lookup"><span data-stu-id="40ec3-134">country</span></span>|<span data-ttu-id="40ec3-135">字符串</span><span class="sxs-lookup"><span data-stu-id="40ec3-135">String</span></span>||
|<span data-ttu-id="40ec3-136">department</span><span class="sxs-lookup"><span data-stu-id="40ec3-136">department</span></span>|<span data-ttu-id="40ec3-137">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-137">String</span></span>||
|<span data-ttu-id="40ec3-138">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="40ec3-138">onPremisesSyncEnabled</span></span>|<span data-ttu-id="40ec3-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="40ec3-139">Boolean</span></span>||
|<span data-ttu-id="40ec3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="40ec3-140">displayName</span></span>|<span data-ttu-id="40ec3-141">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-141">String</span></span>||
|<span data-ttu-id="40ec3-142">givenName</span><span class="sxs-lookup"><span data-stu-id="40ec3-142">givenName</span></span>|<span data-ttu-id="40ec3-143">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-143">String</span></span>||
|<span data-ttu-id="40ec3-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="40ec3-144">jobTitle</span></span>|<span data-ttu-id="40ec3-145">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-145">String</span></span>||
|<span data-ttu-id="40ec3-146">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="40ec3-146">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="40ec3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40ec3-147">DateTimeOffset</span></span>||
|<span data-ttu-id="40ec3-148">mail</span><span class="sxs-lookup"><span data-stu-id="40ec3-148">mail</span></span>|<span data-ttu-id="40ec3-149">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-149">String</span></span>||
|<span data-ttu-id="40ec3-150">mailNickname</span><span class="sxs-lookup"><span data-stu-id="40ec3-150">mailNickname</span></span>|<span data-ttu-id="40ec3-151">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-151">String</span></span>||
|<span data-ttu-id="40ec3-152">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="40ec3-152">mobilePhone</span></span>|<span data-ttu-id="40ec3-153">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-153">String</span></span>||
|<span data-ttu-id="40ec3-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="40ec3-154">officeLocation</span></span>|<span data-ttu-id="40ec3-155">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-155">String</span></span>||
|<span data-ttu-id="40ec3-156">postalCode</span><span class="sxs-lookup"><span data-stu-id="40ec3-156">postalCode</span></span>|<span data-ttu-id="40ec3-157">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-157">String</span></span>||
|<span data-ttu-id="40ec3-158">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="40ec3-158">proxyAddresses</span></span>|<span data-ttu-id="40ec3-159">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-159">String</span></span>||
|<span data-ttu-id="40ec3-160">state</span><span class="sxs-lookup"><span data-stu-id="40ec3-160">state</span></span>|<span data-ttu-id="40ec3-161">字符串</span><span class="sxs-lookup"><span data-stu-id="40ec3-161">String</span></span>||
|<span data-ttu-id="40ec3-162">streetAddress</span><span class="sxs-lookup"><span data-stu-id="40ec3-162">streetAddress</span></span>|<span data-ttu-id="40ec3-163">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-163">String</span></span>||
|<span data-ttu-id="40ec3-164">surname</span><span class="sxs-lookup"><span data-stu-id="40ec3-164">surname</span></span>|<span data-ttu-id="40ec3-165">String</span><span class="sxs-lookup"><span data-stu-id="40ec3-165">String</span></span>||
|<span data-ttu-id="40ec3-166">businessPhones</span><span class="sxs-lookup"><span data-stu-id="40ec3-166">businessPhones</span></span>|<span data-ttu-id="40ec3-167">String collection</span><span class="sxs-lookup"><span data-stu-id="40ec3-167">String collection</span></span>||

## <a name="response"></a><span data-ttu-id="40ec3-168">响应</span><span class="sxs-lookup"><span data-stu-id="40ec3-168">Response</span></span>

<span data-ttu-id="40ec3-169">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[orgContact](../resources/orgcontact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="40ec3-169">If successful, this method returns a `200 OK` response code and updated [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40ec3-170">示例</span><span class="sxs-lookup"><span data-stu-id="40ec3-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="40ec3-171">请求</span><span class="sxs-lookup"><span data-stu-id="40ec3-171">Request</span></span>
<span data-ttu-id="40ec3-172">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40ec3-172">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="40ec3-173">响应</span><span class="sxs-lookup"><span data-stu-id="40ec3-173">Response</span></span>
<span data-ttu-id="40ec3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40ec3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="40ec3-177">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="40ec3-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="40ec3-178">C#</span><span class="sxs-lookup"><span data-stu-id="40ec3-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_orgcontact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40ec3-179">Javascript</span><span class="sxs-lookup"><span data-stu-id="40ec3-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_orgcontact-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/orgcontact-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
