---
title: List taskTriggers
description: 检索与打印机关联的任务触发器列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: b4f76f356120a27eb52dfd013b65cb7cd38ef43a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516965"
---
# <a name="list-tasktriggers"></a><span data-ttu-id="84cde-103">List taskTriggers</span><span class="sxs-lookup"><span data-stu-id="84cde-103">List taskTriggers</span></span>
<span data-ttu-id="84cde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84cde-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="84cde-105">检索与 [打印机](../resources/printtasktrigger.md) 相关联的任务触发器 [的列表](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="84cde-105">Retrieve a list of [task triggers](../resources/printtasktrigger.md) associated with the [printer](../resources/printer.md).</span></span> <span data-ttu-id="84cde-106">任务触发器列表定义打印期间发生的事件将触发的任务。</span><span class="sxs-lookup"><span data-stu-id="84cde-106">The list of task triggers defines which tasks will be triggered as a result of events that occur during printing.</span></span>

<span data-ttu-id="84cde-107">有关如何使用此 API 向通用打印添加拉页打印支持的详细信息，请参阅 [扩展通用打印以支持拉取打印](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing)。</span><span class="sxs-lookup"><span data-stu-id="84cde-107">For details about how to use this API to add pull printing support to Universal Print, see [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).</span></span>

## <a name="permissions"></a><span data-ttu-id="84cde-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="84cde-108">Permissions</span></span>
<span data-ttu-id="84cde-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84cde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="84cde-111">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="84cde-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="84cde-112">登录用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="84cde-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="84cde-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="84cde-113">Permission type</span></span> | <span data-ttu-id="84cde-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84cde-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="84cde-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84cde-115">Delegated (work or school account)</span></span>| <span data-ttu-id="84cde-116">Printer.Read.All、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="84cde-116">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="84cde-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84cde-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84cde-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="84cde-118">Not Supported.</span></span>|
|<span data-ttu-id="84cde-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="84cde-119">Application</span></span>| <span data-ttu-id="84cde-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="84cde-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="84cde-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84cde-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/taskTriggers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84cde-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="84cde-122">Optional query parameters</span></span>
<span data-ttu-id="84cde-123">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="84cde-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="84cde-124">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="84cde-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="84cde-125">Exceptions</span><span class="sxs-lookup"><span data-stu-id="84cde-125">Exceptions</span></span>
<span data-ttu-id="84cde-126">不支持某些运算符： `$count` ， `$format` ， ， ， `$search` `$select` `$skip` `$top` 。</span><span class="sxs-lookup"><span data-stu-id="84cde-126">Some operators are not supported: `$count`, `$format`, `$search`, `$select`, `$skip`, `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84cde-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="84cde-127">Request headers</span></span>
|<span data-ttu-id="84cde-128">名称</span><span class="sxs-lookup"><span data-stu-id="84cde-128">Name</span></span>|<span data-ttu-id="84cde-129">说明</span><span class="sxs-lookup"><span data-stu-id="84cde-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="84cde-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="84cde-130">Authorization</span></span>|<span data-ttu-id="84cde-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="84cde-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="84cde-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="84cde-133">Request body</span></span>
<span data-ttu-id="84cde-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84cde-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84cde-135">响应</span><span class="sxs-lookup"><span data-stu-id="84cde-135">Response</span></span>

<span data-ttu-id="84cde-136">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [printTaskTrigger](../resources/printtasktrigger.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="84cde-136">If successful, this method returns a `200 OK` response code and a collection of [printTaskTrigger](../resources/printtasktrigger.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84cde-137">示例</span><span class="sxs-lookup"><span data-stu-id="84cde-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84cde-138">请求</span><span class="sxs-lookup"><span data-stu-id="84cde-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printtasktrigger"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers
```


### <a name="response"></a><span data-ttu-id="84cde-139">响应</span><span class="sxs-lookup"><span data-stu-id="84cde-139">Response</span></span>
<span data-ttu-id="84cde-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="84cde-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printTaskTrigger)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('fcc7fe6a-5ba7-4059-8017-702f3a41c8a4')/taskTriggers",
  "value": [
    {
      "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
      "event": "jobStarted"
    }
  ]
}
```

