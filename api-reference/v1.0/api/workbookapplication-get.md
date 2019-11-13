---
title: 获取 workbookApplication
description: 检索 workbookApplication 对象的属性和关系。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 06d144097eb7689b75f6ae0e7be941e254cc9592
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302313"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="9624b-103">获取 workbookApplication</span><span class="sxs-lookup"><span data-stu-id="9624b-103">Get workbookApplication</span></span>

<span data-ttu-id="9624b-104">检索[workbookApplication](../resources/workbookapplication.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9624b-104">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9624b-105">权限</span><span class="sxs-lookup"><span data-stu-id="9624b-105">Permissions</span></span>
<span data-ttu-id="9624b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9624b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9624b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9624b-108">Permission type</span></span>      | <span data-ttu-id="9624b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9624b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9624b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9624b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9624b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9624b-111">Files.ReadWrite</span></span>   |
|<span data-ttu-id="9624b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9624b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9624b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9624b-113">Not supported.</span></span>    |
|<span data-ttu-id="9624b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9624b-114">Application</span></span> | <span data-ttu-id="9624b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9624b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9624b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9624b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```

## <a name="request-headers"></a><span data-ttu-id="9624b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9624b-117">Request headers</span></span>
| <span data-ttu-id="9624b-118">名称</span><span class="sxs-lookup"><span data-stu-id="9624b-118">Name</span></span>      |<span data-ttu-id="9624b-119">说明</span><span class="sxs-lookup"><span data-stu-id="9624b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9624b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9624b-120">Authorization</span></span>  | <span data-ttu-id="9624b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9624b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9624b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9624b-123">Request body</span></span>
<span data-ttu-id="9624b-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9624b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9624b-125">响应</span><span class="sxs-lookup"><span data-stu-id="9624b-125">Response</span></span>

<span data-ttu-id="9624b-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[workbookApplication](../resources/workbookapplication.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9624b-126">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9624b-127">示例</span><span class="sxs-lookup"><span data-stu-id="9624b-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="9624b-128">请求</span><span class="sxs-lookup"><span data-stu-id="9624b-128">Request</span></span>
<span data-ttu-id="9624b-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9624b-129">Here is an example of a request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9624b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9624b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9624b-131">C#</span><span class="sxs-lookup"><span data-stu-id="9624b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9624b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9624b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9624b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9624b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9624b-134">Java</span><span class="sxs-lookup"><span data-stu-id="9624b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9624b-135">响应</span><span class="sxs-lookup"><span data-stu-id="9624b-135">Response</span></span>
<span data-ttu-id="9624b-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9624b-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="9624b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9624b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
