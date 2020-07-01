---
title: 列出作业
description: 检索与打印机关联的打印作业的列表。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2f0f539f902bd1b83c8efd046af35b0deb28ed05
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006700"
---
# <a name="list-jobs"></a><span data-ttu-id="951be-103">列出作业</span><span class="sxs-lookup"><span data-stu-id="951be-103">List jobs</span></span>

<span data-ttu-id="951be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="951be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="951be-105">检索与[打印机](../resources/printer.md)关联的打印作业的列表。</span><span class="sxs-lookup"><span data-stu-id="951be-105">Retrieve a list of print jobs associated with the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="951be-106">权限</span><span class="sxs-lookup"><span data-stu-id="951be-106">Permissions</span></span>
<span data-ttu-id="951be-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="951be-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="951be-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="951be-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="951be-109">若要使用通用打印服务，用户或应用程序的租户必须具有活动的通用打印订阅、授予 "[获取打印机](printer-get.md)访问" 权限的权限以及下表中列出的权限之一。</span><span class="sxs-lookup"><span data-stu-id="951be-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="951be-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="951be-110">Permission type</span></span> | <span data-ttu-id="951be-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="951be-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="951be-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="951be-112">Delegated (work or school account)</span></span>| <span data-ttu-id="951be-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="951be-113">Users.Read.All</span></span> |
|<span data-ttu-id="951be-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="951be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="951be-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="951be-115">Not Supported.</span></span>|
|<span data-ttu-id="951be-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="951be-116">Application</span></span>| <span data-ttu-id="951be-117">PrintJob、PrintJob、PrintJob、all、all、All 和 All。</span><span class="sxs-lookup"><span data-stu-id="951be-117">PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="951be-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="951be-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="951be-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="951be-119">Optional query parameters</span></span>
<span data-ttu-id="951be-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="951be-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="951be-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="951be-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="951be-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="951be-122">Exceptions</span></span>
<span data-ttu-id="951be-123">某些运算符不受支持： `$count` 、 `$search` 、 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="951be-123">Some operators are not supported: `$count`, `$search`, `$filter`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="951be-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="951be-124">Request headers</span></span>
| <span data-ttu-id="951be-125">名称</span><span class="sxs-lookup"><span data-stu-id="951be-125">Name</span></span>      |<span data-ttu-id="951be-126">说明</span><span class="sxs-lookup"><span data-stu-id="951be-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="951be-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="951be-127">Authorization</span></span> | <span data-ttu-id="951be-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="951be-128">Bearer {token}.</span></span> <span data-ttu-id="951be-129">Required.</span><span class="sxs-lookup"><span data-stu-id="951be-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="951be-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="951be-130">Request body</span></span>
<span data-ttu-id="951be-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="951be-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="951be-132">响应</span><span class="sxs-lookup"><span data-stu-id="951be-132">Response</span></span>
<span data-ttu-id="951be-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[printJob](../resources/printjob.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="951be-133">If successful, this method returns a `200 OK` response code and collection of [printJob](../resources/printjob.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="951be-134">示例</span><span class="sxs-lookup"><span data-stu-id="951be-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="951be-135">请求</span><span class="sxs-lookup"><span data-stu-id="951be-135">Request</span></span>
<span data-ttu-id="951be-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="951be-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="951be-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="951be-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[<span data-ttu-id="951be-138">C#</span><span class="sxs-lookup"><span data-stu-id="951be-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="951be-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="951be-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="951be-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="951be-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="951be-141">响应</span><span class="sxs-lookup"><span data-stu-id="951be-141">Response</span></span>
<span data-ttu-id="951be-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="951be-142">The following is an example of the response.</span></span>
><span data-ttu-id="951be-143">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="951be-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="951be-144">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="951be-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 461

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
