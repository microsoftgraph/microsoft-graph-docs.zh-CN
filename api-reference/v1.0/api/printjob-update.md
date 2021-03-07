---
title: 更新 printJob
description: 更新打印作业
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3fd3109f914e08d0dd152b2e22ce5f20a84b2d96
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517164"
---
# <a name="update-printjob"></a><span data-ttu-id="cd062-103">更新 printJob</span><span class="sxs-lookup"><span data-stu-id="cd062-103">Update printJob</span></span>
<span data-ttu-id="cd062-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd062-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="cd062-105">更新 [打印作业](../resources/printjob.md)。</span><span class="sxs-lookup"><span data-stu-id="cd062-105">Update a [print job](../resources/printjob.md).</span></span> <span data-ttu-id="cd062-106">只能 **更新配置** 属性。</span><span class="sxs-lookup"><span data-stu-id="cd062-106">Only the **configuration** property can be updated.</span></span>

<span data-ttu-id="cd062-107">只有在关联的打印作业上存在由请求应用创建的触发器启动的 [printTask](../resources/printTask.md) 时，更新打印作业才能 `processing` 成功。</span><span class="sxs-lookup"><span data-stu-id="cd062-107">Updating a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="cd062-108">若要详细了解如何注册任务触发器，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="cd062-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="cd062-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="cd062-109">Permissions</span></span>
<span data-ttu-id="cd062-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd062-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cd062-112">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅（Printer.Read.All 或 Printer.ReadWrite.All 应用程序权限）以及下表中列出的权限之一。</span><span class="sxs-lookup"><span data-stu-id="cd062-112">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="cd062-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd062-113">Permission type</span></span> | <span data-ttu-id="cd062-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd062-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="cd062-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd062-115">Delegated (work or school account)</span></span>| <span data-ttu-id="cd062-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd062-116">Not supported.</span></span> |
|<span data-ttu-id="cd062-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd062-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd062-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd062-118">Not Supported.</span></span>|
|<span data-ttu-id="cd062-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd062-119">Application</span></span>| <span data-ttu-id="cd062-120">PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All、PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="cd062-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd062-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd062-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}/jobs/{printJobId}
```

## <a name="request-headers"></a><span data-ttu-id="cd062-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd062-122">Request headers</span></span>
|<span data-ttu-id="cd062-123">名称</span><span class="sxs-lookup"><span data-stu-id="cd062-123">Name</span></span>|<span data-ttu-id="cd062-124">说明</span><span class="sxs-lookup"><span data-stu-id="cd062-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cd062-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd062-125">Authorization</span></span>|<span data-ttu-id="cd062-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd062-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cd062-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd062-128">Content-Type</span></span>|<span data-ttu-id="cd062-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cd062-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd062-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd062-131">Request body</span></span>
<span data-ttu-id="cd062-132">在请求正文中，提供相关 [printJob 字段](../resources/printjob.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="cd062-132">In the request body, supply the values of the relevant [printJob](../resources/printjob.md) fields.</span></span> <span data-ttu-id="cd062-133">请求正文中不包含的现有属性将保留其以前的值。</span><span class="sxs-lookup"><span data-stu-id="cd062-133">Existing properties that are not included in the request body will maintain their previous values.</span></span> 

<span data-ttu-id="cd062-134">只能 **更新配置** 属性。</span><span class="sxs-lookup"><span data-stu-id="cd062-134">Only the **configuration** property can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="cd062-135">响应</span><span class="sxs-lookup"><span data-stu-id="cd062-135">Response</span></span>

<span data-ttu-id="cd062-136">如果成功，此方法在响应正文中返回具有更新 `200 OK` [的 printJob](../resources/printjob.md) 对象的响应代码。</span><span class="sxs-lookup"><span data-stu-id="cd062-136">If successful, this method returns a `200 OK` response code with an updated [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd062-137">示例</span><span class="sxs-lookup"><span data-stu-id="cd062-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cd062-138">请求</span><span class="sxs-lookup"><span data-stu-id="cd062-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printjob"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}
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

### <a name="response"></a><span data-ttu-id="cd062-139">响应</span><span class="sxs-lookup"><span data-stu-id="cd062-139">Response</span></span>
<span data-ttu-id="cd062-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cd062-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('d5ef6ec4-07ca-4212-baf9-d45be126bfbb')/jobs/$entity",
  "id": "44353",
  "createdDateTime": "2020-06-26T04:20:06.5715544Z",
  "createdBy": {
    "id": "",
    "displayName": "",
    "userPrincipalName": ""
  },
  "status": {
    "state": "paused",
    "description": "The job is not a candidate for processing yet."
  },
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

