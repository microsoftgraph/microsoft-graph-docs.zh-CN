---
title: 列出边框
description: 检索 rangeborder 对象的列表。
ms.openlocfilehash: 26648b7d713b76a6f5d4d5171d2f20a0816a0dc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047001"
---
# <a name="list-borders"></a><span data-ttu-id="aba5a-103">列出边框</span><span class="sxs-lookup"><span data-stu-id="aba5a-103">List borders</span></span>

> <span data-ttu-id="aba5a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aba5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aba5a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aba5a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aba5a-106">检索 rangeborder 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="aba5a-106">Retrieve a list of rangeborder objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="aba5a-107">权限</span><span class="sxs-lookup"><span data-stu-id="aba5a-107">Permissions</span></span>
<span data-ttu-id="aba5a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aba5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aba5a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aba5a-110">Permission type</span></span>      | <span data-ttu-id="aba5a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aba5a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aba5a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aba5a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aba5a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aba5a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aba5a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aba5a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aba5a-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aba5a-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="aba5a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aba5a-116">Application</span></span> | <span data-ttu-id="aba5a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aba5a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aba5a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aba5a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/names(<name>)/range/format/borders
GET /workbook/worksheets/{id|name}/range(address='<address>')/format/borders
GET /workbook/tables/{id|name}/columns/{id|name}/range/format/borders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aba5a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aba5a-119">Optional query parameters</span></span>
<span data-ttu-id="aba5a-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aba5a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aba5a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="aba5a-121">Request headers</span></span>
| <span data-ttu-id="aba5a-122">名称</span><span class="sxs-lookup"><span data-stu-id="aba5a-122">Name</span></span>      |<span data-ttu-id="aba5a-123">说明</span><span class="sxs-lookup"><span data-stu-id="aba5a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aba5a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aba5a-124">Authorization</span></span>  | <span data-ttu-id="aba5a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aba5a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aba5a-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="aba5a-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="aba5a-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="aba5a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aba5a-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="aba5a-130">Request body</span></span>
<span data-ttu-id="aba5a-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aba5a-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aba5a-132">响应</span><span class="sxs-lookup"><span data-stu-id="aba5a-132">Response</span></span>

<span data-ttu-id="aba5a-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [RangeBorder](../resources/rangeborder.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aba5a-133">If successful, this method returns a `200 OK` response code and collection of [RangeBorder](../resources/rangeborder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aba5a-134">示例</span><span class="sxs-lookup"><span data-stu-id="aba5a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aba5a-135">请求</span><span class="sxs-lookup"><span data-stu-id="aba5a-135">Request</span></span>
<span data-ttu-id="aba5a-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aba5a-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_borders"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders
```
##### <a name="response"></a><span data-ttu-id="aba5a-137">响应</span><span class="sxs-lookup"><span data-stu-id="aba5a-137">Response</span></span>
<span data-ttu-id="aba5a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aba5a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 185

{
  "value": [
    {
      "id": "id-value",
      "color": "color-value",
      "style": "style-value",
      "sideIndex": "sideIndex-value",
      "weight": "weight-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List borders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->