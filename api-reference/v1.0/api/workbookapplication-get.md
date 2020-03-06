---
title: 获取 workbookApplication
description: 检索 workbookApplication 对象的属性和关系。
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: f03aeca5c15d26854954ecd4f459e5c0ab49cb4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508819"
---
# <a name="get-workbookapplication"></a><span data-ttu-id="e13b8-103">获取 workbookApplication</span><span class="sxs-lookup"><span data-stu-id="e13b8-103">Get workbookApplication</span></span>

<span data-ttu-id="e13b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e13b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e13b8-105">检索[workbookApplication](../resources/workbookapplication.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e13b8-105">Retrieve the properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e13b8-106">权限</span><span class="sxs-lookup"><span data-stu-id="e13b8-106">Permissions</span></span>
<span data-ttu-id="e13b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e13b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e13b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e13b8-109">Permission type</span></span>      | <span data-ttu-id="e13b8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e13b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e13b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e13b8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e13b8-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e13b8-112">Files.ReadWrite</span></span>   |
|<span data-ttu-id="e13b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e13b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e13b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e13b8-114">Not supported.</span></span>    |
|<span data-ttu-id="e13b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e13b8-115">Application</span></span> | <span data-ttu-id="e13b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e13b8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e13b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e13b8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```

## <a name="request-headers"></a><span data-ttu-id="e13b8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e13b8-118">Request headers</span></span>
| <span data-ttu-id="e13b8-119">名称</span><span class="sxs-lookup"><span data-stu-id="e13b8-119">Name</span></span>      |<span data-ttu-id="e13b8-120">说明</span><span class="sxs-lookup"><span data-stu-id="e13b8-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e13b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e13b8-121">Authorization</span></span>  | <span data-ttu-id="e13b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e13b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e13b8-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e13b8-124">Request body</span></span>
<span data-ttu-id="e13b8-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e13b8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e13b8-126">响应</span><span class="sxs-lookup"><span data-stu-id="e13b8-126">Response</span></span>

<span data-ttu-id="e13b8-127">如果成功，此方法在响应`200 OK`正文中返回响应代码和[workbookApplication](../resources/workbookapplication.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e13b8-127">If successful, this method returns a `200 OK` response code and a [workbookApplication](../resources/workbookapplication.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e13b8-128">示例</span><span class="sxs-lookup"><span data-stu-id="e13b8-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="e13b8-129">请求</span><span class="sxs-lookup"><span data-stu-id="e13b8-129">Request</span></span>
<span data-ttu-id="e13b8-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e13b8-130">Here is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e13b8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e13b8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookApplication"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/application
```
# <a name="c"></a>[<span data-ttu-id="e13b8-132">C#</span><span class="sxs-lookup"><span data-stu-id="e13b8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e13b8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e13b8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e13b8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e13b8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e13b8-135">Java</span><span class="sxs-lookup"><span data-stu-id="e13b8-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e13b8-136">响应</span><span class="sxs-lookup"><span data-stu-id="e13b8-136">Response</span></span>
<span data-ttu-id="e13b8-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e13b8-137">Here is an example of the response.</span></span> 

> <span data-ttu-id="e13b8-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e13b8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
