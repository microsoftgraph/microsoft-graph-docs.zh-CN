---
title: 获取图标
description: 检索 icon 对象的属性和关系。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8c05b0c9733515f80db0189e6f9cb7bbee6a0fd8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050442"
---
# <a name="get-icon"></a><span data-ttu-id="365b9-103">获取图标</span><span class="sxs-lookup"><span data-stu-id="365b9-103">Get Icon</span></span>

<span data-ttu-id="365b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="365b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="365b9-105">检索 icon 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="365b9-105">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="365b9-106">权限</span><span class="sxs-lookup"><span data-stu-id="365b9-106">Permissions</span></span>
<span data-ttu-id="365b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="365b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="365b9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="365b9-109">Permission type</span></span>      | <span data-ttu-id="365b9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="365b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="365b9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="365b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="365b9-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="365b9-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="365b9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="365b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="365b9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="365b9-114">Not supported.</span></span>    |
|<span data-ttu-id="365b9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="365b9-115">Application</span></span> | <span data-ttu-id="365b9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="365b9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="365b9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="365b9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/tables/{id|name}/sort/fields/icon
GET /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
GET /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="365b9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="365b9-118">Optional query parameters</span></span>
<span data-ttu-id="365b9-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="365b9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="365b9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="365b9-120">Request headers</span></span>
| <span data-ttu-id="365b9-121">名称</span><span class="sxs-lookup"><span data-stu-id="365b9-121">Name</span></span>      |<span data-ttu-id="365b9-122">说明</span><span class="sxs-lookup"><span data-stu-id="365b9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="365b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="365b9-123">Authorization</span></span>  | <span data-ttu-id="365b9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="365b9-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="365b9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="365b9-126">Request body</span></span>
<span data-ttu-id="365b9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="365b9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="365b9-128">响应</span><span class="sxs-lookup"><span data-stu-id="365b9-128">Response</span></span>

<span data-ttu-id="365b9-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Icon](../resources/icon.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="365b9-129">If successful, this method returns a `200 OK` response code and [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="365b9-130">示例</span><span class="sxs-lookup"><span data-stu-id="365b9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="365b9-131">请求</span><span class="sxs-lookup"><span data-stu-id="365b9-131">Request</span></span>
<span data-ttu-id="365b9-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="365b9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="365b9-133">响应</span><span class="sxs-lookup"><span data-stu-id="365b9-133">Response</span></span>
<span data-ttu-id="365b9-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="365b9-134">Here is an example of the response.</span></span> <span data-ttu-id="365b9-135">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="365b9-135">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->