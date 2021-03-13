---
title: 更新 printJob
description: 更新打印作业
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 885190ea6a23ed6c5408f7476f5a4f10463ae012
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768759"
---
# <a name="update-printjob"></a><span data-ttu-id="10ba1-103">更新 printJob</span><span class="sxs-lookup"><span data-stu-id="10ba1-103">Update printJob</span></span>
<span data-ttu-id="10ba1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10ba1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="10ba1-105">更新 [打印作业](../resources/printjob.md)。</span><span class="sxs-lookup"><span data-stu-id="10ba1-105">Update a [print job](../resources/printjob.md).</span></span> <span data-ttu-id="10ba1-106">只能 **更新 configuration** 属性。</span><span class="sxs-lookup"><span data-stu-id="10ba1-106">Only the **configuration** property can be updated.</span></span>

<span data-ttu-id="10ba1-107">只有在关联的打印作业上存在由请求应用创建的触发器启动的 [printTask](../resources/printTask.md) 状态时，更新打印作业才能 `processing` 成功。</span><span class="sxs-lookup"><span data-stu-id="10ba1-107">Updating a print job will only succeed if there is a [printTask](../resources/printTask.md) in a `processing` state on the associated print job, started by a trigger that the requesting app created.</span></span> <span data-ttu-id="10ba1-108">若要详细了解如何注册任务触发器，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="10ba1-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="10ba1-109">权限</span><span class="sxs-lookup"><span data-stu-id="10ba1-109">Permissions</span></span>
<span data-ttu-id="10ba1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="10ba1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="10ba1-112">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅（Printer.Read.All 或 Printer.ReadWrite.All 应用程序权限）以及下表中列出的权限之一。</span><span class="sxs-lookup"><span data-stu-id="10ba1-112">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="10ba1-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="10ba1-113">Permission type</span></span> | <span data-ttu-id="10ba1-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="10ba1-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="10ba1-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10ba1-115">Delegated (work or school account)</span></span>| <span data-ttu-id="10ba1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10ba1-116">Not supported.</span></span> |
|<span data-ttu-id="10ba1-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10ba1-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10ba1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="10ba1-118">Not Supported.</span></span>|
|<span data-ttu-id="10ba1-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="10ba1-119">Application</span></span>| <span data-ttu-id="10ba1-120">PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All、PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="10ba1-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10ba1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10ba1-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}/jobs/{printJobId}
```

## <a name="request-headers"></a><span data-ttu-id="10ba1-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="10ba1-122">Request headers</span></span>
|<span data-ttu-id="10ba1-123">名称</span><span class="sxs-lookup"><span data-stu-id="10ba1-123">Name</span></span>|<span data-ttu-id="10ba1-124">说明</span><span class="sxs-lookup"><span data-stu-id="10ba1-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="10ba1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="10ba1-125">Authorization</span></span>|<span data-ttu-id="10ba1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="10ba1-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="10ba1-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10ba1-128">Content-Type</span></span>|<span data-ttu-id="10ba1-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="10ba1-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10ba1-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="10ba1-131">Request body</span></span>
<span data-ttu-id="10ba1-132">在请求正文中，提供相关 [printJob 字段](../resources/printjob.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="10ba1-132">In the request body, supply the values of the relevant [printJob](../resources/printjob.md) fields.</span></span> <span data-ttu-id="10ba1-133">请求正文中未包含的现有属性将保留其以前的值。</span><span class="sxs-lookup"><span data-stu-id="10ba1-133">Existing properties that are not included in the request body will maintain their previous values.</span></span> 

<span data-ttu-id="10ba1-134">只能 **更新 configuration** 属性。</span><span class="sxs-lookup"><span data-stu-id="10ba1-134">Only the **configuration** property can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="10ba1-135">响应</span><span class="sxs-lookup"><span data-stu-id="10ba1-135">Response</span></span>

<span data-ttu-id="10ba1-136">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [printJob](../resources/printjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="10ba1-136">If successful, this method returns a `200 OK` response code with an updated [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10ba1-137">示例</span><span class="sxs-lookup"><span data-stu-id="10ba1-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10ba1-138">请求</span><span class="sxs-lookup"><span data-stu-id="10ba1-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="10ba1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="10ba1-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="10ba1-140">C#</span><span class="sxs-lookup"><span data-stu-id="10ba1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printjob-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10ba1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10ba1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printjob-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10ba1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10ba1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printjob-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10ba1-143">Java</span><span class="sxs-lookup"><span data-stu-id="10ba1-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printjob-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="10ba1-144">响应</span><span class="sxs-lookup"><span data-stu-id="10ba1-144">Response</span></span>
<span data-ttu-id="10ba1-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="10ba1-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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

