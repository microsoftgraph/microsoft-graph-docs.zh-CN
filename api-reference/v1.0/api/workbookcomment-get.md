---
title: 获取 workbookComment
description: 检索 workbookcomment 对象的属性和关系。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: d67bd8f09658f64bcceded821dcc9564892275c5
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538747"
---
# <a name="get-workbookcomment"></a><span data-ttu-id="27d88-103">获取 workbookComment</span><span class="sxs-lookup"><span data-stu-id="27d88-103">Get workbookComment</span></span>

<span data-ttu-id="27d88-104">检索[workbookComment](../resources/workbookcomment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27d88-104">Retrieve the properties and relationships of a [workbookComment](../resources/workbookcomment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27d88-105">权限</span><span class="sxs-lookup"><span data-stu-id="27d88-105">Permissions</span></span>

<span data-ttu-id="27d88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27d88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27d88-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="27d88-108">Permission type</span></span>                        | <span data-ttu-id="27d88-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="27d88-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27d88-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27d88-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="27d88-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27d88-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="27d88-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27d88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27d88-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="27d88-113">Not supported.</span></span> |
| <span data-ttu-id="27d88-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="27d88-114">Application</span></span>                            | <span data-ttu-id="27d88-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="27d88-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27d88-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27d88-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/comments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="27d88-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="27d88-117">Request headers</span></span>

| <span data-ttu-id="27d88-118">名称</span><span class="sxs-lookup"><span data-stu-id="27d88-118">Name</span></span>      |<span data-ttu-id="27d88-119">说明</span><span class="sxs-lookup"><span data-stu-id="27d88-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="27d88-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="27d88-120">Authorization</span></span> | <span data-ttu-id="27d88-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="27d88-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27d88-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="27d88-123">Request body</span></span>

<span data-ttu-id="27d88-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="27d88-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27d88-125">响应</span><span class="sxs-lookup"><span data-stu-id="27d88-125">Response</span></span>

<span data-ttu-id="27d88-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[workbookComment](../resources/workbookcomment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="27d88-126">If successful, this method returns a `200 OK` response code and the requested [workbookComment](../resources/workbookcomment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27d88-127">示例</span><span class="sxs-lookup"><span data-stu-id="27d88-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27d88-128">请求</span><span class="sxs-lookup"><span data-stu-id="27d88-128">Request</span></span>

<span data-ttu-id="27d88-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="27d88-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="27d88-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="27d88-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcomment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/drive/root/workbook/comments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="27d88-131">C#</span><span class="sxs-lookup"><span data-stu-id="27d88-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27d88-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27d88-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="27d88-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27d88-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="27d88-134">Java</span><span class="sxs-lookup"><span data-stu-id="27d88-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27d88-135">响应</span><span class="sxs-lookup"><span data-stu-id="27d88-135">Response</span></span>

<span data-ttu-id="27d88-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="27d88-136">The following is an example of the response.</span></span>

> <span data-ttu-id="27d88-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="27d88-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "content": "This is my comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookComment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
