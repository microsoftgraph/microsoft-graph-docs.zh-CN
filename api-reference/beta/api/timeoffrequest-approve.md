---
title: timeOffRequest：批准
description: 批准 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0c78dbe8da36c03e53431db217ea8f186f8180cb
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981369"
---
# <a name="timeoffrequest-approve"></a><span data-ttu-id="f98ee-103">timeOffRequest：批准</span><span class="sxs-lookup"><span data-stu-id="f98ee-103">timeOffRequest: approve</span></span>

<span data-ttu-id="f98ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f98ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f98ee-105">批准 [timeoffrequest](../resources/timeoffrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="f98ee-105">Approve a [timeoffrequest](../resources/timeoffrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f98ee-106">权限</span><span class="sxs-lookup"><span data-stu-id="f98ee-106">Permissions</span></span>

<span data-ttu-id="f98ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f98ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f98ee-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f98ee-109">Permission type</span></span>                        | <span data-ttu-id="f98ee-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f98ee-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f98ee-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f98ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f98ee-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f98ee-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f98ee-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f98ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f98ee-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f98ee-114">Not supported.</span></span> |
|<span data-ttu-id="f98ee-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f98ee-115">Application</span></span> | <span data-ttu-id="f98ee-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="f98ee-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="f98ee-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="f98ee-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="f98ee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f98ee-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="f98ee-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f98ee-119">Request headers</span></span>

| <span data-ttu-id="f98ee-120">名称</span><span class="sxs-lookup"><span data-stu-id="f98ee-120">Name</span></span>          | <span data-ttu-id="f98ee-121">说明</span><span class="sxs-lookup"><span data-stu-id="f98ee-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f98ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f98ee-122">Authorization</span></span> | <span data-ttu-id="f98ee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f98ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f98ee-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="f98ee-125">Content-type</span></span> | <span data-ttu-id="f98ee-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f98ee-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f98ee-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f98ee-128">Request body</span></span>

<span data-ttu-id="f98ee-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f98ee-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f98ee-130">参数</span><span class="sxs-lookup"><span data-stu-id="f98ee-130">Parameter</span></span>    | <span data-ttu-id="f98ee-131">类型</span><span class="sxs-lookup"><span data-stu-id="f98ee-131">Type</span></span>        | <span data-ttu-id="f98ee-132">描述</span><span class="sxs-lookup"><span data-stu-id="f98ee-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f98ee-133">message</span><span class="sxs-lookup"><span data-stu-id="f98ee-133">message</span></span>|<span data-ttu-id="f98ee-134">String</span><span class="sxs-lookup"><span data-stu-id="f98ee-134">String</span></span>|<span data-ttu-id="f98ee-135">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="f98ee-135">Custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="f98ee-136">响应</span><span class="sxs-lookup"><span data-stu-id="f98ee-136">Response</span></span>

<span data-ttu-id="f98ee-p104">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f98ee-p104">If successful, this method returns a `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f98ee-139">示例</span><span class="sxs-lookup"><span data-stu-id="f98ee-139">Examples</span></span>

<span data-ttu-id="f98ee-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f98ee-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f98ee-141">请求</span><span class="sxs-lookup"><span data-stu-id="f98ee-141">Request</span></span>

<span data-ttu-id="f98ee-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f98ee-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f98ee-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f98ee-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="f98ee-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f98ee-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f98ee-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f98ee-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="f98ee-146">C#</span><span class="sxs-lookup"><span data-stu-id="f98ee-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f98ee-147">Java</span><span class="sxs-lookup"><span data-stu-id="f98ee-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f98ee-148">响应</span><span class="sxs-lookup"><span data-stu-id="f98ee-148">Response</span></span>

<span data-ttu-id="f98ee-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f98ee-149">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


