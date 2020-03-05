---
title: timeOffRequest：批准
description: 批准 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1e161d21b25e474f3433e3c3b49ff5a739e87605
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452263"
---
# <a name="timeoffrequest-approve"></a><span data-ttu-id="dd845-103">timeOffRequest：批准</span><span class="sxs-lookup"><span data-stu-id="dd845-103">timeOffRequest: approve</span></span>

<span data-ttu-id="dd845-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dd845-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd845-105">批准[timeoffrequest](../resources/timeoffrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="dd845-105">Approve a [timeoffrequest](../resources/timeoffrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd845-106">权限</span><span class="sxs-lookup"><span data-stu-id="dd845-106">Permissions</span></span>

<span data-ttu-id="dd845-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd845-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd845-109">Permission type</span></span>                        | <span data-ttu-id="dd845-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd845-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd845-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd845-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd845-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd845-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="dd845-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd845-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd845-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd845-114">Not supported.</span></span> |
|<span data-ttu-id="dd845-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd845-115">Application</span></span> | <span data-ttu-id="dd845-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="dd845-116">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="dd845-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="dd845-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="dd845-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd845-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="dd845-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd845-119">Request headers</span></span>

| <span data-ttu-id="dd845-120">名称</span><span class="sxs-lookup"><span data-stu-id="dd845-120">Name</span></span>          | <span data-ttu-id="dd845-121">说明</span><span class="sxs-lookup"><span data-stu-id="dd845-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dd845-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd845-122">Authorization</span></span> | <span data-ttu-id="dd845-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd845-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd845-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="dd845-125">Content-type</span></span> | <span data-ttu-id="dd845-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="dd845-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd845-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd845-128">Request body</span></span>

<span data-ttu-id="dd845-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="dd845-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dd845-130">参数</span><span class="sxs-lookup"><span data-stu-id="dd845-130">Parameter</span></span>    | <span data-ttu-id="dd845-131">类型</span><span class="sxs-lookup"><span data-stu-id="dd845-131">Type</span></span>        | <span data-ttu-id="dd845-132">描述</span><span class="sxs-lookup"><span data-stu-id="dd845-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd845-133">message</span><span class="sxs-lookup"><span data-stu-id="dd845-133">message</span></span>|<span data-ttu-id="dd845-134">String</span><span class="sxs-lookup"><span data-stu-id="dd845-134">String</span></span>|<span data-ttu-id="dd845-135">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="dd845-135">Custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="dd845-136">响应</span><span class="sxs-lookup"><span data-stu-id="dd845-136">Response</span></span>

<span data-ttu-id="dd845-p104">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dd845-p104">If successful, this method returns a `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd845-139">示例</span><span class="sxs-lookup"><span data-stu-id="dd845-139">Examples</span></span>

<span data-ttu-id="dd845-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="dd845-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="dd845-141">请求</span><span class="sxs-lookup"><span data-stu-id="dd845-141">Request</span></span>

<span data-ttu-id="dd845-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dd845-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd845-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd845-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="javascript"></a>[<span data-ttu-id="dd845-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd845-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd845-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd845-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd845-146">响应</span><span class="sxs-lookup"><span data-stu-id="dd845-146">Response</span></span>

<span data-ttu-id="dd845-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dd845-147">The following is an example of the response.</span></span>
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
