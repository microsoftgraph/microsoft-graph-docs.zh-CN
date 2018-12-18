---
title: 获取 TableRow
description: 检索 tablerow 对象的属性和关系。
author: lumine2008
ms.openlocfilehash: 472906f105a4f43de938e903c43b73adf6cb8045
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329363"
---
# <a name="get-tablerow"></a><span data-ttu-id="c25ed-103">获取 TableRow</span><span class="sxs-lookup"><span data-stu-id="c25ed-103">Get TableRow</span></span>

> <span data-ttu-id="c25ed-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c25ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c25ed-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c25ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c25ed-106">检索 tablerow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c25ed-106">Retrieve the properties and relationships of tablerow object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c25ed-107">权限</span><span class="sxs-lookup"><span data-stu-id="c25ed-107">Permissions</span></span>
<span data-ttu-id="c25ed-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c25ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c25ed-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c25ed-110">Permission type</span></span>      | <span data-ttu-id="c25ed-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c25ed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c25ed-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c25ed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c25ed-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c25ed-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c25ed-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c25ed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c25ed-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c25ed-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c25ed-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c25ed-116">Application</span></span> | <span data-ttu-id="c25ed-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c25ed-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c25ed-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c25ed-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/rows(<index>)
GET /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c25ed-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c25ed-119">Optional query parameters</span></span>
<span data-ttu-id="c25ed-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c25ed-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c25ed-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c25ed-121">Request headers</span></span>
| <span data-ttu-id="c25ed-122">Name</span><span class="sxs-lookup"><span data-stu-id="c25ed-122">Name</span></span>      |<span data-ttu-id="c25ed-123">说明</span><span class="sxs-lookup"><span data-stu-id="c25ed-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c25ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c25ed-124">Authorization</span></span>  | <span data-ttu-id="c25ed-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c25ed-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c25ed-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c25ed-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="c25ed-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c25ed-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c25ed-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c25ed-130">Request body</span></span>
<span data-ttu-id="c25ed-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c25ed-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c25ed-132">响应</span><span class="sxs-lookup"><span data-stu-id="c25ed-132">Response</span></span>

<span data-ttu-id="c25ed-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [TableRow](../resources/tablerow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c25ed-133">If successful, this method returns a `200 OK` response code and [TableRow](../resources/tablerow.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c25ed-134">示例</span><span class="sxs-lookup"><span data-stu-id="c25ed-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c25ed-135">请求</span><span class="sxs-lookup"><span data-stu-id="c25ed-135">Request</span></span>
<span data-ttu-id="c25ed-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c25ed-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tablerow"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)
```
##### <a name="response"></a><span data-ttu-id="c25ed-137">响应</span><span class="sxs-lookup"><span data-stu-id="c25ed-137">Response</span></span>
<span data-ttu-id="c25ed-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c25ed-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableRow"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 45

{
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get TableRow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->