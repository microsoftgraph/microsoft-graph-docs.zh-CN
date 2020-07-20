---
title: 删除 taskTrigger
description: 删除打印机的任务触发器。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c96edf3379e1d20e35070e4e131ffb08cce98d5f
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091584"
---
# <a name="delete-tasktrigger"></a><span data-ttu-id="ca5cb-103">删除 taskTrigger</span><span class="sxs-lookup"><span data-stu-id="ca5cb-103">Delete taskTrigger</span></span>

<span data-ttu-id="ca5cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca5cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca5cb-105">删除[打印机](../resources/printer.md)的[任务触发器](../resources/printtasktrigger.md)，以防止在指定打印机上触发任务的相关打印事件。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-105">Delete a [printer](../resources/printer.md)'s [task trigger](../resources/printtasktrigger.md) to prevent related print events from triggering tasks on the specified printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca5cb-106">权限</span><span class="sxs-lookup"><span data-stu-id="ca5cb-106">Permissions</span></span>
<span data-ttu-id="ca5cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ca5cb-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="ca5cb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca5cb-110">Permission type</span></span> | <span data-ttu-id="ca5cb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca5cb-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ca5cb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca5cb-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ca5cb-113">完全控制和所有打印机。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-113">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="ca5cb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca5cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca5cb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-115">Not Supported.</span></span>|
|<span data-ttu-id="ca5cb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca5cb-116">Application</span></span>|<span data-ttu-id="ca5cb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca5cb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca5cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printers/{id}/taskTriggers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ca5cb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca5cb-119">Request headers</span></span>
| <span data-ttu-id="ca5cb-120">名称</span><span class="sxs-lookup"><span data-stu-id="ca5cb-120">Name</span></span>          | <span data-ttu-id="ca5cb-121">说明</span><span class="sxs-lookup"><span data-stu-id="ca5cb-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ca5cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca5cb-122">Authorization</span></span> | <span data-ttu-id="ca5cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca5cb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca5cb-125">Request body</span></span>
<span data-ttu-id="ca5cb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca5cb-127">响应</span><span class="sxs-lookup"><span data-stu-id="ca5cb-127">Response</span></span>
<span data-ttu-id="ca5cb-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca5cb-130">示例</span><span class="sxs-lookup"><span data-stu-id="ca5cb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca5cb-131">请求</span><span class="sxs-lookup"><span data-stu-id="ca5cb-131">Request</span></span>
<span data-ttu-id="ca5cb-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_printer_tasktrigger"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec
```

---

##### <a name="response"></a><span data-ttu-id="ca5cb-133">响应</span><span class="sxs-lookup"><span data-stu-id="ca5cb-133">Response</span></span>
<span data-ttu-id="ca5cb-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-134">The following is an example of the response.</span></span>
><span data-ttu-id="ca5cb-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ca5cb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete taskTrigger",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
