---
title: 获取 workbookApplication
description: 检索 workbookApplication 对象的属性和关系。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f265fe51ce37504b331ee735f9d3fa91979f5891
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/07/2019
ms.locfileid: "38023232"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="77d88-103">获取 workbookApplication</span><span class="sxs-lookup"><span data-stu-id="77d88-103">Get workbookApplication</span></span>

<span data-ttu-id="77d88-104">检索[workbookApplication](../resources/workbookapplication.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77d88-104">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77d88-105">权限</span><span class="sxs-lookup"><span data-stu-id="77d88-105">Permissions</span></span>
<span data-ttu-id="77d88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="77d88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77d88-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="77d88-108">Permission type</span></span>      | <span data-ttu-id="77d88-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="77d88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77d88-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77d88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77d88-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77d88-111">Files.ReadWrite</span></span>   |
|<span data-ttu-id="77d88-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77d88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77d88-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="77d88-113">Not supported.</span></span>    |
|<span data-ttu-id="77d88-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="77d88-114">Application</span></span> | <span data-ttu-id="77d88-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="77d88-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77d88-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77d88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```

## <a name="request-headers"></a><span data-ttu-id="77d88-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="77d88-117">Request headers</span></span>
| <span data-ttu-id="77d88-118">名称</span><span class="sxs-lookup"><span data-stu-id="77d88-118">Name</span></span>      |<span data-ttu-id="77d88-119">说明</span><span class="sxs-lookup"><span data-stu-id="77d88-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77d88-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="77d88-120">Authorization</span></span>  | <span data-ttu-id="77d88-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="77d88-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77d88-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="77d88-123">Request body</span></span>
<span data-ttu-id="77d88-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77d88-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77d88-125">响应</span><span class="sxs-lookup"><span data-stu-id="77d88-125">Response</span></span>

<span data-ttu-id="77d88-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[workbookApplication](../resources/workbookapplication.md)对象。</span><span class="sxs-lookup"><span data-stu-id="77d88-126">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77d88-127">示例</span><span class="sxs-lookup"><span data-stu-id="77d88-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="77d88-128">请求</span><span class="sxs-lookup"><span data-stu-id="77d88-128">Request</span></span>
<span data-ttu-id="77d88-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77d88-129">Here is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application
```

### <a name="response"></a><span data-ttu-id="77d88-130">响应</span><span class="sxs-lookup"><span data-stu-id="77d88-130">Response</span></span>
<span data-ttu-id="77d88-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="77d88-131">Here is an example of the response.</span></span> 

> <span data-ttu-id="77d88-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="77d88-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookApplication"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get workbookApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
