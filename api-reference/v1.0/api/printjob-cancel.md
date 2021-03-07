---
title: printJob： cancel
description: 取消打印作业。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8733a267f20c2f346ed7163d8d0af2a25725dece
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516982"
---
# <a name="printjob-cancel"></a><span data-ttu-id="97946-103">printJob： cancel</span><span class="sxs-lookup"><span data-stu-id="97946-103">printJob: cancel</span></span>
<span data-ttu-id="97946-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97946-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="97946-105">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="97946-105">Cancel a print job.</span></span> <span data-ttu-id="97946-106">打印作业只能代表用户使用委派权限取消。</span><span class="sxs-lookup"><span data-stu-id="97946-106">Print jobs can be canceled only on behalf of a user, using delegated permissions.</span></span>

## <a name="permissions"></a><span data-ttu-id="97946-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="97946-107">Permissions</span></span>
<span data-ttu-id="97946-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97946-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="97946-110">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [获取](printer-get.md) 打印机访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="97946-110">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [Get printer](printer-get.md) access.</span></span>

|<span data-ttu-id="97946-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="97946-111">Permission type</span></span> | <span data-ttu-id="97946-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97946-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="97946-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97946-113">Delegated (work or school account)</span></span>| <span data-ttu-id="97946-114">PrintJob.ReadWriteBasic、PrintJob.ReadWrite、PrintJob.ReadWriteBasic.All、PrintJob.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97946-114">PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All</span></span> |
|<span data-ttu-id="97946-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97946-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97946-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="97946-116">Not Supported.</span></span>|
|<span data-ttu-id="97946-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="97946-117">Application</span></span>| <span data-ttu-id="97946-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="97946-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97946-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97946-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/jobs/{printJobId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="97946-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="97946-120">Request headers</span></span>
|<span data-ttu-id="97946-121">名称</span><span class="sxs-lookup"><span data-stu-id="97946-121">Name</span></span>|<span data-ttu-id="97946-122">说明</span><span class="sxs-lookup"><span data-stu-id="97946-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="97946-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="97946-123">Authorization</span></span>|<span data-ttu-id="97946-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97946-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97946-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="97946-126">Request body</span></span>
<span data-ttu-id="97946-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97946-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97946-128">响应</span><span class="sxs-lookup"><span data-stu-id="97946-128">Response</span></span>
<span data-ttu-id="97946-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="97946-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97946-131">示例</span><span class="sxs-lookup"><span data-stu-id="97946-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97946-132">请求</span><span class="sxs-lookup"><span data-stu-id="97946-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "printjob_cancel"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/jobs/{printJobId}/cancel
```

### <a name="response"></a><span data-ttu-id="97946-133">响应</span><span class="sxs-lookup"><span data-stu-id="97946-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

