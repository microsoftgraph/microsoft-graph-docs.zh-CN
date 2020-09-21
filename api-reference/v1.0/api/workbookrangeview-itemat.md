---
title: 'workbookRangeView: itemAt'
description: 若要调用此 API，必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 118274017a67d330a3c5e3927fe3d93c7ce30ad2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965692"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="9390f-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="9390f-104">workbookRangeView: itemAt</span></span>

<span data-ttu-id="9390f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9390f-105">Namespace: microsoft.graph</span></span>


## <a name="permissions"></a><span data-ttu-id="9390f-106">权限</span><span class="sxs-lookup"><span data-stu-id="9390f-106">Permissions</span></span>
<span data-ttu-id="9390f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9390f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9390f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9390f-109">Permission type</span></span>      | <span data-ttu-id="9390f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9390f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9390f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9390f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9390f-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9390f-112">Files.ReadWrite</span></span> |
|<span data-ttu-id="9390f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9390f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9390f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9390f-114">Not supported.</span></span>    |
|<span data-ttu-id="9390f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9390f-115">Application</span></span> | <span data-ttu-id="9390f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9390f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9390f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9390f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="9390f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9390f-118">Request headers</span></span>
| <span data-ttu-id="9390f-119">名称</span><span class="sxs-lookup"><span data-stu-id="9390f-119">Name</span></span>       | <span data-ttu-id="9390f-120">说明</span><span class="sxs-lookup"><span data-stu-id="9390f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9390f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9390f-121">Authorization</span></span>  | <span data-ttu-id="9390f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9390f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9390f-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9390f-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="9390f-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="9390f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="function-parameters"></a><span data-ttu-id="9390f-127">函数参数</span><span class="sxs-lookup"><span data-stu-id="9390f-127">Function parameters</span></span>
<span data-ttu-id="9390f-128">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="9390f-128">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="9390f-129">参数</span><span class="sxs-lookup"><span data-stu-id="9390f-129">Parameter</span></span>    | <span data-ttu-id="9390f-130">类型</span><span class="sxs-lookup"><span data-stu-id="9390f-130">Type</span></span>   |<span data-ttu-id="9390f-131">说明</span><span class="sxs-lookup"><span data-stu-id="9390f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9390f-132">index</span><span class="sxs-lookup"><span data-stu-id="9390f-132">index</span></span>|<span data-ttu-id="9390f-133">Int32</span><span class="sxs-lookup"><span data-stu-id="9390f-133">Int32</span></span>|<span data-ttu-id="9390f-134">要返回的项的索引。</span><span class="sxs-lookup"><span data-stu-id="9390f-134">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="9390f-135">响应</span><span class="sxs-lookup"><span data-stu-id="9390f-135">Response</span></span>

<span data-ttu-id="9390f-136">如果成功，此方法在响应正文中返回 `200 OK`响应代码和 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9390f-136">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9390f-137">示例</span><span class="sxs-lookup"><span data-stu-id="9390f-137">Example</span></span>
<span data-ttu-id="9390f-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9390f-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9390f-139">请求</span><span class="sxs-lookup"><span data-stu-id="9390f-139">Request</span></span>
<span data-ttu-id="9390f-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9390f-140">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="9390f-141">响应</span><span class="sxs-lookup"><span data-stu-id="9390f-141">Response</span></span>
<span data-ttu-id="9390f-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9390f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

