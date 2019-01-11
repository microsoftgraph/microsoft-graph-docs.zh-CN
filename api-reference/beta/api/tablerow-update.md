---
title: 更新 tablerow
description: 更新 tablerow 对象的属性。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c1a1cc51a6f148127a446dcbcfa8c9573db24ade
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868318"
---
# <a name="update-tablerow"></a><span data-ttu-id="112e0-103">更新 tablerow</span><span class="sxs-lookup"><span data-stu-id="112e0-103">Update tablerow</span></span>

> <span data-ttu-id="112e0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="112e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="112e0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="112e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="112e0-106">更新 tablerow 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="112e0-106">Update the properties of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="112e0-107">权限</span><span class="sxs-lookup"><span data-stu-id="112e0-107">Permissions</span></span>
<span data-ttu-id="112e0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="112e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="112e0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="112e0-110">Permission type</span></span>      | <span data-ttu-id="112e0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="112e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="112e0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="112e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="112e0-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="112e0-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="112e0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="112e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="112e0-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="112e0-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="112e0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="112e0-116">Application</span></span> | <span data-ttu-id="112e0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="112e0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="112e0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="112e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/rows(<index>)
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="112e0-119">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="112e0-119">Optional request headers</span></span>
| <span data-ttu-id="112e0-120">名称</span><span class="sxs-lookup"><span data-stu-id="112e0-120">Name</span></span>       | <span data-ttu-id="112e0-121">说明</span><span class="sxs-lookup"><span data-stu-id="112e0-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="112e0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="112e0-122">Authorization</span></span>  | <span data-ttu-id="112e0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="112e0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="112e0-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="112e0-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="112e0-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="112e0-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="112e0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="112e0-128">Request body</span></span>
<span data-ttu-id="112e0-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="112e0-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="112e0-132">属性</span><span class="sxs-lookup"><span data-stu-id="112e0-132">Property</span></span>     | <span data-ttu-id="112e0-133">类型</span><span class="sxs-lookup"><span data-stu-id="112e0-133">Type</span></span>   |<span data-ttu-id="112e0-134">说明</span><span class="sxs-lookup"><span data-stu-id="112e0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="112e0-135">values</span><span class="sxs-lookup"><span data-stu-id="112e0-135">values</span></span>|<span data-ttu-id="112e0-136">json</span><span class="sxs-lookup"><span data-stu-id="112e0-136">json</span></span>|<span data-ttu-id="112e0-p106">表示指定区域的原始值。返回的数据类型可能是字符串、数字或布尔值。包含一个将返回错误字符串的错误的单元格。</span><span class="sxs-lookup"><span data-stu-id="112e0-p106">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="response"></a><span data-ttu-id="112e0-140">响应</span><span class="sxs-lookup"><span data-stu-id="112e0-140">Response</span></span>

<span data-ttu-id="112e0-141">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [TableRow](../resources/tablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="112e0-141">If successful, this method returns a `200 OK` response code and updated [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="112e0-142">示例</span><span class="sxs-lookup"><span data-stu-id="112e0-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="112e0-143">请求</span><span class="sxs-lookup"><span data-stu-id="112e0-143">Request</span></span>
<span data-ttu-id="112e0-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="112e0-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_tablerow"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```
##### <a name="response"></a><span data-ttu-id="112e0-145">响应</span><span class="sxs-lookup"><span data-stu-id="112e0-145">Response</span></span>
<span data-ttu-id="112e0-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="112e0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tablerow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
