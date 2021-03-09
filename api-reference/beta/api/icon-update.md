---
title: 更新图标
description: 更新 icon 对象的属性。
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: d9a89b4ed1c07d172c9e3b8d41b2296f781467c3
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574011"
---
# <a name="update-icon"></a><span data-ttu-id="8aa39-103">更新图标</span><span class="sxs-lookup"><span data-stu-id="8aa39-103">Update icon</span></span>

<span data-ttu-id="8aa39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aa39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aa39-105">更新 icon 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8aa39-105">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8aa39-106">权限</span><span class="sxs-lookup"><span data-stu-id="8aa39-106">Permissions</span></span>
<span data-ttu-id="8aa39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8aa39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aa39-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8aa39-109">Permission type</span></span>      | <span data-ttu-id="8aa39-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8aa39-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8aa39-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8aa39-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8aa39-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aa39-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8aa39-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8aa39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aa39-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aa39-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8aa39-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8aa39-115">Application</span></span> | <span data-ttu-id="8aa39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8aa39-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8aa39-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8aa39-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
PATCH /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
PATCH /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="8aa39-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="8aa39-118">Optional request headers</span></span>
| <span data-ttu-id="8aa39-119">名称</span><span class="sxs-lookup"><span data-stu-id="8aa39-119">Name</span></span>       | <span data-ttu-id="8aa39-120">说明</span><span class="sxs-lookup"><span data-stu-id="8aa39-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8aa39-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8aa39-121">Authorization</span></span>  | <span data-ttu-id="8aa39-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8aa39-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8aa39-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8aa39-124">Request body</span></span>
<span data-ttu-id="8aa39-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8aa39-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8aa39-128">属性</span><span class="sxs-lookup"><span data-stu-id="8aa39-128">Property</span></span>     | <span data-ttu-id="8aa39-129">类型</span><span class="sxs-lookup"><span data-stu-id="8aa39-129">Type</span></span>   |<span data-ttu-id="8aa39-130">说明</span><span class="sxs-lookup"><span data-stu-id="8aa39-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8aa39-131">index</span><span class="sxs-lookup"><span data-stu-id="8aa39-131">index</span></span>|<span data-ttu-id="8aa39-132">int</span><span class="sxs-lookup"><span data-stu-id="8aa39-132">int</span></span>|<span data-ttu-id="8aa39-133">表示给定集合中图标的索引。</span><span class="sxs-lookup"><span data-stu-id="8aa39-133">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="8aa39-134">set</span><span class="sxs-lookup"><span data-stu-id="8aa39-134">set</span></span>|<span data-ttu-id="8aa39-135">string</span><span class="sxs-lookup"><span data-stu-id="8aa39-135">string</span></span>|<span data-ttu-id="8aa39-136">表示图标所属的集合。</span><span class="sxs-lookup"><span data-stu-id="8aa39-136">Represents the set that the icon is part of.</span></span> <span data-ttu-id="8aa39-137">可取值为：`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles`、`FiveBoxes`。</span><span class="sxs-lookup"><span data-stu-id="8aa39-137">Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="8aa39-138">响应</span><span class="sxs-lookup"><span data-stu-id="8aa39-138">Response</span></span>

<span data-ttu-id="8aa39-139">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [workbookIcon](../resources/workbookicon.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8aa39-139">If successful, this method returns a `200 OK` response code and updated [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8aa39-140">示例</span><span class="sxs-lookup"><span data-stu-id="8aa39-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8aa39-141">请求</span><span class="sxs-lookup"><span data-stu-id="8aa39-141">Request</span></span>
<span data-ttu-id="8aa39-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8aa39-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="8aa39-143">响应</span><span class="sxs-lookup"><span data-stu-id="8aa39-143">Response</span></span>
<span data-ttu-id="8aa39-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8aa39-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


