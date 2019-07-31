---
title: 获取图标
description: 检索 icon 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 8909f1fb610a664c4d2fe95f73a74abc4707f75c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953246"
---
# <a name="get-icon"></a><span data-ttu-id="c8c34-103">获取图标</span><span class="sxs-lookup"><span data-stu-id="c8c34-103">Get Icon</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8c34-104">检索 icon 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8c34-104">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c8c34-105">权限</span><span class="sxs-lookup"><span data-stu-id="c8c34-105">Permissions</span></span>
<span data-ttu-id="c8c34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8c34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8c34-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8c34-108">Permission type</span></span>      | <span data-ttu-id="c8c34-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8c34-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8c34-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8c34-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c8c34-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8c34-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8c34-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8c34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8c34-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c8c34-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c8c34-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8c34-114">Application</span></span> | <span data-ttu-id="c8c34-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8c34-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8c34-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8c34-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c8c34-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c8c34-117">Optional query parameters</span></span>
<span data-ttu-id="c8c34-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c8c34-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8c34-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8c34-119">Request headers</span></span>
| <span data-ttu-id="c8c34-120">名称</span><span class="sxs-lookup"><span data-stu-id="c8c34-120">Name</span></span>      |<span data-ttu-id="c8c34-121">说明</span><span class="sxs-lookup"><span data-stu-id="c8c34-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c8c34-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8c34-122">Authorization</span></span>  | <span data-ttu-id="c8c34-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8c34-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8c34-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8c34-125">Request body</span></span>
<span data-ttu-id="c8c34-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c8c34-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8c34-127">响应</span><span class="sxs-lookup"><span data-stu-id="c8c34-127">Response</span></span>

<span data-ttu-id="c8c34-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[workbookIcon](../resources/workbookicon.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c8c34-128">If successful, this method returns a `200 OK` response code and [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c8c34-129">示例</span><span class="sxs-lookup"><span data-stu-id="c8c34-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c8c34-130">请求</span><span class="sxs-lookup"><span data-stu-id="c8c34-130">Request</span></span>
<span data-ttu-id="c8c34-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8c34-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="c8c34-132">响应</span><span class="sxs-lookup"><span data-stu-id="c8c34-132">Response</span></span>
<span data-ttu-id="c8c34-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8c34-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get Icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
