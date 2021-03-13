---
title: 为 printerShare 创建 printJob
description: 为 printerShare 创建新的 printJob。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: eade8383dd6ec9868e529ad1045ec3aa56971385
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776856"
---
# <a name="create-printjob-for-a-printershare"></a><span data-ttu-id="8bacd-103">为 printerShare 创建 printJob</span><span class="sxs-lookup"><span data-stu-id="8bacd-103">Create printJob for a printerShare</span></span>
<span data-ttu-id="8bacd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bacd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="8bacd-105">为 printerShare 创建新的[printJob。](../resources/printJob.md) [](../resources/printerShare.md)</span><span class="sxs-lookup"><span data-stu-id="8bacd-105">Create a new [printJob](../resources/printJob.md) for a [printerShare](../resources/printerShare.md).</span></span> 

<span data-ttu-id="8bacd-106">此外，还创建一个与 printJob 关联的新[printDocument。](../resources/printDocument.md)</span><span class="sxs-lookup"><span data-stu-id="8bacd-106">Also creates a new [printDocument](../resources/printDocument.md) associated with the printJob.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bacd-107">权限</span><span class="sxs-lookup"><span data-stu-id="8bacd-107">Permissions</span></span>
<span data-ttu-id="8bacd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bacd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8bacd-110">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [获取 printerShare](printerShare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="8bacd-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printerShare](printerShare-get.md) access.</span></span> <span data-ttu-id="8bacd-111">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="8bacd-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="8bacd-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bacd-112">Permission type</span></span> | <span data-ttu-id="8bacd-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8bacd-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8bacd-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bacd-114">Delegated (work or school account)</span></span>| <span data-ttu-id="8bacd-115">PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bacd-115">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="8bacd-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bacd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bacd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bacd-117">Not Supported.</span></span>|
|<span data-ttu-id="8bacd-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bacd-118">Application</span></span>| <span data-ttu-id="8bacd-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bacd-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bacd-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bacd-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="8bacd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bacd-121">Request headers</span></span>
|<span data-ttu-id="8bacd-122">名称</span><span class="sxs-lookup"><span data-stu-id="8bacd-122">Name</span></span>|<span data-ttu-id="8bacd-123">说明</span><span class="sxs-lookup"><span data-stu-id="8bacd-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8bacd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bacd-124">Authorization</span></span>|<span data-ttu-id="8bacd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8bacd-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8bacd-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bacd-127">Content-Type</span></span>|<span data-ttu-id="8bacd-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="8bacd-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bacd-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bacd-130">Request body</span></span>
<span data-ttu-id="8bacd-131">在请求正文中，提供 [printJob](../resources/printjob.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bacd-131">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span> <span data-ttu-id="8bacd-132">printJob 对象应仅包含 **配置** 属性。</span><span class="sxs-lookup"><span data-stu-id="8bacd-132">The printJob object should only contain **configuration** property.</span></span> <span data-ttu-id="8bacd-133">配置的所有 **属性都** 为 null。</span><span class="sxs-lookup"><span data-stu-id="8bacd-133">All properties of **configuration** are nullable.</span></span> <span data-ttu-id="8bacd-134">所有其他字段（包括作业和文档 ID）将在资源创建过程中自动设置，并且不应在请求中提供。</span><span class="sxs-lookup"><span data-stu-id="8bacd-134">All other fields, including job and document IDs, are set automatically during resource creation and should not be provided in request.</span></span>

<span data-ttu-id="8bacd-135">目前，通用打印仅支持每个 **printJob** 对象一个 **printDocument。**</span><span class="sxs-lookup"><span data-stu-id="8bacd-135">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="8bacd-136">响应</span><span class="sxs-lookup"><span data-stu-id="8bacd-136">Response</span></span>

<span data-ttu-id="8bacd-137">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码[、printJob](../resources/printjob.md)对象和关联的[printDocument。](../resources/printDocument.md)</span><span class="sxs-lookup"><span data-stu-id="8bacd-137">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 

## <a name="examples"></a><span data-ttu-id="8bacd-138">示例</span><span class="sxs-lookup"><span data-stu-id="8bacd-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8bacd-139">请求</span><span class="sxs-lookup"><span data-stu-id="8bacd-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8bacd-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bacd-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printjob_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs
Content-Type: application/json
Content-length: 376

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
# <a name="c"></a>[<span data-ttu-id="8bacd-141">C#</span><span class="sxs-lookup"><span data-stu-id="8bacd-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printjob-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bacd-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bacd-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printjob-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bacd-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bacd-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printjob-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bacd-144">Java</span><span class="sxs-lookup"><span data-stu-id="8bacd-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printjob-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8bacd-145">响应</span><span class="sxs-lookup"><span data-stu-id="8bacd-145">Response</span></span>
<span data-ttu-id="8bacd-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8bacd-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printJobs/$entity",
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

