---
title: 获取 dataPolicyOperation
description: 检索 dataPolicyOperation 对象的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 60284a0664c693168aa4279a1c48a6a6278d45eb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039795"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="d8b9d-103">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d8b9d-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="d8b9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8b9d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d8b9d-105">检索 **dataPolicyOperation 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="d8b9d-105">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8b9d-106">权限</span><span class="sxs-lookup"><span data-stu-id="d8b9d-106">Permissions</span></span>
<span data-ttu-id="d8b9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8b9d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8b9d-109">Permission type</span></span>      | <span data-ttu-id="d8b9d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8b9d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8b9d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8b9d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="d8b9d-112">User.Export.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8b9d-112">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="d8b9d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8b9d-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d8b9d-114">不适用</span><span class="sxs-lookup"><span data-stu-id="d8b9d-114">Not applicable</span></span>  |
|<span data-ttu-id="d8b9d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8b9d-115">Application</span></span> | <span data-ttu-id="d8b9d-116">User.Export.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8b9d-116">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d8b9d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8b9d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d8b9d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8b9d-118">Request headers</span></span>
| <span data-ttu-id="d8b9d-119">名称</span><span class="sxs-lookup"><span data-stu-id="d8b9d-119">Name</span></span>      |<span data-ttu-id="d8b9d-120">说明</span><span class="sxs-lookup"><span data-stu-id="d8b9d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d8b9d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8b9d-121">Authorization</span></span>  | <span data-ttu-id="d8b9d-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d8b9d-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8b9d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8b9d-123">Request body</span></span>
<span data-ttu-id="d8b9d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d8b9d-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d8b9d-125">响应</span><span class="sxs-lookup"><span data-stu-id="d8b9d-125">Response</span></span>
<span data-ttu-id="d8b9d-126">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [dataPolicyOperation](../resources/datapolicyoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8b9d-126">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8b9d-127">示例</span><span class="sxs-lookup"><span data-stu-id="d8b9d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8b9d-128">请求</span><span class="sxs-lookup"><span data-stu-id="d8b9d-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d8b9d-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8b9d-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="d8b9d-130">C#</span><span class="sxs-lookup"><span data-stu-id="d8b9d-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8b9d-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8b9d-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8b9d-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8b9d-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8b9d-133">Java</span><span class="sxs-lookup"><span data-stu-id="d8b9d-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-datapolicyoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d8b9d-134">响应</span><span class="sxs-lookup"><span data-stu-id="d8b9d-134">Response</span></span>
><span data-ttu-id="d8b9d-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d8b9d-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

