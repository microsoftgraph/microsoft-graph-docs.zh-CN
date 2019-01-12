---
title: Range:UsedRange
description: 返回指定 range 对象的所用范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 0ae8f8bec1eea6f2e13b4c4248d55afbb28cf19d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928064"
---
# <a name="range-usedrange"></a><span data-ttu-id="c2b93-103">Range:UsedRange</span><span class="sxs-lookup"><span data-stu-id="c2b93-103">Range: UsedRange</span></span>

> <span data-ttu-id="c2b93-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c2b93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2b93-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c2b93-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2b93-106">返回指定 range 对象的所用范围。</span><span class="sxs-lookup"><span data-stu-id="c2b93-106">Returns the used range of the given range object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2b93-107">权限</span><span class="sxs-lookup"><span data-stu-id="c2b93-107">Permissions</span></span>
<span data-ttu-id="c2b93-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2b93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2b93-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2b93-110">Permission type</span></span>      | <span data-ttu-id="c2b93-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2b93-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2b93-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2b93-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c2b93-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2b93-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c2b93-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2b93-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2b93-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2b93-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c2b93-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2b93-116">Application</span></span> | <span data-ttu-id="c2b93-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2b93-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2b93-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2b93-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/UsedRange
GET /workbook/worksheets/{id|name}/range(address='<address>')/UsedRange
GET /workbook/tables/{id|name}/columns/{id|name}/range/UsedRange

```
## <a name="request-headers"></a><span data-ttu-id="c2b93-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2b93-119">Request headers</span></span>
| <span data-ttu-id="c2b93-120">名称</span><span class="sxs-lookup"><span data-stu-id="c2b93-120">Name</span></span>       | <span data-ttu-id="c2b93-121">说明</span><span class="sxs-lookup"><span data-stu-id="c2b93-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c2b93-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2b93-122">Authorization</span></span>  | <span data-ttu-id="c2b93-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2b93-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c2b93-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c2b93-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="c2b93-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c2b93-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2b93-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2b93-128">Request body</span></span>
<span data-ttu-id="c2b93-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c2b93-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c2b93-130">参数</span><span class="sxs-lookup"><span data-stu-id="c2b93-130">Parameter</span></span>    | <span data-ttu-id="c2b93-131">类型</span><span class="sxs-lookup"><span data-stu-id="c2b93-131">Type</span></span>   |<span data-ttu-id="c2b93-132">说明</span><span class="sxs-lookup"><span data-stu-id="c2b93-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2b93-133">valuesOnly</span><span class="sxs-lookup"><span data-stu-id="c2b93-133">valuesOnly</span></span>|<span data-ttu-id="c2b93-134">boolean</span><span class="sxs-lookup"><span data-stu-id="c2b93-134">boolean</span></span>|<span data-ttu-id="c2b93-p105">可选。仅将有值的单元格视为已使用的单元格。</span><span class="sxs-lookup"><span data-stu-id="c2b93-p105">Optional. Considers only cells with values as used cells.</span></span>|

## <a name="response"></a><span data-ttu-id="c2b93-137">响应</span><span class="sxs-lookup"><span data-stu-id="c2b93-137">Response</span></span>

<span data-ttu-id="c2b93-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c2b93-138">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2b93-139">示例</span><span class="sxs-lookup"><span data-stu-id="c2b93-139">Example</span></span>
<span data-ttu-id="c2b93-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c2b93-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c2b93-141">请求</span><span class="sxs-lookup"><span data-stu-id="c2b93-141">Request</span></span>
<span data-ttu-id="c2b93-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2b93-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_usedrange"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/UsedRange
Content-type: application/json
Content-length: 24

{
  "valuesOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="c2b93-143">响应</span><span class="sxs-lookup"><span data-stu-id="c2b93-143">Response</span></span>
<span data-ttu-id="c2b93-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2b93-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnIndex": 99,
  "valueTypes": "valueTypes-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: UsedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
