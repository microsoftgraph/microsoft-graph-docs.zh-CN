---
title: 创建 printTaskTrigger
description: 在指定的打印机上创建新的任务触发器。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3ed74256934310df5f5ea99217f8f0956e109eda
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771832"
---
# <a name="create-printtasktrigger"></a><span data-ttu-id="4af94-103">创建 printTaskTrigger</span><span class="sxs-lookup"><span data-stu-id="4af94-103">Create printTaskTrigger</span></span>
<span data-ttu-id="4af94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4af94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="4af94-105">在指定的 [打印机上创建新的](../resources/printtasktrigger.md) 任务 [触发器](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="4af94-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="4af94-106">目前， **每个打印机** 只能指定一个任务触发器，但以后可能会删除此限制。</span><span class="sxs-lookup"><span data-stu-id="4af94-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> 

## <a name="permissions"></a><span data-ttu-id="4af94-107">权限</span><span class="sxs-lookup"><span data-stu-id="4af94-107">Permissions</span></span>
<span data-ttu-id="4af94-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4af94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="4af94-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="4af94-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="4af94-111">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="4af94-111">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="4af94-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="4af94-112">Permission type</span></span> | <span data-ttu-id="4af94-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4af94-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="4af94-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4af94-114">Delegated (work or school account)</span></span>| <span data-ttu-id="4af94-115">Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="4af94-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="4af94-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4af94-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4af94-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4af94-117">Not Supported.</span></span>|
|<span data-ttu-id="4af94-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="4af94-118">Application</span></span>|<span data-ttu-id="4af94-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="4af94-119">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4af94-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4af94-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/{printerId}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="4af94-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4af94-121">Request headers</span></span>
|<span data-ttu-id="4af94-122">名称</span><span class="sxs-lookup"><span data-stu-id="4af94-122">Name</span></span>|<span data-ttu-id="4af94-123">说明</span><span class="sxs-lookup"><span data-stu-id="4af94-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4af94-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4af94-124">Authorization</span></span>|<span data-ttu-id="4af94-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4af94-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4af94-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4af94-127">Content-Type</span></span>|<span data-ttu-id="4af94-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4af94-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4af94-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="4af94-130">Request body</span></span>
<span data-ttu-id="4af94-131">在请求正文中，提供 [printTaskTrigger](../resources/printtasktrigger.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4af94-131">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="4af94-132">使用 格式提供 [对 printTaskDefinition](../resources/printtaskdefinition.md) 的引用 `@odata.bind` ，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="4af94-132">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="4af94-133">响应</span><span class="sxs-lookup"><span data-stu-id="4af94-133">Response</span></span>
<span data-ttu-id="4af94-134">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和[printTaskTrigger。](../resources/printtasktrigger.md)</span><span class="sxs-lookup"><span data-stu-id="4af94-134">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4af94-135">示例</span><span class="sxs-lookup"><span data-stu-id="4af94-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4af94-136">请求</span><span class="sxs-lookup"><span data-stu-id="4af94-136">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4af94-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4af94-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4af94-138">C#</span><span class="sxs-lookup"><span data-stu-id="4af94-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printtasktrigger-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4af94-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4af94-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printtasktrigger-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4af94-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4af94-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printtasktrigger-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4af94-141">Java</span><span class="sxs-lookup"><span data-stu-id="4af94-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printtasktrigger-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4af94-142">响应</span><span class="sxs-lookup"><span data-stu-id="4af94-142">Response</span></span>
<span data-ttu-id="4af94-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4af94-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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

