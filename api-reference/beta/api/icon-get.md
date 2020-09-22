---
title: 获取图标
description: 检索 icon 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: b9250047be24afd5e4946d076e46338336fa1b84
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001706"
---
# <a name="get-icon"></a><span data-ttu-id="9baed-103">获取图标</span><span class="sxs-lookup"><span data-stu-id="9baed-103">Get Icon</span></span>

<span data-ttu-id="9baed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9baed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9baed-105">检索 icon 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9baed-105">Retrieve the properties and relationships of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9baed-106">权限</span><span class="sxs-lookup"><span data-stu-id="9baed-106">Permissions</span></span>
<span data-ttu-id="9baed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9baed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9baed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9baed-109">Permission type</span></span>      | <span data-ttu-id="9baed-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9baed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9baed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9baed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9baed-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9baed-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9baed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9baed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9baed-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9baed-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9baed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9baed-115">Application</span></span> | <span data-ttu-id="9baed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9baed-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9baed-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9baed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/tables/{id|name}/sort/fields/icon
GET /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9baed-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9baed-118">Optional query parameters</span></span>
<span data-ttu-id="9baed-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9baed-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9baed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9baed-120">Request headers</span></span>
| <span data-ttu-id="9baed-121">名称</span><span class="sxs-lookup"><span data-stu-id="9baed-121">Name</span></span>      |<span data-ttu-id="9baed-122">说明</span><span class="sxs-lookup"><span data-stu-id="9baed-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9baed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9baed-123">Authorization</span></span>  | <span data-ttu-id="9baed-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9baed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9baed-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9baed-126">Request body</span></span>
<span data-ttu-id="9baed-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9baed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9baed-128">响应</span><span class="sxs-lookup"><span data-stu-id="9baed-128">Response</span></span>

<span data-ttu-id="9baed-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [workbookIcon](../resources/workbookicon.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9baed-129">If successful, this method returns a `200 OK` response code and [workbookIcon](../resources/workbookicon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9baed-130">示例</span><span class="sxs-lookup"><span data-stu-id="9baed-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9baed-131">请求</span><span class="sxs-lookup"><span data-stu-id="9baed-131">Request</span></span>
<span data-ttu-id="9baed-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9baed-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_icon"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
```
##### <a name="response"></a><span data-ttu-id="9baed-133">响应</span><span class="sxs-lookup"><span data-stu-id="9baed-133">Response</span></span>
<span data-ttu-id="9baed-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9baed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


