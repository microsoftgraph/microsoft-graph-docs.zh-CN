---
title: 为 printerShare 创建 printJob
description: 为 printerShare 创建新的 printJob。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 9dafcee89de7352c2887ffd13788d5f1bcda202f
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517192"
---
# <a name="create-printjob-for-a-printershare"></a><span data-ttu-id="29adc-103">为 printerShare 创建 printJob</span><span class="sxs-lookup"><span data-stu-id="29adc-103">Create printJob for a printerShare</span></span>
<span data-ttu-id="29adc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29adc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="29adc-105">为 printerShare 创建新的[printJob。](../resources/printJob.md) [](../resources/printerShare.md)</span><span class="sxs-lookup"><span data-stu-id="29adc-105">Create a new [printJob](../resources/printJob.md) for a [printerShare](../resources/printerShare.md).</span></span> 

<span data-ttu-id="29adc-106">此外，创建与 printJob 关联的新[printDocument。](../resources/printDocument.md)</span><span class="sxs-lookup"><span data-stu-id="29adc-106">Also creates a new [printDocument](../resources/printDocument.md) associated with the printJob.</span></span>

## <a name="permissions"></a><span data-ttu-id="29adc-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="29adc-107">Permissions</span></span>
<span data-ttu-id="29adc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29adc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="29adc-110">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [获取 printerShare](printerShare-get.md) 访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="29adc-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printerShare](printerShare-get.md) access.</span></span> <span data-ttu-id="29adc-111">登录用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="29adc-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="29adc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="29adc-112">Permission type</span></span> | <span data-ttu-id="29adc-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29adc-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="29adc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29adc-114">Delegated (work or school account)</span></span>| <span data-ttu-id="29adc-115">PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29adc-115">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="29adc-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29adc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29adc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="29adc-117">Not Supported.</span></span>|
|<span data-ttu-id="29adc-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="29adc-118">Application</span></span>| <span data-ttu-id="29adc-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="29adc-119">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="29adc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29adc-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs
```

## <a name="request-headers"></a><span data-ttu-id="29adc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="29adc-121">Request headers</span></span>
|<span data-ttu-id="29adc-122">名称</span><span class="sxs-lookup"><span data-stu-id="29adc-122">Name</span></span>|<span data-ttu-id="29adc-123">说明</span><span class="sxs-lookup"><span data-stu-id="29adc-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="29adc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="29adc-124">Authorization</span></span>|<span data-ttu-id="29adc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29adc-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="29adc-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29adc-127">Content-Type</span></span>|<span data-ttu-id="29adc-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="29adc-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29adc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="29adc-130">Request body</span></span>
<span data-ttu-id="29adc-131">在请求正文中，提供 [printJob](../resources/printjob.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29adc-131">In the request body, supply a JSON representation of a [printJob](../resources/printjob.md) object.</span></span> <span data-ttu-id="29adc-132">printJob 对象应仅包含 **配置** 属性。</span><span class="sxs-lookup"><span data-stu-id="29adc-132">The printJob object should only contain **configuration** property.</span></span> <span data-ttu-id="29adc-133">配置的所有 **属性都** 为 null。</span><span class="sxs-lookup"><span data-stu-id="29adc-133">All properties of **configuration** are nullable.</span></span> <span data-ttu-id="29adc-134">所有其他字段（包括作业和文档 ID）将在资源创建过程中自动设置，不应在请求中提供。</span><span class="sxs-lookup"><span data-stu-id="29adc-134">All other fields, including job and document IDs, are set automatically during resource creation and should not be provided in request.</span></span>

<span data-ttu-id="29adc-135">目前，通用打印仅支持每个 **printJob** 对象一个 **printDocument。**</span><span class="sxs-lookup"><span data-stu-id="29adc-135">Right now, Universal Print supports only one **printDocument** per **printJob** object.</span></span>

## <a name="response"></a><span data-ttu-id="29adc-136">响应</span><span class="sxs-lookup"><span data-stu-id="29adc-136">Response</span></span>

<span data-ttu-id="29adc-137">如果成功，此方法在响应正文中返回响应 `201 Created` 代码[、printJob](../resources/printjob.md)对象和关联的[printDocument。](../resources/printDocument.md)</span><span class="sxs-lookup"><span data-stu-id="29adc-137">If successful, this method returns a `201 Created` response code and a [printJob](../resources/printjob.md) object and associated [printDocument](../resources/printDocument.md) in the response body.</span></span> 

## <a name="examples"></a><span data-ttu-id="29adc-138">示例</span><span class="sxs-lookup"><span data-stu-id="29adc-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29adc-139">请求</span><span class="sxs-lookup"><span data-stu-id="29adc-139">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="29adc-140">响应</span><span class="sxs-lookup"><span data-stu-id="29adc-140">Response</span></span>
<span data-ttu-id="29adc-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="29adc-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

