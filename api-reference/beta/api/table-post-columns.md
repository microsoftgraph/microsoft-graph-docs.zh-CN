---
title: 创建 TableColumn
description: 使用此 API 创建新的 TableColumn。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a95079908dfb85e8474f308808f0ade26f3952a0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330153"
---
# <a name="create-tablecolumn"></a><span data-ttu-id="39bf5-103">创建 TableColumn</span><span class="sxs-lookup"><span data-stu-id="39bf5-103">Create TableColumn</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39bf5-104">使用此 API 创建新的 TableColumn。</span><span class="sxs-lookup"><span data-stu-id="39bf5-104">Use this API to create a new TableColumn.</span></span>
## <a name="permissions"></a><span data-ttu-id="39bf5-105">权限</span><span class="sxs-lookup"><span data-stu-id="39bf5-105">Permissions</span></span>
<span data-ttu-id="39bf5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39bf5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39bf5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="39bf5-108">Permission type</span></span>      | <span data-ttu-id="39bf5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39bf5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39bf5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39bf5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="39bf5-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39bf5-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39bf5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39bf5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39bf5-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="39bf5-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="39bf5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="39bf5-114">Application</span></span> | <span data-ttu-id="39bf5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="39bf5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39bf5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39bf5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns

```
## <a name="request-headers"></a><span data-ttu-id="39bf5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="39bf5-117">Request headers</span></span>
| <span data-ttu-id="39bf5-118">名称</span><span class="sxs-lookup"><span data-stu-id="39bf5-118">Name</span></span>       | <span data-ttu-id="39bf5-119">说明</span><span class="sxs-lookup"><span data-stu-id="39bf5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="39bf5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="39bf5-120">Authorization</span></span>  | <span data-ttu-id="39bf5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39bf5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39bf5-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="39bf5-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="39bf5-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="39bf5-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39bf5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="39bf5-126">Request body</span></span>
<span data-ttu-id="39bf5-127">在请求正文中, 提供[workbookTableColumn](../resources/workbooktablecolumn.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39bf5-127">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="39bf5-128">响应</span><span class="sxs-lookup"><span data-stu-id="39bf5-128">Response</span></span>

<span data-ttu-id="39bf5-129">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[workbookTableColumn](../resources/workbooktablecolumn.md)对象。</span><span class="sxs-lookup"><span data-stu-id="39bf5-129">If successful, this method returns `201 Created` response code and [workbookTableColumn](../resources/workbooktablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39bf5-130">示例</span><span class="sxs-lookup"><span data-stu-id="39bf5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39bf5-131">请求</span><span class="sxs-lookup"><span data-stu-id="39bf5-131">Request</span></span>
<span data-ttu-id="39bf5-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39bf5-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="39bf5-133">在请求正文中, 提供[workbookTableColumn](../resources/workbooktablecolumn.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39bf5-133">In the request body, supply a JSON representation of [workbookTableColumn](../resources/workbooktablecolumn.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="39bf5-134">响应</span><span class="sxs-lookup"><span data-stu-id="39bf5-134">Response</span></span>
<span data-ttu-id="39bf5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39bf5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableColumn"
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
<!--
{
  "type": "#page.annotation",
  "description": "Create TableColumn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
