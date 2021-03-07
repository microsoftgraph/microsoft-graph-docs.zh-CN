---
title: 创建 printTaskTrigger
description: 在指定的打印机上创建新的任务触发器。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e02a2b0ce73d11153a0f778f9b0eeb80d505421b
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517325"
---
# <a name="create-printtasktrigger"></a><span data-ttu-id="6577b-103">创建 printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="6577b-103">Create printTaskTrigger</span></span>
<span data-ttu-id="6577b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6577b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="6577b-105">在指定的 [打印机上创建新的](../resources/printtasktrigger.md) 任务 [触发器](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="6577b-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="6577b-106">目前， **每个打印机** 只能指定一个任务触发器，但以后可能会删除此限制。</span><span class="sxs-lookup"><span data-stu-id="6577b-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6577b-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="6577b-107">Permissions</span></span>
<span data-ttu-id="6577b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6577b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6577b-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="6577b-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="6577b-111">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="6577b-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="6577b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6577b-112">Permission type</span></span> | <span data-ttu-id="6577b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6577b-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="6577b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6577b-114">Delegated (work or school account)</span></span>| <span data-ttu-id="6577b-115">Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6577b-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="6577b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6577b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6577b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6577b-117">Not Supported.</span></span>|
|<span data-ttu-id="6577b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6577b-118">Application</span></span>|<span data-ttu-id="6577b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6577b-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6577b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6577b-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="6577b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6577b-121">Request headers</span></span>
|<span data-ttu-id="6577b-122">名称</span><span class="sxs-lookup"><span data-stu-id="6577b-122">Name</span></span>|<span data-ttu-id="6577b-123">说明</span><span class="sxs-lookup"><span data-stu-id="6577b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6577b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6577b-124">Authorization</span></span>|<span data-ttu-id="6577b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6577b-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6577b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6577b-127">Content-Type</span></span>|<span data-ttu-id="6577b-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6577b-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6577b-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6577b-130">Request body</span></span>
<span data-ttu-id="6577b-131">在请求正文中，提供 [printTaskTrigger](../resources/printtasktrigger.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6577b-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="6577b-132">使用格式提供对 [printTaskDefinition](../resources/printtaskdefinition.md) 的引用， `@odata.bind` 如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="6577b-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="6577b-133">响应</span><span class="sxs-lookup"><span data-stu-id="6577b-133">Response</span></span>
<span data-ttu-id="6577b-134">如果成功，此方法在响应正文中返回响应代码 `201 Created` 和[printTaskTrigger。](../resources/printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="6577b-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6577b-135">示例</span><span class="sxs-lookup"><span data-stu-id="6577b-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6577b-136">请求</span><span class="sxs-lookup"><span data-stu-id="6577b-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_printtasktrigger_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/{printerId}/taskTriggers
Content-Type: application/json
Content-length: 80

{
  "event": "jobStarted",
  "definition@odata.bind": "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"
}
```


### <a name="response"></a><span data-ttu-id="6577b-137">响应</span><span class="sxs-lookup"><span data-stu-id="6577b-137">Response</span></span>
<span data-ttu-id="6577b-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6577b-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.print.microsoft.com/v1.0/$metadata#Collection(Microsoft.Graph.PrintTaskTrigger)",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```

