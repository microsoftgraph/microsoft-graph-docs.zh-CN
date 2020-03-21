---
title: 'printJob: startPrintJob'
description: 将打印作业提交到关联打印机。 任何现有的挂起作业完成、终止或取消后都将打印。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a5c558be384fcecad72e08e9d8aa45b0b397da06
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895670"
---
# <a name="printjob-startprintjob"></a><span data-ttu-id="38117-104">printJob: startPrintJob</span><span class="sxs-lookup"><span data-stu-id="38117-104">printJob: startPrintJob</span></span>

<span data-ttu-id="38117-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38117-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38117-106">将打印作业提交到关联[打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="38117-106">Submits the print job to the associated [printer](../resources/printer.md).</span></span> <span data-ttu-id="38117-107">它将在任何现有的挂起**作业**完成、终止或取消后进行打印。</span><span class="sxs-lookup"><span data-stu-id="38117-107">It will be printed after any existing pending **jobs** are completed, aborted, or canceled.</span></span>

## <a name="permissions"></a><span data-ttu-id="38117-108">权限</span><span class="sxs-lookup"><span data-stu-id="38117-108">Permissions</span></span>
<span data-ttu-id="38117-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38117-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="38117-111">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="38117-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="38117-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="38117-112">Permission type</span></span> | <span data-ttu-id="38117-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38117-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="38117-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38117-114">Delegated (work or school account)</span></span>| <span data-ttu-id="38117-115">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="38117-115">Users.Read.All</span></span> |
|<span data-ttu-id="38117-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38117-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38117-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="38117-117">Not Supported.</span></span>|
|<span data-ttu-id="38117-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="38117-118">Application</span></span>|<span data-ttu-id="38117-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="38117-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38117-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38117-120">HTTP request</span></span>
```http
POST /print/printers/{id}/jobs/{id}/startPrintJob
```
## <a name="request-headers"></a><span data-ttu-id="38117-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="38117-121">Request headers</span></span>
| <span data-ttu-id="38117-122">名称</span><span class="sxs-lookup"><span data-stu-id="38117-122">Name</span></span>          | <span data-ttu-id="38117-123">说明</span><span class="sxs-lookup"><span data-stu-id="38117-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="38117-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="38117-124">Authorization</span></span> | <span data-ttu-id="38117-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38117-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38117-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38117-127">Request body</span></span>

<span data-ttu-id="38117-128">请勿提交此 metho 的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38117-128">Do not submit a request body for this metho.</span></span> 

## <a name="response"></a><span data-ttu-id="38117-129">响应</span><span class="sxs-lookup"><span data-stu-id="38117-129">Response</span></span>
<span data-ttu-id="38117-130">如果成功，此方法在正文`200 OK`中返回响应代码和[printJobStatus](../resources/printjobstatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38117-130">If successful, this method returns a `200 OK` response code and a [printJobStatus](../resources/printjobstatus.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="38117-131">示例</span><span class="sxs-lookup"><span data-stu-id="38117-131">Example</span></span>
<span data-ttu-id="38117-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="38117-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38117-133">请求</span><span class="sxs-lookup"><span data-stu-id="38117-133">Request</span></span>

```http
POST https://graph.microsoft.com/beta/print/printers/{id}/jobs/{id}/startPrintJob
```

##### <a name="response"></a><span data-ttu-id="38117-134">响应</span><span class="sxs-lookup"><span data-stu-id="38117-134">Response</span></span>
<span data-ttu-id="38117-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="38117-135">The following is an example of the response.</span></span> 
><span data-ttu-id="38117-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="38117-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK

{
    "processingState": "processing",
    "processingStateDescription": "The print job is currently being processed.",
    "acquiredByPrinter": false
}
```
