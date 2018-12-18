---
title: 列出名称
description: '检索与工作表关联的已命名项的列表。 '
author: lumine2008
ms.openlocfilehash: 3d9a1cdff9c7903622309028c2d5e73a5868d219
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333283"
---
# <a name="list-names"></a><span data-ttu-id="a9539-103">列出名称</span><span class="sxs-lookup"><span data-stu-id="a9539-103">List names</span></span>

<span data-ttu-id="a9539-104">检索与工作表关联的已命名项的列表。</span><span class="sxs-lookup"><span data-stu-id="a9539-104">Retrieve a list of named item associated with the worksheet.</span></span> 
## <a name="permissions"></a><span data-ttu-id="a9539-105">权限</span><span class="sxs-lookup"><span data-stu-id="a9539-105">Permissions</span></span>
<span data-ttu-id="a9539-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9539-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9539-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9539-108">Permission type</span></span>      | <span data-ttu-id="a9539-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9539-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9539-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9539-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9539-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9539-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a9539-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9539-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9539-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9539-113">Not supported.</span></span>    |
|<span data-ttu-id="a9539-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9539-114">Application</span></span> | <span data-ttu-id="a9539-115">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9539-115">Sites.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9539-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9539-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/worksheets({id|name})/names
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a9539-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a9539-117">Optional query parameters</span></span>
<span data-ttu-id="a9539-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a9539-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9539-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9539-119">Request headers</span></span>
| <span data-ttu-id="a9539-120">Name</span><span class="sxs-lookup"><span data-stu-id="a9539-120">Name</span></span>      |<span data-ttu-id="a9539-121">说明</span><span class="sxs-lookup"><span data-stu-id="a9539-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9539-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9539-122">Authorization</span></span>  | <span data-ttu-id="a9539-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9539-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9539-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a9539-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a9539-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="a9539-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9539-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9539-128">Request body</span></span>
<span data-ttu-id="a9539-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9539-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9539-130">响应</span><span class="sxs-lookup"><span data-stu-id="a9539-130">Response</span></span>

<span data-ttu-id="a9539-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[WorkbookNamedItem](../resources/nameditem.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a9539-131">If successful, this method returns a `200 OK` response code and collection of [WorkbookNamedItem](../resources/nameditem.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9539-132">示例</span><span class="sxs-lookup"><span data-stu-id="a9539-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9539-133">请求</span><span class="sxs-lookup"><span data-stu-id="a9539-133">Request</span></span>
<span data-ttu-id="a9539-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9539-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tables"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/names
```
##### <a name="response"></a><span data-ttu-id="a9539-135">响应</span><span class="sxs-lookup"><span data-stu-id="a9539-135">Response</span></span>
<span data-ttu-id="a9539-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9539-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookNamedItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 158

{
  "value": [
    {
      "name": "myrange",
      "scope": "worksheet"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tables",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
