---
title: timeOffRequest：批准
description: 批准 timeoffrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5df1ebc343bc22b359e889c31743f3c321c86f9d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863664"
---
# <a name="timeoffrequest-approve"></a><span data-ttu-id="1c02e-103">timeOffRequest：批准</span><span class="sxs-lookup"><span data-stu-id="1c02e-103">timeOffRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c02e-104">批准[timeoffrequest](../resources/timeoffrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="1c02e-104">Approve a [timeoffrequest](../resources/timeoffrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c02e-105">权限</span><span class="sxs-lookup"><span data-stu-id="1c02e-105">Permissions</span></span>

<span data-ttu-id="1c02e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c02e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c02e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c02e-108">Permission type</span></span>                        | <span data-ttu-id="1c02e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c02e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c02e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c02e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c02e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c02e-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1c02e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c02e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c02e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c02e-113">Not supported.</span></span> |
|<span data-ttu-id="1c02e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c02e-114">Application</span></span> | <span data-ttu-id="1c02e-115">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="1c02e-115">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="1c02e-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="1c02e-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="1c02e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c02e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="1c02e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c02e-118">Request headers</span></span>

| <span data-ttu-id="1c02e-119">名称</span><span class="sxs-lookup"><span data-stu-id="1c02e-119">Name</span></span>          | <span data-ttu-id="1c02e-120">说明</span><span class="sxs-lookup"><span data-stu-id="1c02e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1c02e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c02e-121">Authorization</span></span> | <span data-ttu-id="1c02e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c02e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c02e-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="1c02e-124">Content-type</span></span> | <span data-ttu-id="1c02e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1c02e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c02e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c02e-127">Request body</span></span>

<span data-ttu-id="1c02e-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1c02e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c02e-129">参数</span><span class="sxs-lookup"><span data-stu-id="1c02e-129">Parameter</span></span>    | <span data-ttu-id="1c02e-130">类型</span><span class="sxs-lookup"><span data-stu-id="1c02e-130">Type</span></span>        | <span data-ttu-id="1c02e-131">描述</span><span class="sxs-lookup"><span data-stu-id="1c02e-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c02e-132">message</span><span class="sxs-lookup"><span data-stu-id="1c02e-132">message</span></span>|<span data-ttu-id="1c02e-133">String</span><span class="sxs-lookup"><span data-stu-id="1c02e-133">String</span></span>|<span data-ttu-id="1c02e-134">自定义审批邮件。</span><span class="sxs-lookup"><span data-stu-id="1c02e-134">Custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="1c02e-135">响应</span><span class="sxs-lookup"><span data-stu-id="1c02e-135">Response</span></span>

<span data-ttu-id="1c02e-p104">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1c02e-p104">If successful, this method returns a `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c02e-138">示例</span><span class="sxs-lookup"><span data-stu-id="1c02e-138">Examples</span></span>

<span data-ttu-id="1c02e-139">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1c02e-139">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1c02e-140">请求</span><span class="sxs-lookup"><span data-stu-id="1c02e-140">Request</span></span>

<span data-ttu-id="1c02e-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1c02e-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1c02e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c02e-142">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c02e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c02e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c02e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c02e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1c02e-145">响应</span><span class="sxs-lookup"><span data-stu-id="1c02e-145">Response</span></span>

<span data-ttu-id="1c02e-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1c02e-146">The following is an example of the response.</span></span>
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
