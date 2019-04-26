---
title: 'workbookPivotTable: refreshAll'
description: 刷新给定工作表中的数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 43d11f6c016f2d15fc0c0b9c4f74d9de731b7dca
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339544"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="ff176-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="ff176-103">workbookPivotTable: refreshAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff176-104">刷新给定工作表中的数据透视表。</span><span class="sxs-lookup"><span data-stu-id="ff176-104">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff176-105">权限</span><span class="sxs-lookup"><span data-stu-id="ff176-105">Permissions</span></span>
<span data-ttu-id="ff176-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff176-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff176-108">Permission type</span></span>      | <span data-ttu-id="ff176-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff176-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff176-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff176-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff176-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff176-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ff176-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff176-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff176-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff176-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ff176-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff176-114">Application</span></span> | <span data-ttu-id="ff176-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff176-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff176-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff176-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="ff176-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff176-117">Request headers</span></span>
| <span data-ttu-id="ff176-118">名称</span><span class="sxs-lookup"><span data-stu-id="ff176-118">Name</span></span>       | <span data-ttu-id="ff176-119">说明</span><span class="sxs-lookup"><span data-stu-id="ff176-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ff176-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff176-120">Authorization</span></span>  | <span data-ttu-id="ff176-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff176-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff176-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ff176-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="ff176-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ff176-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff176-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff176-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ff176-127">响应</span><span class="sxs-lookup"><span data-stu-id="ff176-127">Response</span></span>

<span data-ttu-id="ff176-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ff176-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff176-130">示例</span><span class="sxs-lookup"><span data-stu-id="ff176-130">Example</span></span>
<span data-ttu-id="ff176-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ff176-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ff176-132">请求</span><span class="sxs-lookup"><span data-stu-id="ff176-132">Request</span></span>
<span data-ttu-id="ff176-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff176-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="ff176-134">响应</span><span class="sxs-lookup"><span data-stu-id="ff176-134">Response</span></span>
<span data-ttu-id="ff176-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ff176-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
