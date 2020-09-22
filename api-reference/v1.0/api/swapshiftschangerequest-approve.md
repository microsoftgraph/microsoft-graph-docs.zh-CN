---
title: swapShiftsChangeRequest：批准
description: 批准交换转换请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 83da14797ddbb6747cf6074390dabf8a8968e419
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037939"
---
# <a name="swapshiftschangerequest-approve"></a><span data-ttu-id="9c71c-103">swapShiftsChangeRequest：批准</span><span class="sxs-lookup"><span data-stu-id="9c71c-103">swapShiftsChangeRequest: approve</span></span>

<span data-ttu-id="9c71c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c71c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c71c-105">批准 [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9c71c-105">Approve a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c71c-106">权限</span><span class="sxs-lookup"><span data-stu-id="9c71c-106">Permissions</span></span>

<span data-ttu-id="9c71c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c71c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9c71c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c71c-109">Permission type</span></span>                        | <span data-ttu-id="9c71c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c71c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="9c71c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c71c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9c71c-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="9c71c-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c71c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c71c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c71c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c71c-114">Not supported.</span></span>    |
|<span data-ttu-id="9c71c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c71c-115">Application</span></span> | <span data-ttu-id="9c71c-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c71c-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="9c71c-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="9c71c-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9c71c-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="9c71c-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="9c71c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c71c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="9c71c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c71c-120">Request headers</span></span>

| <span data-ttu-id="9c71c-121">名称</span><span class="sxs-lookup"><span data-stu-id="9c71c-121">Name</span></span>          | <span data-ttu-id="9c71c-122">说明</span><span class="sxs-lookup"><span data-stu-id="9c71c-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9c71c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c71c-123">Authorization</span></span> | <span data-ttu-id="9c71c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c71c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9c71c-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="9c71c-126">Content-type</span></span> | <span data-ttu-id="9c71c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9c71c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c71c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c71c-129">Request body</span></span>

<span data-ttu-id="9c71c-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="9c71c-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9c71c-131">参数</span><span class="sxs-lookup"><span data-stu-id="9c71c-131">Parameter</span></span>    | <span data-ttu-id="9c71c-132">类型</span><span class="sxs-lookup"><span data-stu-id="9c71c-132">Type</span></span>        | <span data-ttu-id="9c71c-133">描述</span><span class="sxs-lookup"><span data-stu-id="9c71c-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9c71c-134">message</span><span class="sxs-lookup"><span data-stu-id="9c71c-134">message</span></span>|<span data-ttu-id="9c71c-135">String</span><span class="sxs-lookup"><span data-stu-id="9c71c-135">String</span></span>|<span data-ttu-id="9c71c-136">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="9c71c-136">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="9c71c-137">响应</span><span class="sxs-lookup"><span data-stu-id="9c71c-137">Response</span></span>

<span data-ttu-id="9c71c-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9c71c-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9c71c-140">示例</span><span class="sxs-lookup"><span data-stu-id="9c71c-140">Examples</span></span>

<span data-ttu-id="9c71c-141">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9c71c-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="9c71c-142">请求</span><span class="sxs-lookup"><span data-stu-id="9c71c-142">Request</span></span>

<span data-ttu-id="9c71c-143">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="9c71c-143">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9c71c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c71c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="9c71c-145">C#</span><span class="sxs-lookup"><span data-stu-id="9c71c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c71c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c71c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c71c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c71c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c71c-148">Java</span><span class="sxs-lookup"><span data-stu-id="9c71c-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="9c71c-149">响应</span><span class="sxs-lookup"><span data-stu-id="9c71c-149">Response</span></span>

<span data-ttu-id="9c71c-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9c71c-150">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

