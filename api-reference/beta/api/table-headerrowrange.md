---
title: Table:HeaderRowRange
description: 获取与表的标头行相关的 range 对象。
ms.openlocfilehash: 2f6a21b54812e691f581a560dac4dfa89b4de010
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043075"
---
# <a name="table-headerrowrange"></a><span data-ttu-id="3e43e-103">Table:HeaderRowRange</span><span class="sxs-lookup"><span data-stu-id="3e43e-103">Table: HeaderRowRange</span></span>

> <span data-ttu-id="3e43e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3e43e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e43e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3e43e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e43e-106">获取与表的标头行相关的 range 对象。</span><span class="sxs-lookup"><span data-stu-id="3e43e-106">Gets the range object associated with header row of the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="3e43e-107">权限</span><span class="sxs-lookup"><span data-stu-id="3e43e-107">Permissions</span></span>
<span data-ttu-id="3e43e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e43e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e43e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e43e-110">Permission type</span></span>      | <span data-ttu-id="3e43e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e43e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e43e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e43e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e43e-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e43e-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e43e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e43e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e43e-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e43e-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3e43e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e43e-116">Application</span></span> | <span data-ttu-id="3e43e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e43e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e43e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e43e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/HeaderRowRange
POST /workbook/worksheets/{id|name}/tables/{id|name}/HeaderRowRange

```
## <a name="request-headers"></a><span data-ttu-id="3e43e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e43e-119">Request headers</span></span>
| <span data-ttu-id="3e43e-120">名称</span><span class="sxs-lookup"><span data-stu-id="3e43e-120">Name</span></span>       | <span data-ttu-id="3e43e-121">说明</span><span class="sxs-lookup"><span data-stu-id="3e43e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e43e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e43e-122">Authorization</span></span>  | <span data-ttu-id="3e43e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e43e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e43e-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3e43e-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e43e-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="3e43e-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e43e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e43e-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3e43e-129">响应</span><span class="sxs-lookup"><span data-stu-id="3e43e-129">Response</span></span>

<span data-ttu-id="3e43e-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Range](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e43e-130">If successful, this method returns `200 OK` response code and [Range](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e43e-131">示例</span><span class="sxs-lookup"><span data-stu-id="3e43e-131">Example</span></span>
<span data-ttu-id="3e43e-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3e43e-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3e43e-133">请求</span><span class="sxs-lookup"><span data-stu-id="3e43e-133">Request</span></span>
<span data-ttu-id="3e43e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3e43e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "table_headerrowrange"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange
```

##### <a name="response"></a><span data-ttu-id="3e43e-135">响应</span><span class="sxs-lookup"><span data-stu-id="3e43e-135">Response</span></span>
<span data-ttu-id="3e43e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3e43e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Table: HeaderRowRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->