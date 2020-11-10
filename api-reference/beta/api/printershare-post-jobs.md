---
title: 为 printerShare 创建 printJob
description: 为 printerShare 创建新的 printJob。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1e04b2eb45f39326010eefdc302c9e14980a09ba
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968357"
---
# <a name="create-printjob-for-a-printershare"></a><span data-ttu-id="f155e-103">为 printerShare 创建 printJob</span><span class="sxs-lookup"><span data-stu-id="f155e-103">Create printJob for a printerShare</span></span>

<span data-ttu-id="f155e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f155e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f155e-105">为[printerShare](../resources/printerShare.md)创建新的[printJob](../resources/printJob.md) 。</span><span class="sxs-lookup"><span data-stu-id="f155e-105">Create a new [printJob](../resources/printJob.md) for a [printerShare](../resources/printerShare.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="f155e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f155e-106">Permissions</span></span>
<span data-ttu-id="f155e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f155e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f155e-109">除了以下权限之外，用户或应用程序的租户必须具有活动的通用打印订阅，并且拥有授予 [Get printerShare](printerShare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="f155e-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printerShare](printerShare-get.md) access.</span></span> <span data-ttu-id="f155e-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="f155e-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f155e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f155e-111">Permission type</span></span> | <span data-ttu-id="f155e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f155e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f155e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f155e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="f155e-114">PrintJob、ReadWriteBasic、PrintJob、All、ReadWriteBasic、All</span><span class="sxs-lookup"><span data-stu-id="f155e-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="f155e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f155e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f155e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f155e-116">Not Supported.</span></span>|
|<span data-ttu-id="f155e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f155e-117">Application</span></span>| <span data-ttu-id="f155e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f155e-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f155e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f155e-119">HTTP request</span></span>

```http
POST print/shares/{id}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="f155e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f155e-120">Request headers</span></span>
| <span data-ttu-id="f155e-121">名称</span><span class="sxs-lookup"><span data-stu-id="f155e-121">Name</span></span>      |<span data-ttu-id="f155e-122">说明</span><span class="sxs-lookup"><span data-stu-id="f155e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f155e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f155e-123">Authorization</span></span> | <span data-ttu-id="f155e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f155e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f155e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="f155e-126">Content-type</span></span>  | <span data-ttu-id="f155e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f155e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f155e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f155e-129">Request body</span></span>
<span data-ttu-id="f155e-130">在请求正文中，提供 [printJob](../resources/printjob.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f155e-130">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span>
<span data-ttu-id="f155e-131">PrintJob 对象应仅包含 **配置** 。</span><span class="sxs-lookup"><span data-stu-id="f155e-131">The printJob object should only contain **configuration**.</span></span> <span data-ttu-id="f155e-132">**配置** 的所有属性都可以为 null。</span><span class="sxs-lookup"><span data-stu-id="f155e-132">All properties of **configuration** are nullable.</span></span>
<span data-ttu-id="f155e-133">在创建资源的过程中，会自动设置所有其他字段，包括作业和文档 Id。</span><span class="sxs-lookup"><span data-stu-id="f155e-133">All other fields including job and document IDs are set automatically during resource creation.</span></span>

<span data-ttu-id="f155e-134">目前，通用打印支持每个 **printJob** 对象仅支持一个 **printDocument** 。</span><span class="sxs-lookup"><span data-stu-id="f155e-134">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="f155e-135">响应</span><span class="sxs-lookup"><span data-stu-id="f155e-135">Response</span></span>
<span data-ttu-id="f155e-136">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [printJob](../resources/printjob.md) 对象以及关联的 [printDocument](../resources/printDocument.md) 。</span><span class="sxs-lookup"><span data-stu-id="f155e-136">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 
## <a name="example"></a><span data-ttu-id="f155e-137">示例</span><span class="sxs-lookup"><span data-stu-id="f155e-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="f155e-138">请求</span><span class="sxs-lookup"><span data-stu-id="f155e-138">Request</span></span>
<span data-ttu-id="f155e-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f155e-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f155e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f155e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs
Content-type: application/json

{
  "configuration": {
    "feedOrientation": "longEdgeFirst",
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "quality": "medium",
    "dpi": 600,
    "orientation": "landscape",
    "copies": 1,
    "duplexMode": "oneSided",
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    },
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false
  }
}
```
# <a name="c"></a>[<span data-ttu-id="f155e-141">C#</span><span class="sxs-lookup"><span data-stu-id="f155e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f155e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f155e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f155e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f155e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f155e-144">Java</span><span class="sxs-lookup"><span data-stu-id="f155e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="f155e-145">响应</span><span class="sxs-lookup"><span data-stu-id="f155e-145">Response</span></span>
<span data-ttu-id="f155e-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f155e-146">The following is an example of the response.</span></span>
><span data-ttu-id="f155e-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f155e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1065

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printJobs/$entity",
  "id": "1825",
  "createdDateTime": "2020-10-14T05:16:49-07:00",
  "isFetchable": false,
  "redirectedFrom": null,
  "redirectedTo": null,
  "createdBy": {
    "id": "{userId}",
    "displayName": "{username}",
    "ipAddress": null,
    "userPrincipalName": "{userupn}"
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet.",
    "isAcquiredByPrinter": false,
    "details": [
      "uploadPending"
    ]
  },
  "configuration": {
    "quality": "medium",
    "dpi": 600,
    "feedOrientation": "longEdgeFirst",
    "orientation": "landscape",
    "duplexMode": "oneSided",
    "copies": 1,
    "colorMode": "blackAndWhite",
    "inputBin": "by-pass-tray",
    "outputBin": "output-tray",
    "mediaSize": "A4",
    "mediaType": "stationery",
    "finishings": null,
    "pagesPerSheet": 1,
    "multipageLayout": "clockwiseFromBottomLeft",
    "collate": false,
    "scaling": "shrinkToFit",
    "fitPdfToPage": false,
    "pageRanges": [
      {
        "start": 1,
        "end": 1
      }
    ],
    "margin": {
      "top": 0,
      "bottom": 0,
      "left": 0,
      "right": 0
    }
  },
  "documents": [
    {
      "id": "1477576d-5dab-4ea9-865c-c0b82cd70bd5",
      "displayName": "",
      "contentType": "",
      "size": 0
    }
  ]
}
```
