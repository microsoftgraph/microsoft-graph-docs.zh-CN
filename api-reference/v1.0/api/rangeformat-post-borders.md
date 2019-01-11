---
title: 创建 RangeBorder
description: 使用此 API 创建新 RangeBorder。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2d87f4943158fa33d2cc09e600959bd7dc99087b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873085"
---
# <a name="create-rangeborder"></a><span data-ttu-id="1ee0b-103">创建 RangeBorder</span><span class="sxs-lookup"><span data-stu-id="1ee0b-103">Create RangeBorder</span></span>

<span data-ttu-id="1ee0b-104">使用此 API 创建新 RangeBorder。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-104">Use this API to create a new RangeBorder.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ee0b-105">权限</span><span class="sxs-lookup"><span data-stu-id="1ee0b-105">Permissions</span></span>
<span data-ttu-id="1ee0b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ee0b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ee0b-108">Permission type</span></span>      | <span data-ttu-id="1ee0b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ee0b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ee0b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ee0b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ee0b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ee0b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1ee0b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ee0b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ee0b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-113">Not supported.</span></span>    |
|<span data-ttu-id="1ee0b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ee0b-114">Application</span></span> | <span data-ttu-id="1ee0b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ee0b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ee0b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/format/borders
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders

```
## <a name="request-headers"></a><span data-ttu-id="1ee0b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ee0b-117">Request headers</span></span>
| <span data-ttu-id="1ee0b-118">名称</span><span class="sxs-lookup"><span data-stu-id="1ee0b-118">Name</span></span>       | <span data-ttu-id="1ee0b-119">说明</span><span class="sxs-lookup"><span data-stu-id="1ee0b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1ee0b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ee0b-120">Authorization</span></span>  | <span data-ttu-id="1ee0b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ee0b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1ee0b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="1ee0b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ee0b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ee0b-126">Request body</span></span>
<span data-ttu-id="1ee0b-127">在请求正文中，提供[WorkbookRangeBorder](../resources/rangeborder.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-127">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1ee0b-128">响应</span><span class="sxs-lookup"><span data-stu-id="1ee0b-128">Response</span></span>

<span data-ttu-id="1ee0b-129">如果成功，此方法返回`201 Created`响应代码和[WorkbookRangeBorder](../resources/rangeborder.md)响应正文中的对象。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-129">If successful, this method returns `201 Created` response code and [WorkbookRangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ee0b-130">示例</span><span class="sxs-lookup"><span data-stu-id="1ee0b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ee0b-131">请求</span><span class="sxs-lookup"><span data-stu-id="1ee0b-131">Request</span></span>
<span data-ttu-id="1ee0b-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rangeborder_from_rangeformat"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/format/borders
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```
<span data-ttu-id="1ee0b-133">在请求正文中，提供[WorkbookRangeBorder](../resources/rangeborder.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-133">In the request body, supply a JSON representation of [WorkbookRangeBorder](../resources/rangeborder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1ee0b-134">响应</span><span class="sxs-lookup"><span data-stu-id="1ee0b-134">Response</span></span>
<span data-ttu-id="1ee0b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ee0b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeBorder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create RangeBorder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
