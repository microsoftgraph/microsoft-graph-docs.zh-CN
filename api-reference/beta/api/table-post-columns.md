---
title: 创建 TableColumn
description: 使用此 API 创建新的 TableColumn。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c6a0dc30be0e423129a0bd7ec9c6582e6f582d96
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959781"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="ec5e1-103">创建 TableColumn</span><span class="sxs-lookup"><span data-stu-id="ec5e1-103">Create TableColumn</span></span>

> <span data-ttu-id="ec5e1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec5e1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec5e1-106">使用此 API 创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-106">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec5e1-107">权限</span><span class="sxs-lookup"><span data-stu-id="ec5e1-107">Permissions</span></span>
<span data-ttu-id="ec5e1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec5e1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec5e1-110">Permission type</span></span>      | <span data-ttu-id="ec5e1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec5e1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec5e1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec5e1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ec5e1-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec5e1-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec5e1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec5e1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec5e1-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec5e1-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ec5e1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec5e1-116">Application</span></span> | <span data-ttu-id="ec5e1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec5e1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec5e1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="ec5e1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec5e1-119">Request headers</span></span>
| <span data-ttu-id="ec5e1-120">名称</span><span class="sxs-lookup"><span data-stu-id="ec5e1-120">Name</span></span>       | <span data-ttu-id="ec5e1-121">说明</span><span class="sxs-lookup"><span data-stu-id="ec5e1-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ec5e1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec5e1-122">Authorization</span></span>  | <span data-ttu-id="ec5e1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec5e1-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="ec5e1-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ec5e1-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec5e1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec5e1-128">Request body</span></span>
<span data-ttu-id="ec5e1-129">在请求正文中，提供 [TableColumn](../resources/tablecolumn.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-129">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ec5e1-130">响应</span><span class="sxs-lookup"><span data-stu-id="ec5e1-130">Response</span></span>

<span data-ttu-id="ec5e1-131">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [TableColumn](../resources/tablecolumn.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-131">If successful, this method returns `201 Created` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec5e1-132">示例</span><span class="sxs-lookup"><span data-stu-id="ec5e1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec5e1-133">请求</span><span class="sxs-lookup"><span data-stu-id="ec5e1-133">Request</span></span>
<span data-ttu-id="ec5e1-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_tablecolumn_from_table"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```
<span data-ttu-id="ec5e1-135">在请求正文中，提供 [TableColumn](../resources/tablecolumn.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-135">In the request body, supply a JSON representation of [TableColumn](../resources/tablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ec5e1-136">响应</span><span class="sxs-lookup"><span data-stu-id="ec5e1-136">Response</span></span>
<span data-ttu-id="ec5e1-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec5e1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
