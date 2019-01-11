---
title: 更新图标
description: 更新 icon 对象的属性。
localization_priority: Normal
ms.openlocfilehash: 83e9845e87018a6f7b059a917643c1c51ccd01d5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859176"
---
# <a name="update-icon"></a><span data-ttu-id="22008-103">更新图标</span><span class="sxs-lookup"><span data-stu-id="22008-103">Update icon</span></span>

> <span data-ttu-id="22008-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="22008-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22008-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="22008-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22008-106">更新 icon 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="22008-106">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="22008-107">权限</span><span class="sxs-lookup"><span data-stu-id="22008-107">Permissions</span></span>
<span data-ttu-id="22008-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22008-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22008-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="22008-110">Permission type</span></span>      | <span data-ttu-id="22008-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22008-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22008-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22008-112">Delegated (work or school account)</span></span> | <span data-ttu-id="22008-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22008-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="22008-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22008-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22008-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22008-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="22008-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="22008-116">Application</span></span> | <span data-ttu-id="22008-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="22008-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22008-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22008-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="22008-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="22008-119">Optional request headers</span></span>
| <span data-ttu-id="22008-120">名称</span><span class="sxs-lookup"><span data-stu-id="22008-120">Name</span></span>       | <span data-ttu-id="22008-121">说明</span><span class="sxs-lookup"><span data-stu-id="22008-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="22008-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22008-122">Authorization</span></span>  | <span data-ttu-id="22008-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22008-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22008-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="22008-125">Request body</span></span>
<span data-ttu-id="22008-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="22008-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="22008-129">属性</span><span class="sxs-lookup"><span data-stu-id="22008-129">Property</span></span>     | <span data-ttu-id="22008-130">类型</span><span class="sxs-lookup"><span data-stu-id="22008-130">Type</span></span>   |<span data-ttu-id="22008-131">说明</span><span class="sxs-lookup"><span data-stu-id="22008-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22008-132">index</span><span class="sxs-lookup"><span data-stu-id="22008-132">index</span></span>|<span data-ttu-id="22008-133">int</span><span class="sxs-lookup"><span data-stu-id="22008-133">int</span></span>|<span data-ttu-id="22008-134">表示给定集合中图标的索引。</span><span class="sxs-lookup"><span data-stu-id="22008-134">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="22008-135">set</span><span class="sxs-lookup"><span data-stu-id="22008-135">set</span></span>|<span data-ttu-id="22008-136">string</span><span class="sxs-lookup"><span data-stu-id="22008-136">string</span></span>|<span data-ttu-id="22008-p105">表示图标所属的集合。可能的值是：`Invalid`、`ThreeArrows`、`ThreeArrowsGray`、`ThreeFlags`、`ThreeTrafficLights1`、`ThreeTrafficLights2`、`ThreeSigns`、`ThreeSymbols`、`ThreeSymbols2`、`FourArrows`、`FourArrowsGray`、`FourRedToBlack`、`FourRating`、`FourTrafficLights`、`FiveArrows`、`FiveArrowsGray`、`FiveRating`、`FiveQuarters`、`ThreeStars`、`ThreeTriangles``FiveBoxes`。</span><span class="sxs-lookup"><span data-stu-id="22008-p105">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="22008-139">响应</span><span class="sxs-lookup"><span data-stu-id="22008-139">Response</span></span>

<span data-ttu-id="22008-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [Icon](../resources/icon.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22008-140">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="22008-141">示例</span><span class="sxs-lookup"><span data-stu-id="22008-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22008-142">请求</span><span class="sxs-lookup"><span data-stu-id="22008-142">Request</span></span>
<span data-ttu-id="22008-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="22008-143">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="22008-144">响应</span><span class="sxs-lookup"><span data-stu-id="22008-144">Response</span></span>
<span data-ttu-id="22008-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="22008-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
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
