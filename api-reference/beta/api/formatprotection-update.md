---
title: 更新 formatProtection
description: 更新 formatprotection 对象的属性。
ms.openlocfilehash: 7a75af3b340b194df16a53dd7800d5d6981730ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044961"
---
# <a name="update-formatprotection"></a><span data-ttu-id="be2d3-103">更新 formatProtection</span><span class="sxs-lookup"><span data-stu-id="be2d3-103">Update formatprotection</span></span>

> <span data-ttu-id="be2d3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="be2d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="be2d3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="be2d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="be2d3-106">更新 formatprotection 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="be2d3-106">Update the properties of formatprotection object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be2d3-107">权限</span><span class="sxs-lookup"><span data-stu-id="be2d3-107">Permissions</span></span>
<span data-ttu-id="be2d3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="be2d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be2d3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="be2d3-110">Permission type</span></span>      | <span data-ttu-id="be2d3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="be2d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be2d3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="be2d3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="be2d3-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be2d3-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be2d3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="be2d3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be2d3-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be2d3-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="be2d3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="be2d3-116">Application</span></span> | <span data-ttu-id="be2d3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="be2d3-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be2d3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="be2d3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/protection
PATCH /workbook/worksheets/{id|name}/range(<address>)/format/protection
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/protection
```
## <a name="optional-request-headers"></a><span data-ttu-id="be2d3-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="be2d3-119">Optional request headers</span></span>
| <span data-ttu-id="be2d3-120">名称</span><span class="sxs-lookup"><span data-stu-id="be2d3-120">Name</span></span>       | <span data-ttu-id="be2d3-121">说明</span><span class="sxs-lookup"><span data-stu-id="be2d3-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="be2d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="be2d3-122">Authorization</span></span>  | <span data-ttu-id="be2d3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="be2d3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be2d3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="be2d3-125">Request body</span></span>
<span data-ttu-id="be2d3-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="be2d3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="be2d3-129">属性</span><span class="sxs-lookup"><span data-stu-id="be2d3-129">Property</span></span>     | <span data-ttu-id="be2d3-130">类型</span><span class="sxs-lookup"><span data-stu-id="be2d3-130">Type</span></span>   |<span data-ttu-id="be2d3-131">说明</span><span class="sxs-lookup"><span data-stu-id="be2d3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be2d3-132">formulaHidden</span><span class="sxs-lookup"><span data-stu-id="be2d3-132">formulaHidden</span></span>|<span data-ttu-id="be2d3-133">boolean</span><span class="sxs-lookup"><span data-stu-id="be2d3-133">boolean</span></span>|<span data-ttu-id="be2d3-p105">表示 Excel 是否隐藏区域中的单元格公式。指示整个区域不具有统一公式隐藏设置的空值。</span><span class="sxs-lookup"><span data-stu-id="be2d3-p105">Indicates if Excel hides the formula for the cells in the range. A null value indicates that the entire range doesn't have uniform formula hidden setting.</span></span>|
|<span data-ttu-id="be2d3-136">已锁定</span><span class="sxs-lookup"><span data-stu-id="be2d3-136">locked</span></span>|<span data-ttu-id="be2d3-137">boolean</span><span class="sxs-lookup"><span data-stu-id="be2d3-137">boolean</span></span>|<span data-ttu-id="be2d3-p106">指示 Excel 是否锁定对象中的单元格。指示整个区域不具有统一锁定设置的空值。</span><span class="sxs-lookup"><span data-stu-id="be2d3-p106">Indicates if Excel locks the cells in the object. A null value indicates that the entire range doesn't have uniform lock setting.</span></span>|

## <a name="response"></a><span data-ttu-id="be2d3-140">响应</span><span class="sxs-lookup"><span data-stu-id="be2d3-140">Response</span></span>

<span data-ttu-id="be2d3-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [FormatProtection](../resources/formatprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be2d3-141">If successful, this method returns a `200 OK` response code and updated [FormatProtection](../resources/formatprotection.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be2d3-142">示例</span><span class="sxs-lookup"><span data-stu-id="be2d3-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be2d3-143">请求</span><span class="sxs-lookup"><span data-stu-id="be2d3-143">Request</span></span>
<span data-ttu-id="be2d3-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="be2d3-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_formatprotection"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/protection
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```
##### <a name="response"></a><span data-ttu-id="be2d3-145">响应</span><span class="sxs-lookup"><span data-stu-id="be2d3-145">Response</span></span>
<span data-ttu-id="be2d3-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="be2d3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.formatProtection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "locked": true,
  "formulaHidden": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update formatprotection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->