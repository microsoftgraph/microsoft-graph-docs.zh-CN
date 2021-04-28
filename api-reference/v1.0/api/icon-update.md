---
title: 更新图标
description: 更新 icon 对象的属性。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 619502932eddf6e70e3b35e1532a44ed642bb891
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053991"
---
# <a name="update-icon"></a><span data-ttu-id="3e62a-103">更新图标</span><span class="sxs-lookup"><span data-stu-id="3e62a-103">Update icon</span></span>

<span data-ttu-id="3e62a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e62a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3e62a-105">更新 icon 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3e62a-105">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e62a-106">权限</span><span class="sxs-lookup"><span data-stu-id="3e62a-106">Permissions</span></span>
<span data-ttu-id="3e62a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e62a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e62a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e62a-109">Permission type</span></span>      | <span data-ttu-id="3e62a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e62a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e62a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e62a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3e62a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e62a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e62a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e62a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e62a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e62a-114">Not supported.</span></span>    |
|<span data-ttu-id="3e62a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e62a-115">Application</span></span> | <span data-ttu-id="3e62a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e62a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e62a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e62a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="3e62a-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="3e62a-118">Optional request headers</span></span>
| <span data-ttu-id="3e62a-119">名称</span><span class="sxs-lookup"><span data-stu-id="3e62a-119">Name</span></span>       | <span data-ttu-id="3e62a-120">说明</span><span class="sxs-lookup"><span data-stu-id="3e62a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="3e62a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e62a-121">Authorization</span></span>  | <span data-ttu-id="3e62a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e62a-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3e62a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e62a-124">Request body</span></span>
<span data-ttu-id="3e62a-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="3e62a-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="3e62a-128">属性</span><span class="sxs-lookup"><span data-stu-id="3e62a-128">Property</span></span>     | <span data-ttu-id="3e62a-129">类型</span><span class="sxs-lookup"><span data-stu-id="3e62a-129">Type</span></span>   |<span data-ttu-id="3e62a-130">说明</span><span class="sxs-lookup"><span data-stu-id="3e62a-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e62a-131">index</span><span class="sxs-lookup"><span data-stu-id="3e62a-131">index</span></span>|<span data-ttu-id="3e62a-132">int</span><span class="sxs-lookup"><span data-stu-id="3e62a-132">int</span></span>|<span data-ttu-id="3e62a-133">表示给定集合中图标的索引。</span><span class="sxs-lookup"><span data-stu-id="3e62a-133">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="3e62a-134">set</span><span class="sxs-lookup"><span data-stu-id="3e62a-134">set</span></span>|<span data-ttu-id="3e62a-135">string</span><span class="sxs-lookup"><span data-stu-id="3e62a-135">string</span></span>|<span data-ttu-id="3e62a-136">表示图标所属的集合。</span><span class="sxs-lookup"><span data-stu-id="3e62a-136">Represents the set that the icon is part of.</span></span> <span data-ttu-id="3e62a-137">可能的值是：、 `Invalid` `ThreeArrows` `ThreeArrowsGray` `ThreeFlags` `ThreeTrafficLights1` `ThreeTrafficLights2` `ThreeSigns` `ThreeSymbols` `ThreeSymbols2` `FourArrows` `FourArrowsGray` `FourRedToBlack` `FourRating` `FourTrafficLights` `FiveArrows` `FiveArrowsGray` `FiveRating` `FiveQuarters` `ThreeStars` `ThreeTriangles` `FiveBoxes` 。</span><span class="sxs-lookup"><span data-stu-id="3e62a-137">The possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="3e62a-138">响应</span><span class="sxs-lookup"><span data-stu-id="3e62a-138">Response</span></span>

<span data-ttu-id="3e62a-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Icon](../resources/icon.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e62a-139">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e62a-140">示例</span><span class="sxs-lookup"><span data-stu-id="3e62a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e62a-141">请求</span><span class="sxs-lookup"><span data-stu-id="3e62a-141">Request</span></span>
<span data-ttu-id="3e62a-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e62a-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="3e62a-143">响应</span><span class="sxs-lookup"><span data-stu-id="3e62a-143">Response</span></span>
<span data-ttu-id="3e62a-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3e62a-144">Here is an example of the response.</span></span> <span data-ttu-id="3e62a-145">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3e62a-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

