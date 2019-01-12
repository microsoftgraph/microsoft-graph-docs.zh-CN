---
title: 'workbookPivotTable: refreshAll'
description: 刷新给定工作表中的数据透视表。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6edad0def37d67dddb6258814c6d4a4004a93366
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982237"
---
# <a name="workbookpivottable-refreshall"></a><span data-ttu-id="4771f-103">workbookPivotTable: refreshAll</span><span class="sxs-lookup"><span data-stu-id="4771f-103">workbookPivotTable: refreshAll</span></span>

> <span data-ttu-id="4771f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4771f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4771f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4771f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4771f-106">刷新给定工作表中的数据透视表。</span><span class="sxs-lookup"><span data-stu-id="4771f-106">Refreshes the PivotTable within a given worksheet.</span></span>

## <a name="permissions"></a><span data-ttu-id="4771f-107">权限</span><span class="sxs-lookup"><span data-stu-id="4771f-107">Permissions</span></span>
<span data-ttu-id="4771f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4771f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4771f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4771f-110">Permission type</span></span>      | <span data-ttu-id="4771f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4771f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4771f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4771f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4771f-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4771f-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4771f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4771f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4771f-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4771f-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4771f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4771f-116">Application</span></span> | <span data-ttu-id="4771f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4771f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4771f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4771f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll

```
## <a name="request-headers"></a><span data-ttu-id="4771f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4771f-119">Request headers</span></span>
| <span data-ttu-id="4771f-120">名称</span><span class="sxs-lookup"><span data-stu-id="4771f-120">Name</span></span>       | <span data-ttu-id="4771f-121">说明</span><span class="sxs-lookup"><span data-stu-id="4771f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4771f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4771f-122">Authorization</span></span>  | <span data-ttu-id="4771f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4771f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4771f-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="4771f-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="4771f-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="4771f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4771f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4771f-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="4771f-129">响应</span><span class="sxs-lookup"><span data-stu-id="4771f-129">Response</span></span>

<span data-ttu-id="4771f-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4771f-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4771f-132">示例</span><span class="sxs-lookup"><span data-stu-id="4771f-132">Example</span></span>
<span data-ttu-id="4771f-133">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4771f-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4771f-134">请求</span><span class="sxs-lookup"><span data-stu-id="4771f-134">Request</span></span>
<span data-ttu-id="4771f-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4771f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="4771f-136">响应</span><span class="sxs-lookup"><span data-stu-id="4771f-136">Response</span></span>
<span data-ttu-id="4771f-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4771f-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
