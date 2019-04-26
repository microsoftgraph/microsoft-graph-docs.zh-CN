---
title: 'Range: unmerge'
description: 将范围单元格取消合并为各个单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 31f668506ce04271e31acec3efd85ce0cd747e9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583968"
---
# <a name="range-unmerge"></a><span data-ttu-id="89a6b-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="89a6b-103">Range: unmerge</span></span>

<span data-ttu-id="89a6b-104">将范围单元格取消合并为各个单元格。</span><span class="sxs-lookup"><span data-stu-id="89a6b-104">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="89a6b-105">权限</span><span class="sxs-lookup"><span data-stu-id="89a6b-105">Permissions</span></span>
<span data-ttu-id="89a6b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89a6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89a6b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="89a6b-108">Permission type</span></span>      | <span data-ttu-id="89a6b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89a6b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89a6b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89a6b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="89a6b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89a6b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="89a6b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89a6b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89a6b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="89a6b-113">Not supported.</span></span>    |
|<span data-ttu-id="89a6b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="89a6b-114">Application</span></span> | <span data-ttu-id="89a6b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="89a6b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89a6b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89a6b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="89a6b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="89a6b-117">Request headers</span></span>
| <span data-ttu-id="89a6b-118">名称</span><span class="sxs-lookup"><span data-stu-id="89a6b-118">Name</span></span>       | <span data-ttu-id="89a6b-119">说明</span><span class="sxs-lookup"><span data-stu-id="89a6b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="89a6b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="89a6b-120">Authorization</span></span>  | <span data-ttu-id="89a6b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89a6b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="89a6b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="89a6b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="89a6b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="89a6b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="89a6b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="89a6b-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="89a6b-127">响应</span><span class="sxs-lookup"><span data-stu-id="89a6b-127">Response</span></span>

<span data-ttu-id="89a6b-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="89a6b-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89a6b-130">示例</span><span class="sxs-lookup"><span data-stu-id="89a6b-130">Example</span></span>
<span data-ttu-id="89a6b-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="89a6b-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="89a6b-132">请求</span><span class="sxs-lookup"><span data-stu-id="89a6b-132">Request</span></span>
<span data-ttu-id="89a6b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="89a6b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/unmerge
```

##### <a name="response"></a><span data-ttu-id="89a6b-134">响应</span><span class="sxs-lookup"><span data-stu-id="89a6b-134">Response</span></span>
<span data-ttu-id="89a6b-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="89a6b-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
