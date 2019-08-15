---
title: 获取 dataPolicyOperation
description: 检索 dataPolicyOperation 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e19a0d078f38bc285bfa55815b72be9fa991b6d4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417702"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="1e141-103">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="1e141-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="1e141-104">检索 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1e141-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e141-105">权限</span><span class="sxs-lookup"><span data-stu-id="1e141-105">Permissions</span></span>
<span data-ttu-id="1e141-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e141-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e141-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e141-108">Permission type</span></span>      | <span data-ttu-id="1e141-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e141-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e141-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e141-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1e141-111">Export. All 和 User. All</span><span class="sxs-lookup"><span data-stu-id="1e141-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="1e141-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e141-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1e141-113">不适用</span><span class="sxs-lookup"><span data-stu-id="1e141-113">Not applicable</span></span>  |
|<span data-ttu-id="1e141-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e141-114">Application</span></span> | <span data-ttu-id="1e141-115">Export. All 和 User. All</span><span class="sxs-lookup"><span data-stu-id="1e141-115">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1e141-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e141-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1e141-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e141-117">Request headers</span></span>
| <span data-ttu-id="1e141-118">名称</span><span class="sxs-lookup"><span data-stu-id="1e141-118">Name</span></span>      |<span data-ttu-id="1e141-119">说明</span><span class="sxs-lookup"><span data-stu-id="1e141-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e141-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e141-120">Authorization</span></span>  | <span data-ttu-id="1e141-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="1e141-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e141-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e141-122">Request body</span></span>
<span data-ttu-id="1e141-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e141-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1e141-124">响应</span><span class="sxs-lookup"><span data-stu-id="1e141-124">Response</span></span>
<span data-ttu-id="1e141-125">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[dataPolicyOperation](../resources/datapolicyoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1e141-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e141-126">示例</span><span class="sxs-lookup"><span data-stu-id="1e141-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e141-127">请求</span><span class="sxs-lookup"><span data-stu-id="1e141-127">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1e141-128">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1e141-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1e141-129">C#</span><span class="sxs-lookup"><span data-stu-id="1e141-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1e141-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e141-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1e141-131">目标-C</span><span class="sxs-lookup"><span data-stu-id="1e141-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1e141-132">响应</span><span class="sxs-lookup"><span data-stu-id="1e141-132">Response</span></span>
<span data-ttu-id="1e141-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e141-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
