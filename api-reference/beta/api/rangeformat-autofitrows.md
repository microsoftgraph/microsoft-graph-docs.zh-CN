---
title: 'RangeFormat: autofitRows'
description: 根据列中的当前数据，更改当前范围的行高以达到最佳高度。
localization_priority: Normal
ms.openlocfilehash: 1a915a3af5a0d0300f957ebf27ef0415c0d00465
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894283"
---
# <a name="rangeformat-autofitrows"></a><span data-ttu-id="442ca-103">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="442ca-103">RangeFormat: autofitRows</span></span>

> <span data-ttu-id="442ca-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="442ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="442ca-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="442ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="442ca-106">根据列中的当前数据，更改当前范围的行高以达到最佳高度。</span><span class="sxs-lookup"><span data-stu-id="442ca-106">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="442ca-107">权限</span><span class="sxs-lookup"><span data-stu-id="442ca-107">Permissions</span></span>
<span data-ttu-id="442ca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="442ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="442ca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="442ca-110">Permission type</span></span>      | <span data-ttu-id="442ca-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="442ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="442ca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="442ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="442ca-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="442ca-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="442ca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="442ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="442ca-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="442ca-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="442ca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="442ca-116">Application</span></span> | <span data-ttu-id="442ca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="442ca-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="442ca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="442ca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="442ca-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="442ca-119">Request headers</span></span>
| <span data-ttu-id="442ca-120">名称</span><span class="sxs-lookup"><span data-stu-id="442ca-120">Name</span></span>       | <span data-ttu-id="442ca-121">说明</span><span class="sxs-lookup"><span data-stu-id="442ca-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="442ca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="442ca-122">Authorization</span></span>  | <span data-ttu-id="442ca-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="442ca-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="442ca-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="442ca-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="442ca-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="442ca-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="442ca-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="442ca-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="442ca-129">响应</span><span class="sxs-lookup"><span data-stu-id="442ca-129">Response</span></span>

<span data-ttu-id="442ca-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="442ca-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="442ca-132">示例</span><span class="sxs-lookup"><span data-stu-id="442ca-132">Example</span></span>
<span data-ttu-id="442ca-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="442ca-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="442ca-134">请求</span><span class="sxs-lookup"><span data-stu-id="442ca-134">Request</span></span>
<span data-ttu-id="442ca-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="442ca-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="442ca-136">响应</span><span class="sxs-lookup"><span data-stu-id="442ca-136">Response</span></span>
<span data-ttu-id="442ca-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="442ca-137">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
