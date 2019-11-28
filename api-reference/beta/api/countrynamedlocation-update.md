---
title: 更新 countryNamedlocation
description: 更新 countryNamedLocation 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 81224b2c0e31ad4ade9caeca661624e1b0fe4383
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636741"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="07565-103">更新 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="07565-103">Update countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07565-104">更新[countryNamedLocation](../resources/countryNamedLocation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="07565-104">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="07565-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="07565-105">Permissions</span></span>

<span data-ttu-id="07565-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07565-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07565-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="07565-108">Permission type</span></span>                        | <span data-ttu-id="07565-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07565-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="07565-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07565-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="07565-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="07565-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="07565-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07565-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07565-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="07565-113">Not supported.</span></span> |
| <span data-ttu-id="07565-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="07565-114">Application</span></span>                            | <span data-ttu-id="07565-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="07565-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="07565-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07565-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="07565-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="07565-117">Request headers</span></span>

| <span data-ttu-id="07565-118">名称</span><span class="sxs-lookup"><span data-stu-id="07565-118">Name</span></span>       | <span data-ttu-id="07565-119">说明</span><span class="sxs-lookup"><span data-stu-id="07565-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="07565-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="07565-120">Authorization</span></span> | <span data-ttu-id="07565-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07565-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="07565-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="07565-123">Content-type</span></span>  | <span data-ttu-id="07565-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="07565-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07565-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="07565-126">Request body</span></span>

<span data-ttu-id="07565-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="07565-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="07565-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="07565-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="07565-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="07565-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="07565-130">属性</span><span class="sxs-lookup"><span data-stu-id="07565-130">Property</span></span>     | <span data-ttu-id="07565-131">类型</span><span class="sxs-lookup"><span data-stu-id="07565-131">Type</span></span>        | <span data-ttu-id="07565-132">说明</span><span class="sxs-lookup"><span data-stu-id="07565-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07565-133">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="07565-133">countriesAndRegions</span></span>|<span data-ttu-id="07565-134">String collection</span><span class="sxs-lookup"><span data-stu-id="07565-134">String collection</span></span>|<span data-ttu-id="07565-135">由 ISO 3166-2 指定的两个字母格式的国家/地区和/或地区列表。</span><span class="sxs-lookup"><span data-stu-id="07565-135">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="07565-136">displayName</span><span class="sxs-lookup"><span data-stu-id="07565-136">displayName</span></span>|<span data-ttu-id="07565-137">String</span><span class="sxs-lookup"><span data-stu-id="07565-137">String</span></span>|<span data-ttu-id="07565-138">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="07565-138">Human-readable name of the location.</span></span>|
|<span data-ttu-id="07565-139">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="07565-139">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="07565-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="07565-140">Boolean</span></span>|<span data-ttu-id="07565-141">值是`true`如果未映射到国家或地区的 IP 地址应包含在指定的位置。</span><span class="sxs-lookup"><span data-stu-id="07565-141">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="07565-142">响应</span><span class="sxs-lookup"><span data-stu-id="07565-142">Response</span></span>

<span data-ttu-id="07565-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="07565-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="07565-145">示例</span><span class="sxs-lookup"><span data-stu-id="07565-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="07565-146">请求</span><span class="sxs-lookup"><span data-stu-id="07565-146">Request</span></span>

<span data-ttu-id="07565-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07565-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="07565-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="07565-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "displayName": "Updated named location without unknown countries and regions",
    "countriesAndRegions": [
        "CA",
        "IN"
    ],
    "includeUnknownCountriesAndRegions": false
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07565-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07565-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="07565-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07565-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="07565-151">响应</span><span class="sxs-lookup"><span data-stu-id="07565-151">Response</span></span>

<span data-ttu-id="07565-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="07565-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update countrynamedlocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
