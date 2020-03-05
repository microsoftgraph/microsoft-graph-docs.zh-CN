---
title: 获取 dataPolicyOperation
description: 检索 dataPolicyOperation 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ce26de4e8dadd58d7a3a337b1c8217d3db1d5eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436116"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="97213-103">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="97213-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="97213-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="97213-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97213-105">检索 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="97213-105">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97213-106">权限</span><span class="sxs-lookup"><span data-stu-id="97213-106">Permissions</span></span>
<span data-ttu-id="97213-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97213-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97213-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="97213-109">Permission type</span></span>      | <span data-ttu-id="97213-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97213-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97213-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97213-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="97213-112">Export. All 和 User. All</span><span class="sxs-lookup"><span data-stu-id="97213-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="97213-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97213-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="97213-114">不适用</span><span class="sxs-lookup"><span data-stu-id="97213-114">Not applicable</span></span>  |
|<span data-ttu-id="97213-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="97213-115">Application</span></span> | <span data-ttu-id="97213-116">Export. All 和 User. All</span><span class="sxs-lookup"><span data-stu-id="97213-116">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="97213-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97213-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="97213-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="97213-118">Request headers</span></span>
| <span data-ttu-id="97213-119">名称</span><span class="sxs-lookup"><span data-stu-id="97213-119">Name</span></span>      |<span data-ttu-id="97213-120">说明</span><span class="sxs-lookup"><span data-stu-id="97213-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="97213-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97213-121">Authorization</span></span>  | <span data-ttu-id="97213-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="97213-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="97213-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="97213-123">Request body</span></span>
<span data-ttu-id="97213-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97213-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="97213-125">响应</span><span class="sxs-lookup"><span data-stu-id="97213-125">Response</span></span>
<span data-ttu-id="97213-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[dataPolicyOperation](../resources/datapolicyoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="97213-126">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97213-127">示例</span><span class="sxs-lookup"><span data-stu-id="97213-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97213-128">请求</span><span class="sxs-lookup"><span data-stu-id="97213-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97213-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="97213-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="97213-130">C#</span><span class="sxs-lookup"><span data-stu-id="97213-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97213-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97213-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97213-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97213-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="97213-133">响应</span><span class="sxs-lookup"><span data-stu-id="97213-133">Response</span></span>
<span data-ttu-id="97213-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97213-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
