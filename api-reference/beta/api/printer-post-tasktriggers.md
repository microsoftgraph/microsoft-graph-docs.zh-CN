---
title: Create taskTrigger
description: 在指定的打印机上创建新的任务触发器。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1b06d96f311301bb87d0b22e9a36e79aace6b9df
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979828"
---
# <a name="create-tasktrigger"></a><span data-ttu-id="ff5c0-103">Create taskTrigger</span><span class="sxs-lookup"><span data-stu-id="ff5c0-103">Create taskTrigger</span></span>

<span data-ttu-id="ff5c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff5c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff5c0-105">在指定的[打印机](../resources/printer.md)上创建新的[任务触发器](../resources/printtasktrigger.md)。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-105">Create a new [task trigger](../resources/printtasktrigger.md) on the specified [printer](../resources/printer.md).</span></span> <span data-ttu-id="ff5c0-106">目前，每台打印机只能指定 **一个** 任务触发器，但将来可以删除此限制。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-106">Currently, only **one** task trigger can be specified per printer, but this limit may be removed in the future.</span></span> <span data-ttu-id="ff5c0-107">此外，只有注册打印机的应用程序可以管理其任务触发器。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-107">Additionally, only the application that registered the printer can manage its task triggers.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff5c0-108">权限</span><span class="sxs-lookup"><span data-stu-id="ff5c0-108">Permissions</span></span>
<span data-ttu-id="ff5c0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ff5c0-111">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="ff5c0-112">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ff5c0-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff5c0-113">Permission type</span></span> | <span data-ttu-id="ff5c0-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff5c0-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ff5c0-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff5c0-115">Delegated (work or school account)</span></span>| <span data-ttu-id="ff5c0-116">完全控制和所有打印机。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-116">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="ff5c0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff5c0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff5c0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-118">Not Supported.</span></span>|
|<span data-ttu-id="ff5c0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff5c0-119">Application</span></span>|<span data-ttu-id="ff5c0-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-120">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff5c0-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff5c0-121">HTTP request</span></span>

```http
POST /print/printers/{id}/taskTriggers
```

## <a name="request-headers"></a><span data-ttu-id="ff5c0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff5c0-122">Request headers</span></span>
| <span data-ttu-id="ff5c0-123">名称</span><span class="sxs-lookup"><span data-stu-id="ff5c0-123">Name</span></span>      |<span data-ttu-id="ff5c0-124">说明</span><span class="sxs-lookup"><span data-stu-id="ff5c0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff5c0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff5c0-125">Authorization</span></span> | <span data-ttu-id="ff5c0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff5c0-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="ff5c0-128">Content-type</span></span>  | <span data-ttu-id="ff5c0-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ff5c0-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff5c0-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff5c0-131">Request body</span></span>
<span data-ttu-id="ff5c0-132">在请求正文中，提供 [printTaskTrigger](../resources/printtasktrigger.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-132">In the request body, supply a JSON representation of a [printTaskTrigger](../resources/printtasktrigger.md) object.</span></span> <span data-ttu-id="ff5c0-133">使用格式提供对 [printTaskDefinition](../resources/printtaskdefinition.md) 的引用 `@odata.bind` ，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-133">Supply a reference to a [printTaskDefinition](../resources/printtaskdefinition.md) by using the `@odata.bind` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="ff5c0-134">响应</span><span class="sxs-lookup"><span data-stu-id="ff5c0-134">Response</span></span>
<span data-ttu-id="ff5c0-135">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [printTaskTrigger](../resources/printtasktrigger.md) 。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-135">If successful, this method returns a `201 Created` response code and a [printTaskTrigger](../resources/printtasktrigger.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff5c0-136">示例</span><span class="sxs-lookup"><span data-stu-id="ff5c0-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff5c0-137">请求</span><span class="sxs-lookup"><span data-stu-id="ff5c0-137">Request</span></span>
<span data-ttu-id="ff5c0-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ff5c0-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff5c0-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer_tasktrigger"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/ae63f617-4856-4b45-8ea9-69dfbeea230e/taskTriggers

{
  "event": "jobStarted",
  "definition@odata.bind": "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"
}
```
# <a name="c"></a>[<span data-ttu-id="ff5c0-140">C#</span><span class="sxs-lookup"><span data-stu-id="ff5c0-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-tasktrigger-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff5c0-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff5c0-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-tasktrigger-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff5c0-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff5c0-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-tasktrigger-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ff5c0-143">Java</span><span class="sxs-lookup"><span data-stu-id="ff5c0-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printer-tasktrigger-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="ff5c0-144">响应</span><span class="sxs-lookup"><span data-stu-id="ff5c0-144">Response</span></span>
<span data-ttu-id="ff5c0-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-145">The following is an example of the response.</span></span>
><span data-ttu-id="ff5c0-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ff5c0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskTrigger"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 196

{
  "@odata.context": "https://graph.print.microsoft.com/v1.0/$metadata#Collection(Microsoft.Graph.PrintTaskTrigger)",
  "id": "b6a843ca-e60e-4e20-a222-a58d85eead6d",
  "event": "jobStarted"
}
```
