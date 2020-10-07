---
title: 创建 printJob
description: 为打印机创建新的 printJob。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a96128756744d790f631cd69cd669b4172593999
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372846"
---
# <a name="create-printjob"></a><span data-ttu-id="c1d87-103">创建 printJob</span><span class="sxs-lookup"><span data-stu-id="c1d87-103">Create printJob</span></span>

<span data-ttu-id="c1d87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1d87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1d87-105">为[打印机](../resources/printer.md)创建新的[printJob](../resources/printJob.md) 。</span><span class="sxs-lookup"><span data-stu-id="c1d87-105">Create a new [printJob](../resources/printJob.md) for a [printer](../resources/printer.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c1d87-106">权限</span><span class="sxs-lookup"><span data-stu-id="c1d87-106">Permissions</span></span>
<span data-ttu-id="c1d87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1d87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c1d87-109">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且具有授予 [获取打印机](printer-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="c1d87-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span> <span data-ttu-id="c1d87-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="c1d87-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="c1d87-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1d87-111">Permission type</span></span> | <span data-ttu-id="c1d87-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1d87-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c1d87-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1d87-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c1d87-114">PrintJob、ReadWriteBasic、PrintJob、All、ReadWriteBasic、All</span><span class="sxs-lookup"><span data-stu-id="c1d87-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="c1d87-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1d87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1d87-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1d87-116">Not Supported.</span></span>|
|<span data-ttu-id="c1d87-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1d87-117">Application</span></span>| <span data-ttu-id="c1d87-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1d87-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1d87-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1d87-119">HTTP request</span></span>

```http
POST print/printers/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="c1d87-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1d87-120">Request headers</span></span>
| <span data-ttu-id="c1d87-121">名称</span><span class="sxs-lookup"><span data-stu-id="c1d87-121">Name</span></span>      |<span data-ttu-id="c1d87-122">说明</span><span class="sxs-lookup"><span data-stu-id="c1d87-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c1d87-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1d87-123">Authorization</span></span> | <span data-ttu-id="c1d87-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1d87-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1d87-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="c1d87-126">Content-type</span></span>  | <span data-ttu-id="c1d87-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c1d87-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1d87-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1d87-129">Request body</span></span>
<span data-ttu-id="c1d87-130">在请求正文中，提供 [printJob](../resources/printjob.md) 对象的 JSON 表示形式，包括一个 [printDocument](../resources/printDocument.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c1d87-130">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object, including one [printDocument](../resources/printDocument.md) object.</span></span> <span data-ttu-id="c1d87-131">在创建资源的过程中会自动设置作业和文档 Id。</span><span class="sxs-lookup"><span data-stu-id="c1d87-131">The job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="c1d87-132">目前，通用打印支持每个**printJob**对象仅支持一个**printDocument** 。</span><span class="sxs-lookup"><span data-stu-id="c1d87-132">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="c1d87-133">响应</span><span class="sxs-lookup"><span data-stu-id="c1d87-133">Response</span></span>
<span data-ttu-id="c1d87-134">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [printJob](../resources/printjob.md) 对象以及关联的 [printDocument](../resources/printDocument.md) 。</span><span class="sxs-lookup"><span data-stu-id="c1d87-134">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="c1d87-135">示例</span><span class="sxs-lookup"><span data-stu-id="c1d87-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1d87-136">请求</span><span class="sxs-lookup"><span data-stu-id="c1d87-136">Request</span></span>
<span data-ttu-id="c1d87-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1d87-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c1d87-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1d87-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="javascript"></a>[<span data-ttu-id="c1d87-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1d87-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1d87-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1d87-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1d87-141">响应</span><span class="sxs-lookup"><span data-stu-id="c1d87-141">Response</span></span>
<span data-ttu-id="c1d87-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1d87-142">The following is an example of the response.</span></span>
><span data-ttu-id="c1d87-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1d87-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
