---
title: 更新 countryNamedlocation
description: 更新 countryNamedLocation 对象的属性。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e5c73b039ec2939505367d4faad9a34f332b3c12
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567091"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="735ab-103">更新 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="735ab-103">Update countryNamedLocation</span></span>

<span data-ttu-id="735ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="735ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="735ab-105">更新[countryNamedLocation](../resources/countryNamedLocation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="735ab-105">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="735ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="735ab-106">Permissions</span></span>

<span data-ttu-id="735ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="735ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="735ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="735ab-109">Permission type</span></span>                        | <span data-ttu-id="735ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="735ab-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="735ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="735ab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="735ab-112">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="735ab-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="735ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="735ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="735ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="735ab-114">Not supported.</span></span> |
| <span data-ttu-id="735ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="735ab-115">Application</span></span>                            | <span data-ttu-id="735ab-116">Policy。 Read. All 和 ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="735ab-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="735ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="735ab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="735ab-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="735ab-118">Request headers</span></span>

| <span data-ttu-id="735ab-119">名称</span><span class="sxs-lookup"><span data-stu-id="735ab-119">Name</span></span>       | <span data-ttu-id="735ab-120">说明</span><span class="sxs-lookup"><span data-stu-id="735ab-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="735ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="735ab-121">Authorization</span></span> | <span data-ttu-id="735ab-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="735ab-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="735ab-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="735ab-124">Content-type</span></span>  | <span data-ttu-id="735ab-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="735ab-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="735ab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="735ab-127">Request body</span></span>

<span data-ttu-id="735ab-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="735ab-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="735ab-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="735ab-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="735ab-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="735ab-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="735ab-131">属性</span><span class="sxs-lookup"><span data-stu-id="735ab-131">Property</span></span>     | <span data-ttu-id="735ab-132">类型</span><span class="sxs-lookup"><span data-stu-id="735ab-132">Type</span></span>        | <span data-ttu-id="735ab-133">说明</span><span class="sxs-lookup"><span data-stu-id="735ab-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="735ab-134">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="735ab-134">countriesAndRegions</span></span>|<span data-ttu-id="735ab-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="735ab-135">String collection</span></span>|<span data-ttu-id="735ab-136">由 ISO 3166-2 指定的两个字母格式的国家/地区和/或地区列表。</span><span class="sxs-lookup"><span data-stu-id="735ab-136">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="735ab-137">displayName</span><span class="sxs-lookup"><span data-stu-id="735ab-137">displayName</span></span>|<span data-ttu-id="735ab-138">String</span><span class="sxs-lookup"><span data-stu-id="735ab-138">String</span></span>|<span data-ttu-id="735ab-139">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="735ab-139">Human-readable name of the location.</span></span>|
|<span data-ttu-id="735ab-140">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="735ab-140">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="735ab-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="735ab-141">Boolean</span></span>|<span data-ttu-id="735ab-142">值是 `true` 如果未映射到国家或地区的 IP 地址应包含在指定的位置。</span><span class="sxs-lookup"><span data-stu-id="735ab-142">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="735ab-143">响应</span><span class="sxs-lookup"><span data-stu-id="735ab-143">Response</span></span>

<span data-ttu-id="735ab-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="735ab-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="735ab-146">示例</span><span class="sxs-lookup"><span data-stu-id="735ab-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="735ab-147">请求</span><span class="sxs-lookup"><span data-stu-id="735ab-147">Request</span></span>

<span data-ttu-id="735ab-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="735ab-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="735ab-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="735ab-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
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
# <a name="c"></a>[<span data-ttu-id="735ab-150">C#</span><span class="sxs-lookup"><span data-stu-id="735ab-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="735ab-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="735ab-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="735ab-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="735ab-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="735ab-153">Java</span><span class="sxs-lookup"><span data-stu-id="735ab-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-countrynamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="735ab-154">响应</span><span class="sxs-lookup"><span data-stu-id="735ab-154">Response</span></span>

<span data-ttu-id="735ab-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="735ab-155">The following is an example of the response.</span></span>

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
