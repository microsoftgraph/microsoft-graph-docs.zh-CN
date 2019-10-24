---
title: 更新 countryNamedlocation
description: 更新 countryNamedLocation 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d68138088ed39d8c4fe4dfbcec7abcb77aa11dd3
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653739"
---
# <a name="update-countrynamedlocation"></a><span data-ttu-id="7c936-103">更新 countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="7c936-103">Update countryNamedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c936-104">更新[countryNamedLocation](../resources/countryNamedLocation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7c936-104">Update the properties of a [countryNamedLocation](../resources/countryNamedLocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c936-105">权限</span><span class="sxs-lookup"><span data-stu-id="7c936-105">Permissions</span></span>

<span data-ttu-id="7c936-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c936-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c936-108">Permission type</span></span>                        | <span data-ttu-id="7c936-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c936-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7c936-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c936-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c936-111">ConditionalAccess 和 Directory.accessasuser.all 的所有</span><span class="sxs-lookup"><span data-stu-id="7c936-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="7c936-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c936-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c936-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c936-113">Not supported.</span></span> |
| <span data-ttu-id="7c936-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c936-114">Application</span></span>                            | <span data-ttu-id="7c936-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c936-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="7c936-116">此 API 需要多个权限。</span><span class="sxs-lookup"><span data-stu-id="7c936-116">This API requires multiple permissions.</span></span> <span data-ttu-id="7c936-117">有关详细信息，请参阅[已知问题](/graph/known-issues#conditional-access-policies-and-named-locations)。</span><span class="sxs-lookup"><span data-stu-id="7c936-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="7c936-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c936-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7c936-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c936-119">Request headers</span></span>

| <span data-ttu-id="7c936-120">名称</span><span class="sxs-lookup"><span data-stu-id="7c936-120">Name</span></span>       | <span data-ttu-id="7c936-121">说明</span><span class="sxs-lookup"><span data-stu-id="7c936-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7c936-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c936-122">Authorization</span></span> | <span data-ttu-id="7c936-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c936-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7c936-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="7c936-125">Content-type</span></span>  | <span data-ttu-id="7c936-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7c936-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c936-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c936-128">Request body</span></span>

<span data-ttu-id="7c936-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="7c936-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="7c936-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="7c936-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7c936-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="7c936-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7c936-132">属性</span><span class="sxs-lookup"><span data-stu-id="7c936-132">Property</span></span>     | <span data-ttu-id="7c936-133">类型</span><span class="sxs-lookup"><span data-stu-id="7c936-133">Type</span></span>        | <span data-ttu-id="7c936-134">说明</span><span class="sxs-lookup"><span data-stu-id="7c936-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c936-135">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="7c936-135">countriesAndRegions</span></span>|<span data-ttu-id="7c936-136">String collection</span><span class="sxs-lookup"><span data-stu-id="7c936-136">String collection</span></span>|<span data-ttu-id="7c936-137">由 ISO 3166-2 指定的两个字母格式的国家/地区和/或地区列表。</span><span class="sxs-lookup"><span data-stu-id="7c936-137">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="7c936-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7c936-138">displayName</span></span>|<span data-ttu-id="7c936-139">String</span><span class="sxs-lookup"><span data-stu-id="7c936-139">String</span></span>|<span data-ttu-id="7c936-140">位置的人可读名称。</span><span class="sxs-lookup"><span data-stu-id="7c936-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="7c936-141">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="7c936-141">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="7c936-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c936-142">Boolean</span></span>|<span data-ttu-id="7c936-143">值是`true`如果未映射到国家或地区的 IP 地址应包含在指定的位置。</span><span class="sxs-lookup"><span data-stu-id="7c936-143">The value is `true` if IP addresses that don't map to a country or region should be included in the named location.</span></span>|

## <a name="response"></a><span data-ttu-id="7c936-144">响应</span><span class="sxs-lookup"><span data-stu-id="7c936-144">Response</span></span>

<span data-ttu-id="7c936-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7c936-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c936-147">示例</span><span class="sxs-lookup"><span data-stu-id="7c936-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c936-148">请求</span><span class="sxs-lookup"><span data-stu-id="7c936-148">Request</span></span>

<span data-ttu-id="7c936-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c936-149">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c936-150">响应</span><span class="sxs-lookup"><span data-stu-id="7c936-150">Response</span></span>

<span data-ttu-id="7c936-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7c936-151">The following is an example of the response.</span></span>

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
