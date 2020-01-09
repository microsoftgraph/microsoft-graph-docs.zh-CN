---
title: offerShiftRequest：批准
description: 批准 offershiftrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d1c7bfc627c6a8ff52fe78807783e0c4b88dc90e
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994942"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="0f669-103">offerShiftRequest：批准</span><span class="sxs-lookup"><span data-stu-id="0f669-103">offerShiftRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f669-104">批准[offershiftrequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0f669-104">Approve an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f669-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="0f669-105">Permissions</span></span>

<span data-ttu-id="0f669-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f669-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0f669-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f669-108">Permission type</span></span>                        | <span data-ttu-id="0f669-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f669-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0f669-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f669-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f669-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f669-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="0f669-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f669-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f669-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f669-113">Not supported.</span></span> |
| <span data-ttu-id="0f669-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f669-114">Application</span></span>                            | <span data-ttu-id="0f669-115">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="0f669-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="0f669-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="0f669-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="0f669-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f669-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="0f669-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f669-118">Request headers</span></span>

| <span data-ttu-id="0f669-119">名称</span><span class="sxs-lookup"><span data-stu-id="0f669-119">Name</span></span>          | <span data-ttu-id="0f669-120">说明</span><span class="sxs-lookup"><span data-stu-id="0f669-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0f669-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f669-121">Authorization</span></span> | <span data-ttu-id="0f669-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f669-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0f669-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="0f669-124">Content-type</span></span> | <span data-ttu-id="0f669-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0f669-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f669-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f669-127">Request body</span></span>

<span data-ttu-id="0f669-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0f669-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0f669-129">参数</span><span class="sxs-lookup"><span data-stu-id="0f669-129">Parameter</span></span>    | <span data-ttu-id="0f669-130">类型</span><span class="sxs-lookup"><span data-stu-id="0f669-130">Type</span></span>        | <span data-ttu-id="0f669-131">描述</span><span class="sxs-lookup"><span data-stu-id="0f669-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0f669-132">message</span><span class="sxs-lookup"><span data-stu-id="0f669-132">message</span></span>|<span data-ttu-id="0f669-133">String</span><span class="sxs-lookup"><span data-stu-id="0f669-133">String</span></span>|<span data-ttu-id="0f669-134">在审批时发送的自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="0f669-134">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="0f669-135">响应</span><span class="sxs-lookup"><span data-stu-id="0f669-135">Response</span></span>

<span data-ttu-id="0f669-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0f669-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f669-138">示例</span><span class="sxs-lookup"><span data-stu-id="0f669-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f669-139">请求</span><span class="sxs-lookup"><span data-stu-id="0f669-139">Request</span></span>

<span data-ttu-id="0f669-140">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="0f669-140">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0f669-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f669-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0f669-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f669-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f669-143">响应</span><span class="sxs-lookup"><span data-stu-id="0f669-143">Response</span></span>

<span data-ttu-id="0f669-144">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="0f669-144">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
