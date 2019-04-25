---
title: Range:LastRow
description: .
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8f6ed391f1158b6b9253827c52c50a0b197e31a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546198"
---
# <a name="range-lastrow"></a><span data-ttu-id="f6dfd-103">Range:LastRow</span><span class="sxs-lookup"><span data-stu-id="f6dfd-103">Range: LastRow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6dfd-p101">获取区域内的最后一行。例如，“B2:D5”的最后一行是“B5:D5”。</span><span class="sxs-lookup"><span data-stu-id="f6dfd-p101">Gets the last row within the range. For example, the last row of "B2:D5" is "B5:D5".</span></span>
## <a name="permissions"></a><span data-ttu-id="f6dfd-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6dfd-106">Permissions</span></span>
<span data-ttu-id="f6dfd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6dfd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6dfd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6dfd-109">Permission type</span></span>      | <span data-ttu-id="f6dfd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6dfd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6dfd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6dfd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6dfd-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6dfd-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f6dfd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6dfd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6dfd-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6dfd-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f6dfd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6dfd-115">Application</span></span> | <span data-ttu-id="f6dfd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6dfd-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6dfd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6dfd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/LastRow
GET /workbook/worksheets/{id|name}/range(address='<address>')/LastRow
GET /workbook/tables/{id|name}/columns/{id|name}/range/LastRow

```
## <a name="request-headers"></a><span data-ttu-id="f6dfd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6dfd-118">Request headers</span></span>
| <span data-ttu-id="f6dfd-119">名称</span><span class="sxs-lookup"><span data-stu-id="f6dfd-119">Name</span></span>       | <span data-ttu-id="f6dfd-120">说明</span><span class="sxs-lookup"><span data-stu-id="f6dfd-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f6dfd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6dfd-121">Authorization</span></span>  | <span data-ttu-id="f6dfd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6dfd-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6dfd-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f6dfd-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f6dfd-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f6dfd-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6dfd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6dfd-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f6dfd-128">响应</span><span class="sxs-lookup"><span data-stu-id="f6dfd-128">Response</span></span>

<span data-ttu-id="f6dfd-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6dfd-129">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6dfd-130">示例</span><span class="sxs-lookup"><span data-stu-id="f6dfd-130">Example</span></span>
<span data-ttu-id="f6dfd-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f6dfd-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f6dfd-132">请求</span><span class="sxs-lookup"><span data-stu-id="f6dfd-132">Request</span></span>
<span data-ttu-id="f6dfd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6dfd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_lastrow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/LastRow
```

##### <a name="response"></a><span data-ttu-id="f6dfd-134">响应</span><span class="sxs-lookup"><span data-stu-id="f6dfd-134">Response</span></span>
<span data-ttu-id="f6dfd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6dfd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Range: LastRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/range-lastrow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
