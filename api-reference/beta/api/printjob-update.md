---
title: 更新 printJob
description: 更新打印作业的配置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 6405acd01be075c44c4271c4c3395a83889f9d0e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777683"
---
# <a name="update-printjob"></a><span data-ttu-id="bbc06-103">更新 printJob</span><span class="sxs-lookup"><span data-stu-id="bbc06-103">Update printJob</span></span>

<span data-ttu-id="bbc06-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbc06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbc06-105">更新 [打印作业](../resources/printjob.md)。</span><span class="sxs-lookup"><span data-stu-id="bbc06-105">Update a [print job](../resources/printjob.md).</span></span> <span data-ttu-id="bbc06-106">只能 **更新 configuration** 属性。</span><span class="sxs-lookup"><span data-stu-id="bbc06-106">Only the **configuration** property can be updated.</span></span>

<span data-ttu-id="bbc06-107">只有在状态为（由请求应用创建的触发器启动）的 [printTask](../resources/printTask.md) 与打印作业关联时，更新打印作业才能 `processing` 成功。</span><span class="sxs-lookup"><span data-stu-id="bbc06-107">Updating a print job will only succeed if a [printTask](../resources/printTask.md) in a `processing` state, started by a trigger that the requesting app created, is associated with the print job.</span></span> <span data-ttu-id="bbc06-108">若要详细了解如何注册任务触发器，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="bbc06-108">For details about how to register a task trigger, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="bbc06-109">权限</span><span class="sxs-lookup"><span data-stu-id="bbc06-109">Permissions</span></span>
<span data-ttu-id="bbc06-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bbc06-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bbc06-112">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅（Printer.Read.All 或 Printer.ReadWrite.All 应用程序权限）以及下表中列出的权限之一。</span><span class="sxs-lookup"><span data-stu-id="bbc06-112">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, either the Printer.Read.All or Printer.ReadWrite.All application permission, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="bbc06-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbc06-113">Permission type</span></span> | <span data-ttu-id="bbc06-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bbc06-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bbc06-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbc06-115">Delegated (work or school account)</span></span>| <span data-ttu-id="bbc06-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbc06-116">Not supported.</span></span> |
|<span data-ttu-id="bbc06-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbc06-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbc06-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbc06-118">Not Supported.</span></span>|
|<span data-ttu-id="bbc06-119">Application</span><span class="sxs-lookup"><span data-stu-id="bbc06-119">Application</span></span>| <span data-ttu-id="bbc06-120">PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All、PrintJob.Manage.All</span><span class="sxs-lookup"><span data-stu-id="bbc06-120">PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All, PrintJob.Manage.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbc06-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbc06-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}/jobs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bbc06-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbc06-122">Request headers</span></span>
| <span data-ttu-id="bbc06-123">名称</span><span class="sxs-lookup"><span data-stu-id="bbc06-123">Name</span></span>          | <span data-ttu-id="bbc06-124">说明</span><span class="sxs-lookup"><span data-stu-id="bbc06-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bbc06-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbc06-125">Authorization</span></span> | <span data-ttu-id="bbc06-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bbc06-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbc06-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbc06-128">Request body</span></span>
<span data-ttu-id="bbc06-129">在请求正文中，提供相关 [printJob 字段](../resources/printjob.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="bbc06-129">In the request body, supply the values of the relevant [printJob](../resources/printjob.md) fields.</span></span> <span data-ttu-id="bbc06-130">请求正文中未包含的现有属性将保留其以前的值。</span><span class="sxs-lookup"><span data-stu-id="bbc06-130">Existing properties that are not included in the request body will maintain their previous values.</span></span> <span data-ttu-id="bbc06-131">只能更新"configuration"属性。</span><span class="sxs-lookup"><span data-stu-id="bbc06-131">Only the "configuration" property can be updated.</span></span>

## <a name="response"></a><span data-ttu-id="bbc06-132">响应</span><span class="sxs-lookup"><span data-stu-id="bbc06-132">Response</span></span>
<span data-ttu-id="bbc06-133">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [printJob](../resources/printjob.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bbc06-133">If successful, this method returns a `200 OK` response code with an updated [printJob](../resources/printjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbc06-134">示例</span><span class="sxs-lookup"><span data-stu-id="bbc06-134">Example</span></span>
<span data-ttu-id="bbc06-135">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="bbc06-135">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="bbc06-136">请求</span><span class="sxs-lookup"><span data-stu-id="bbc06-136">Request</span></span>
<span data-ttu-id="bbc06-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bbc06-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bbc06-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbc06-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printjob-update"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353

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
# <a name="c"></a>[<span data-ttu-id="bbc06-139">C#</span><span class="sxs-lookup"><span data-stu-id="bbc06-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printjob-update-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbc06-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbc06-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printjob-update-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbc06-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbc06-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printjob-update-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bbc06-142">Java</span><span class="sxs-lookup"><span data-stu-id="bbc06-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printjob-update-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bbc06-143">响应</span><span class="sxs-lookup"><span data-stu-id="bbc06-143">Response</span></span>
<span data-ttu-id="bbc06-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bbc06-144">The following is an example of the response.</span></span> 
><span data-ttu-id="bbc06-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bbc06-145">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('d5ef6ec4-07ca-4212-baf9-d45be126bfbb')/jobs/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update print job",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


