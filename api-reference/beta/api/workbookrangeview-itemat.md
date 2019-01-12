---
title: 'workbookRangeView: itemAt'
description: >
  需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅权限。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 423c20f6cbdcbfe65a2f8db965a4765c93079f18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960579"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="01b80-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="01b80-104">workbookRangeView: itemAt</span></span>

> <span data-ttu-id="01b80-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01b80-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01b80-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01b80-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="01b80-107">权限</span><span class="sxs-lookup"><span data-stu-id="01b80-107">Permissions</span></span>
<span data-ttu-id="01b80-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01b80-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01b80-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01b80-110">Permission type</span></span>      | <span data-ttu-id="01b80-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01b80-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01b80-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01b80-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01b80-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="01b80-113">Not supported.</span></span>    |
|<span data-ttu-id="01b80-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01b80-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01b80-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01b80-115">Not supported.</span></span>    |
|<span data-ttu-id="01b80-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="01b80-116">Application</span></span> | <span data-ttu-id="01b80-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="01b80-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01b80-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01b80-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="01b80-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="01b80-119">Request headers</span></span>
| <span data-ttu-id="01b80-120">名称</span><span class="sxs-lookup"><span data-stu-id="01b80-120">Name</span></span>       | <span data-ttu-id="01b80-121">说明</span><span class="sxs-lookup"><span data-stu-id="01b80-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01b80-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="01b80-122">Authorization</span></span>  | <span data-ttu-id="01b80-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01b80-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01b80-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="01b80-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="01b80-p105">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="01b80-p105">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01b80-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="01b80-128">Request body</span></span>
<span data-ttu-id="01b80-129">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="01b80-129">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="01b80-130">参数</span><span class="sxs-lookup"><span data-stu-id="01b80-130">Parameter</span></span>    | <span data-ttu-id="01b80-131">类型</span><span class="sxs-lookup"><span data-stu-id="01b80-131">Type</span></span>   |<span data-ttu-id="01b80-132">说明</span><span class="sxs-lookup"><span data-stu-id="01b80-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01b80-133">index</span><span class="sxs-lookup"><span data-stu-id="01b80-133">index</span></span>|<span data-ttu-id="01b80-134">Int32</span><span class="sxs-lookup"><span data-stu-id="01b80-134">Int32</span></span>|<span data-ttu-id="01b80-135">要返回的项的索引。</span><span class="sxs-lookup"><span data-stu-id="01b80-135">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="01b80-136">响应</span><span class="sxs-lookup"><span data-stu-id="01b80-136">Response</span></span>

<span data-ttu-id="01b80-137">如果成功，此方法在响应正文中返回 `200 OK`响应代码和 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01b80-137">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01b80-138">示例</span><span class="sxs-lookup"><span data-stu-id="01b80-138">Example</span></span>
<span data-ttu-id="01b80-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="01b80-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="01b80-140">请求</span><span class="sxs-lookup"><span data-stu-id="01b80-140">Request</span></span>
<span data-ttu-id="01b80-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01b80-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="01b80-142">响应</span><span class="sxs-lookup"><span data-stu-id="01b80-142">Response</span></span>
<span data-ttu-id="01b80-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01b80-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
