---
title: 获取 dataPolicyOperation
description: 检索 dataPolicyOperation 对象的属性。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f0f02e526e11962c8ab2f6573d6090535b46a296
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326048"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="0b06b-103">获取 dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="0b06b-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="0b06b-104">检索 dataPolicyOperation 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b06b-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b06b-105">权限</span><span class="sxs-lookup"><span data-stu-id="0b06b-105">Permissions</span></span>
<span data-ttu-id="0b06b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b06b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b06b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b06b-108">Permission type</span></span>      | <span data-ttu-id="0b06b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b06b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b06b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b06b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="0b06b-111">Export. all 和 user. all</span><span class="sxs-lookup"><span data-stu-id="0b06b-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="0b06b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b06b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0b06b-113">不适用</span><span class="sxs-lookup"><span data-stu-id="0b06b-113">Not applicable</span></span>  |
|<span data-ttu-id="0b06b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b06b-114">Application</span></span> | <span data-ttu-id="0b06b-115">Export. all 和 user. all</span><span class="sxs-lookup"><span data-stu-id="0b06b-115">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0b06b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b06b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0b06b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b06b-117">Request headers</span></span>
| <span data-ttu-id="0b06b-118">名称</span><span class="sxs-lookup"><span data-stu-id="0b06b-118">Name</span></span>      |<span data-ttu-id="0b06b-119">说明</span><span class="sxs-lookup"><span data-stu-id="0b06b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b06b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b06b-120">Authorization</span></span>  | <span data-ttu-id="0b06b-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0b06b-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b06b-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b06b-122">Request body</span></span>
<span data-ttu-id="0b06b-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b06b-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0b06b-124">响应</span><span class="sxs-lookup"><span data-stu-id="0b06b-124">Response</span></span>
<span data-ttu-id="0b06b-125">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[dataPolicyOperation](../resources/datapolicyoperation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b06b-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b06b-126">示例</span><span class="sxs-lookup"><span data-stu-id="0b06b-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b06b-127">请求</span><span class="sxs-lookup"><span data-stu-id="0b06b-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="0b06b-128">响应</span><span class="sxs-lookup"><span data-stu-id="0b06b-128">Response</span></span>
<span data-ttu-id="0b06b-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b06b-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
