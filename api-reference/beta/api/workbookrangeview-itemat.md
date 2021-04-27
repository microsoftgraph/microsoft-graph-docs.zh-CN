---
title: 'workbookRangeView: itemAt'
description: 要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4af87ed2df66089e6ba5fc8292d133a972f5b0ce
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053291"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="7bbe6-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="7bbe6-104">workbookRangeView: itemAt</span></span>

<span data-ttu-id="7bbe6-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bbe6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="7bbe6-106">权限</span><span class="sxs-lookup"><span data-stu-id="7bbe6-106">Permissions</span></span>
<span data-ttu-id="7bbe6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bbe6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7bbe6-109">Permission type</span></span>      | <span data-ttu-id="7bbe6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7bbe6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bbe6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7bbe6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7bbe6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-112">Not supported.</span></span>    |
|<span data-ttu-id="7bbe6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7bbe6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bbe6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-114">Not supported.</span></span>    |
|<span data-ttu-id="7bbe6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7bbe6-115">Application</span></span> | <span data-ttu-id="7bbe6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bbe6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7bbe6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="7bbe6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7bbe6-118">Request headers</span></span>
| <span data-ttu-id="7bbe6-119">名称</span><span class="sxs-lookup"><span data-stu-id="7bbe6-119">Name</span></span>       | <span data-ttu-id="7bbe6-120">说明</span><span class="sxs-lookup"><span data-stu-id="7bbe6-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7bbe6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bbe6-121">Authorization</span></span>  | <span data-ttu-id="7bbe6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7bbe6-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7bbe6-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="7bbe6-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bbe6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7bbe6-127">Request body</span></span>
<span data-ttu-id="7bbe6-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-128">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="7bbe6-129">参数</span><span class="sxs-lookup"><span data-stu-id="7bbe6-129">Parameter</span></span>    | <span data-ttu-id="7bbe6-130">类型</span><span class="sxs-lookup"><span data-stu-id="7bbe6-130">Type</span></span>   |<span data-ttu-id="7bbe6-131">说明</span><span class="sxs-lookup"><span data-stu-id="7bbe6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bbe6-132">index</span><span class="sxs-lookup"><span data-stu-id="7bbe6-132">index</span></span>|<span data-ttu-id="7bbe6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="7bbe6-133">Int32</span></span>|<span data-ttu-id="7bbe6-134">要返回的项的索引。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-134">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="7bbe6-135">响应</span><span class="sxs-lookup"><span data-stu-id="7bbe6-135">Response</span></span>

<span data-ttu-id="7bbe6-136">如果成功，此方法在响应正文中返回 `200 OK`响应代码和 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-136">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bbe6-137">示例</span><span class="sxs-lookup"><span data-stu-id="7bbe6-137">Example</span></span>
<span data-ttu-id="7bbe6-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7bbe6-139">请求</span><span class="sxs-lookup"><span data-stu-id="7bbe6-139">Request</span></span>
<span data-ttu-id="7bbe6-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="7bbe6-141">响应</span><span class="sxs-lookup"><span data-stu-id="7bbe6-141">Response</span></span>
<span data-ttu-id="7bbe6-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-142">Here is an example of the response.</span></span> <span data-ttu-id="7bbe6-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7bbe6-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```


