---
title: 获取 dataPolicyOperation
description: 检索 dataPolicyOperation 对象的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 13b2668d71dbf4bf1e1a708f46594caeacd7b8f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973386"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="53e12-103">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="53e12-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="53e12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53e12-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53e12-105">检索 **dataPolicyOperation** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="53e12-105">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53e12-106">权限</span><span class="sxs-lookup"><span data-stu-id="53e12-106">Permissions</span></span>
<span data-ttu-id="53e12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53e12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53e12-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53e12-109">Permission type</span></span>      | <span data-ttu-id="53e12-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53e12-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53e12-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53e12-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="53e12-112">将用户导出为 All、User、Read。 All</span><span class="sxs-lookup"><span data-stu-id="53e12-112">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="53e12-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53e12-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="53e12-114">不适用</span><span class="sxs-lookup"><span data-stu-id="53e12-114">Not applicable</span></span>  |
|<span data-ttu-id="53e12-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="53e12-115">Application</span></span> | <span data-ttu-id="53e12-116">将用户导出为 All、User、Read。 All</span><span class="sxs-lookup"><span data-stu-id="53e12-116">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="53e12-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53e12-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="53e12-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="53e12-118">Request headers</span></span>
| <span data-ttu-id="53e12-119">名称</span><span class="sxs-lookup"><span data-stu-id="53e12-119">Name</span></span>      |<span data-ttu-id="53e12-120">说明</span><span class="sxs-lookup"><span data-stu-id="53e12-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="53e12-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53e12-121">Authorization</span></span>  | <span data-ttu-id="53e12-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="53e12-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="53e12-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="53e12-123">Request body</span></span>
<span data-ttu-id="53e12-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53e12-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="53e12-125">响应</span><span class="sxs-lookup"><span data-stu-id="53e12-125">Response</span></span>
<span data-ttu-id="53e12-126">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [dataPolicyOperation](../resources/datapolicyoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53e12-126">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53e12-127">示例</span><span class="sxs-lookup"><span data-stu-id="53e12-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53e12-128">请求</span><span class="sxs-lookup"><span data-stu-id="53e12-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="53e12-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="53e12-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="53e12-130">C#</span><span class="sxs-lookup"><span data-stu-id="53e12-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53e12-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53e12-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53e12-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53e12-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53e12-133">Java</span><span class="sxs-lookup"><span data-stu-id="53e12-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-datapolicyoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="53e12-134">响应</span><span class="sxs-lookup"><span data-stu-id="53e12-134">Response</span></span>
><span data-ttu-id="53e12-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="53e12-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value", 
  "progress": "double-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

