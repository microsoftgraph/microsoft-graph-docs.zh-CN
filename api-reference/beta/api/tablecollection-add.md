---
title: 'TableCollection: add'
description: 创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: ba339cd0d3be6c46d9280b19e774f2a0062f616b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335543"
---
# <a name="tablecollection-add"></a><span data-ttu-id="ec05d-105">TableCollection: add</span><span class="sxs-lookup"><span data-stu-id="ec05d-105">TableCollection: add</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec05d-p102">创建一个新表。区域源地址确定将在其下添加表的工作表。如果无法添加表（例如，由于地址无效，或者表与另一个表重叠），将抛出错误。</span><span class="sxs-lookup"><span data-stu-id="ec05d-p102">Create a new table. The range source address determines the worksheet under which the table will be added. If the table cannot be added (e.g., because the address is invalid, or the table would overlap with another table), an error will be thrown.</span></span>

## <a name="error-handling"></a><span data-ttu-id="ec05d-109">错误处理</span><span class="sxs-lookup"><span data-stu-id="ec05d-109">Error Handling</span></span>

<span data-ttu-id="ec05d-110">此请求有时可能会收到 504 HTTP 错误。</span><span class="sxs-lookup"><span data-stu-id="ec05d-110">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="ec05d-111">此错误的适当响应做法是重复发出请求。</span><span class="sxs-lookup"><span data-stu-id="ec05d-111">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec05d-112">权限</span><span class="sxs-lookup"><span data-stu-id="ec05d-112">Permissions</span></span>
<span data-ttu-id="ec05d-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec05d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec05d-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec05d-115">Permission type</span></span>      | <span data-ttu-id="ec05d-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec05d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec05d-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec05d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ec05d-118">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec05d-118">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec05d-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec05d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec05d-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec05d-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec05d-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec05d-121">Application</span></span> | <span data-ttu-id="ec05d-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec05d-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec05d-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec05d-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/add
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="ec05d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec05d-124">Request headers</span></span>
| <span data-ttu-id="ec05d-125">名称</span><span class="sxs-lookup"><span data-stu-id="ec05d-125">Name</span></span>       | <span data-ttu-id="ec05d-126">说明</span><span class="sxs-lookup"><span data-stu-id="ec05d-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ec05d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec05d-127">Authorization</span></span>  | <span data-ttu-id="ec05d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec05d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec05d-130">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec05d-130">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec05d-p106">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ec05d-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec05d-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec05d-133">Request body</span></span>
<span data-ttu-id="ec05d-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ec05d-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ec05d-135">参数</span><span class="sxs-lookup"><span data-stu-id="ec05d-135">Parameter</span></span>    | <span data-ttu-id="ec05d-136">类型</span><span class="sxs-lookup"><span data-stu-id="ec05d-136">Type</span></span>   |<span data-ttu-id="ec05d-137">说明</span><span class="sxs-lookup"><span data-stu-id="ec05d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec05d-138">address</span><span class="sxs-lookup"><span data-stu-id="ec05d-138">address</span></span>|<span data-ttu-id="ec05d-139">string</span><span class="sxs-lookup"><span data-stu-id="ec05d-139">string</span></span>|<span data-ttu-id="ec05d-p107">表示数据源的 range 对象的地址或名称。如果该地址不包含工作表名称，则使用当前活动的工作表。</span><span class="sxs-lookup"><span data-stu-id="ec05d-p107">Address or name of the range object representing the data source. If the address does not contain a sheet name, the currently-active sheet is used.</span></span>|
|<span data-ttu-id="ec05d-142">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="ec05d-142">hasHeaders</span></span>|<span data-ttu-id="ec05d-143">boolean</span><span class="sxs-lookup"><span data-stu-id="ec05d-143">boolean</span></span>|<span data-ttu-id="ec05d-p108">指示导入的数据是否具有列标签的布尔值。如果源不包含标头（即，当此属性设置为 false 时），Excel 将自动生成标头，数据将向下移动一行。</span><span class="sxs-lookup"><span data-stu-id="ec05d-p108">Boolean value that indicates whether the data being imported has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="ec05d-147">响应</span><span class="sxs-lookup"><span data-stu-id="ec05d-147">Response</span></span>

<span data-ttu-id="ec05d-148">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[workbookTable](../resources/workbooktable.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ec05d-148">If successful, this method returns `200 OK` response code and [workbookTable](../resources/workbooktable.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec05d-149">示例</span><span class="sxs-lookup"><span data-stu-id="ec05d-149">Example</span></span>
<span data-ttu-id="ec05d-150">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ec05d-150">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ec05d-151">请求</span><span class="sxs-lookup"><span data-stu-id="ec05d-151">Request</span></span>
<span data-ttu-id="ec05d-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec05d-152">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecollection_add"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/add
Content-type: application/json
Content-length: 54

{
  "address": "Sheet1!A1:D5",
  "hasHeaders": true
}
```

##### <a name="response"></a><span data-ttu-id="ec05d-153">响应</span><span class="sxs-lookup"><span data-stu-id="ec05d-153">Response</span></span>
<span data-ttu-id="ec05d-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec05d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTable"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
