---
title: 获取 dataPolicyOperation
description: 检索 dataPolicyOperation 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01cf28480b8b0d8f54bba08fb74e46a633000b2f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276375"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="9371f-103">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="9371f-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="9371f-104">检索**dataPolicyOperation**对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9371f-104">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9371f-105">权限</span><span class="sxs-lookup"><span data-stu-id="9371f-105">Permissions</span></span>
<span data-ttu-id="9371f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9371f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9371f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9371f-108">Permission type</span></span>      | <span data-ttu-id="9371f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9371f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9371f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9371f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9371f-111">将用户导出为 All、User、Read。 All</span><span class="sxs-lookup"><span data-stu-id="9371f-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="9371f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9371f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9371f-113">不适用</span><span class="sxs-lookup"><span data-stu-id="9371f-113">Not applicable</span></span>  |
|<span data-ttu-id="9371f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9371f-114">Application</span></span> | <span data-ttu-id="9371f-115">将用户导出为 All、User、Read。 All</span><span class="sxs-lookup"><span data-stu-id="9371f-115">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9371f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9371f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9371f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9371f-117">Request headers</span></span>
| <span data-ttu-id="9371f-118">名称</span><span class="sxs-lookup"><span data-stu-id="9371f-118">Name</span></span>      |<span data-ttu-id="9371f-119">说明</span><span class="sxs-lookup"><span data-stu-id="9371f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9371f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9371f-120">Authorization</span></span>  | <span data-ttu-id="9371f-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9371f-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9371f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="9371f-122">Request body</span></span>
<span data-ttu-id="9371f-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9371f-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9371f-124">响应</span><span class="sxs-lookup"><span data-stu-id="9371f-124">Response</span></span>
<span data-ttu-id="9371f-125">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[dataPolicyOperation](../resources/datapolicyoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9371f-125">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9371f-126">示例</span><span class="sxs-lookup"><span data-stu-id="9371f-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9371f-127">请求</span><span class="sxs-lookup"><span data-stu-id="9371f-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="9371f-128">响应</span><span class="sxs-lookup"><span data-stu-id="9371f-128">Response</span></span>
><span data-ttu-id="9371f-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9371f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="9371f-131">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9371f-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9371f-132">C#</span><span class="sxs-lookup"><span data-stu-id="9371f-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9371f-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="9371f-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9371f-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="9371f-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
