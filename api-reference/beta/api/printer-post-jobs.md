---
title: 创建 printJob
description: 为打印机创建新的 printJob。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: bf7ef738b82482caddef6a64e1c0f0f8eeb47c27
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947777"
---
# <a name="create-printjob"></a><span data-ttu-id="fa3b5-103">创建 printJob</span><span class="sxs-lookup"><span data-stu-id="fa3b5-103">Create printJob</span></span>

<span data-ttu-id="fa3b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa3b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa3b5-105">为[打印机](../resources/printer.md)创建新的[printJob](../resources/printJob.md) 。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="fa3b5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fa3b5-106">Permissions</span></span>
<span data-ttu-id="fa3b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fa3b5-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="fa3b5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa3b5-110">Permission type</span></span> | <span data-ttu-id="fa3b5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa3b5-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fa3b5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa3b5-112">Delegated (work or school account)</span></span>| <span data-ttu-id="fa3b5-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="fa3b5-113">Users.Read.All</span></span> |
|<span data-ttu-id="fa3b5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa3b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa3b5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-115">Not Supported.</span></span>|
|<span data-ttu-id="fa3b5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa3b5-116">Application</span></span>|<span data-ttu-id="fa3b5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa3b5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa3b5-118">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="fa3b5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa3b5-119">Request headers</span></span>
| <span data-ttu-id="fa3b5-120">名称</span><span class="sxs-lookup"><span data-stu-id="fa3b5-120">Name</span></span>      |<span data-ttu-id="fa3b5-121">说明</span><span class="sxs-lookup"><span data-stu-id="fa3b5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa3b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa3b5-122">Authorization</span></span> | <span data-ttu-id="fa3b5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fa3b5-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="fa3b5-125">Content-type</span></span>  | <span data-ttu-id="fa3b5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fa3b5-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa3b5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa3b5-128">Request body</span></span>
<span data-ttu-id="fa3b5-129">在请求正文中，提供[printJob](../resources/printjob.md)对象的 JSON 表示形式，包括一个[printDocument](../resources/printDocument.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-129">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object, including one [printDocument](../resources/printDocument.md) object.</span></span> <span data-ttu-id="fa3b5-130">在创建资源的过程中会自动设置作业和文档 Id。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-130">The job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="fa3b5-131">目前，通用打印支持每个**printJob**对象仅支持一个**printDocument** 。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-131">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="fa3b5-132">响应</span><span class="sxs-lookup"><span data-stu-id="fa3b5-132">Response</span></span>
<span data-ttu-id="fa3b5-133">如果成功，此方法在响应`201 Created`正文中返回响应代码和[printJob](../resources/printjob.md)对象以及关联的[printDocument](../resources/printDocument.md) 。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-133">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="fa3b5-134">示例</span><span class="sxs-lookup"><span data-stu-id="fa3b5-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa3b5-135">请求</span><span class="sxs-lookup"><span data-stu-id="fa3b5-135">Request</span></span>
<span data-ttu-id="fa3b5-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa3b5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa3b5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="javascript"></a>[<span data-ttu-id="fa3b5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa3b5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa3b5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa3b5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fa3b5-140">响应</span><span class="sxs-lookup"><span data-stu-id="fa3b5-140">Response</span></span>
<span data-ttu-id="fa3b5-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-141">The following is an example of the response.</span></span>
><span data-ttu-id="fa3b5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fa3b5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 425

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printJobs/$entity",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
      }
    }
  ]
}
```
