---
title: 'RangeFormat: autofitRows'
description: 根据列中的当前数据，更改当前范围的行高以达到最佳高度。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a25fdd90f8bb0f7ad92aca5207c1529abc370a65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517706"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="e0cc8-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="e0cc8-103">RangeFormat: autofitRows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0cc8-104">根据列中的当前数据，更改当前范围的行高以达到最佳高度。</span><span class="sxs-lookup"><span data-stu-id="e0cc8-104">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0cc8-105">权限</span><span class="sxs-lookup"><span data-stu-id="e0cc8-105">Permissions</span></span>
<span data-ttu-id="e0cc8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0cc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0cc8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0cc8-108">Permission type</span></span>      | <span data-ttu-id="e0cc8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0cc8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0cc8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0cc8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e0cc8-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0cc8-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0cc8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0cc8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0cc8-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0cc8-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e0cc8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0cc8-114">Application</span></span> | <span data-ttu-id="e0cc8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0cc8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0cc8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0cc8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="e0cc8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0cc8-117">Request headers</span></span>
| <span data-ttu-id="e0cc8-118">名称</span><span class="sxs-lookup"><span data-stu-id="e0cc8-118">Name</span></span>       | <span data-ttu-id="e0cc8-119">说明</span><span class="sxs-lookup"><span data-stu-id="e0cc8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0cc8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0cc8-120">Authorization</span></span>  | <span data-ttu-id="e0cc8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e0cc8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e0cc8-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e0cc8-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="e0cc8-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="e0cc8-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0cc8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0cc8-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e0cc8-127">响应</span><span class="sxs-lookup"><span data-stu-id="e0cc8-127">Response</span></span>

<span data-ttu-id="e0cc8-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e0cc8-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0cc8-130">示例</span><span class="sxs-lookup"><span data-stu-id="e0cc8-130">Example</span></span>
<span data-ttu-id="e0cc8-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e0cc8-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e0cc8-132">请求</span><span class="sxs-lookup"><span data-stu-id="e0cc8-132">Request</span></span>
<span data-ttu-id="e0cc8-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0cc8-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="e0cc8-134">响应</span><span class="sxs-lookup"><span data-stu-id="e0cc8-134">Response</span></span>
<span data-ttu-id="e0cc8-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0cc8-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangeformat-autofitrows.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
