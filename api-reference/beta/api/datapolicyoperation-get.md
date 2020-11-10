---
title: 获取 dataPolicyOperation
description: 检索 dataPolicyOperation 对象的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fb356740aa79a1980bfbe0b0305a362a4a0db7df
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956490"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="9250f-103">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="9250f-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="9250f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9250f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9250f-105">检索 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9250f-105">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9250f-106">权限</span><span class="sxs-lookup"><span data-stu-id="9250f-106">Permissions</span></span>
<span data-ttu-id="9250f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9250f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9250f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9250f-109">Permission type</span></span>      | <span data-ttu-id="9250f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9250f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9250f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9250f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="9250f-112">Export. All 和 User. All</span><span class="sxs-lookup"><span data-stu-id="9250f-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="9250f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9250f-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9250f-114">不适用</span><span class="sxs-lookup"><span data-stu-id="9250f-114">Not applicable</span></span>  |
|<span data-ttu-id="9250f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9250f-115">Application</span></span> | <span data-ttu-id="9250f-116">Export. All 和 User. All</span><span class="sxs-lookup"><span data-stu-id="9250f-116">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9250f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9250f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9250f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9250f-118">Request headers</span></span>
| <span data-ttu-id="9250f-119">名称</span><span class="sxs-lookup"><span data-stu-id="9250f-119">Name</span></span>      |<span data-ttu-id="9250f-120">说明</span><span class="sxs-lookup"><span data-stu-id="9250f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9250f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9250f-121">Authorization</span></span>  | <span data-ttu-id="9250f-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9250f-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9250f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="9250f-123">Request body</span></span>
<span data-ttu-id="9250f-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9250f-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9250f-125">响应</span><span class="sxs-lookup"><span data-stu-id="9250f-125">Response</span></span>
<span data-ttu-id="9250f-126">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [dataPolicyOperation](../resources/datapolicyoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9250f-126">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9250f-127">示例</span><span class="sxs-lookup"><span data-stu-id="9250f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9250f-128">请求</span><span class="sxs-lookup"><span data-stu-id="9250f-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9250f-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="9250f-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="9250f-130">C#</span><span class="sxs-lookup"><span data-stu-id="9250f-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9250f-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9250f-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9250f-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9250f-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9250f-133">Java</span><span class="sxs-lookup"><span data-stu-id="9250f-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-datapolicyoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9250f-134">响应</span><span class="sxs-lookup"><span data-stu-id="9250f-134">Response</span></span>
<span data-ttu-id="9250f-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9250f-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "progress": "double"
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


