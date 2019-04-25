---
title: 'workbookRangeView: itemAt'
description: 若要调用此 API, 必须有以下权限之一。 若要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 85dcf4efd1cbbeae56b1f200ef53f48d19641369
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535961"
---
# <a name="workbookrangeview-itemat"></a><span data-ttu-id="b2278-104">workbookRangeView: itemAt</span><span class="sxs-lookup"><span data-stu-id="b2278-104">workbookRangeView: itemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="b2278-105">权限</span><span class="sxs-lookup"><span data-stu-id="b2278-105">Permissions</span></span>
<span data-ttu-id="b2278-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2278-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2278-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2278-108">Permission type</span></span>      | <span data-ttu-id="b2278-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2278-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2278-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2278-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b2278-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2278-111">Not supported.</span></span>    |
|<span data-ttu-id="b2278-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2278-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2278-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2278-113">Not supported.</span></span>    |
|<span data-ttu-id="b2278-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2278-114">Application</span></span> | <span data-ttu-id="b2278-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2278-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2278-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2278-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/itemAt(index={n})

```
## <a name="request-headers"></a><span data-ttu-id="b2278-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2278-117">Request headers</span></span>
| <span data-ttu-id="b2278-118">名称</span><span class="sxs-lookup"><span data-stu-id="b2278-118">Name</span></span>       | <span data-ttu-id="b2278-119">说明</span><span class="sxs-lookup"><span data-stu-id="b2278-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2278-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2278-120">Authorization</span></span>  | <span data-ttu-id="b2278-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2278-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2278-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b2278-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="b2278-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="b2278-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2278-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2278-126">Request body</span></span>
<span data-ttu-id="b2278-127">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="b2278-127">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="b2278-128">参数</span><span class="sxs-lookup"><span data-stu-id="b2278-128">Parameter</span></span>    | <span data-ttu-id="b2278-129">类型</span><span class="sxs-lookup"><span data-stu-id="b2278-129">Type</span></span>   |<span data-ttu-id="b2278-130">说明</span><span class="sxs-lookup"><span data-stu-id="b2278-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2278-131">index</span><span class="sxs-lookup"><span data-stu-id="b2278-131">index</span></span>|<span data-ttu-id="b2278-132">Int32</span><span class="sxs-lookup"><span data-stu-id="b2278-132">Int32</span></span>|<span data-ttu-id="b2278-133">要返回的项的索引。</span><span class="sxs-lookup"><span data-stu-id="b2278-133">Index of the item to be returned.</span></span>|

## <a name="response"></a><span data-ttu-id="b2278-134">响应</span><span class="sxs-lookup"><span data-stu-id="b2278-134">Response</span></span>

<span data-ttu-id="b2278-135">如果成功，此方法在响应正文中返回 `200 OK`响应代码和 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b2278-135">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2278-136">示例</span><span class="sxs-lookup"><span data-stu-id="b2278-136">Example</span></span>
<span data-ttu-id="b2278-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b2278-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b2278-138">请求</span><span class="sxs-lookup"><span data-stu-id="b2278-138">Request</span></span>
<span data-ttu-id="b2278-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b2278-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/itemAt(index=0)

```

##### <a name="response"></a><span data-ttu-id="b2278-140">响应</span><span class="sxs-lookup"><span data-stu-id="b2278-140">Response</span></span>
<span data-ttu-id="b2278-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b2278-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrangeview-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
