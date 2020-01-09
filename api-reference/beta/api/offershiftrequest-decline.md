---
title: offerShiftRequest：拒绝
description: 拒绝促销活动请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 92a085bb089c549bf4860dcbce135cd4f887ea48
ms.sourcegitcommit: 66c8fcafee151278f8089cd26d0c5766d33d04a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2020
ms.locfileid: "40994928"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="cdd4e-103">offerShiftRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="cdd4e-103">offerShiftRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdd4e-104">拒绝[offershiftrequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-104">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdd4e-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="cdd4e-105">Permissions</span></span>

<span data-ttu-id="cdd4e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cdd4e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdd4e-108">Permission type</span></span>                        | <span data-ttu-id="cdd4e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdd4e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cdd4e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdd4e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cdd4e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdd4e-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cdd4e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdd4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdd4e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-113">Not supported.</span></span> |
| <span data-ttu-id="cdd4e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdd4e-114">Application</span></span>                            | <span data-ttu-id="cdd4e-115">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="cdd4e-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="cdd4e-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="cdd4e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdd4e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/decline
```

## <a name="request-headers"></a><span data-ttu-id="cdd4e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdd4e-118">Request headers</span></span>

| <span data-ttu-id="cdd4e-119">名称</span><span class="sxs-lookup"><span data-stu-id="cdd4e-119">Name</span></span>          | <span data-ttu-id="cdd4e-120">说明</span><span class="sxs-lookup"><span data-stu-id="cdd4e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cdd4e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdd4e-121">Authorization</span></span> | <span data-ttu-id="cdd4e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cdd4e-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="cdd4e-124">Content-type</span></span> | <span data-ttu-id="cdd4e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cdd4e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdd4e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdd4e-127">Request body</span></span>

<span data-ttu-id="cdd4e-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cdd4e-129">参数</span><span class="sxs-lookup"><span data-stu-id="cdd4e-129">Parameter</span></span>    | <span data-ttu-id="cdd4e-130">类型</span><span class="sxs-lookup"><span data-stu-id="cdd4e-130">Type</span></span>        | <span data-ttu-id="cdd4e-131">描述</span><span class="sxs-lookup"><span data-stu-id="cdd4e-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cdd4e-132">message</span><span class="sxs-lookup"><span data-stu-id="cdd4e-132">message</span></span>|<span data-ttu-id="cdd4e-133">String</span><span class="sxs-lookup"><span data-stu-id="cdd4e-133">String</span></span>|<span data-ttu-id="cdd4e-134">在拒绝时发送自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-134">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="cdd4e-135">响应</span><span class="sxs-lookup"><span data-stu-id="cdd4e-135">Response</span></span>

<span data-ttu-id="cdd4e-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdd4e-138">示例</span><span class="sxs-lookup"><span data-stu-id="cdd4e-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cdd4e-139">请求</span><span class="sxs-lookup"><span data-stu-id="cdd4e-139">Request</span></span>

<span data-ttu-id="cdd4e-140">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-140">The following example shows a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cdd4e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdd4e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cdd4e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdd4e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cdd4e-143">响应</span><span class="sxs-lookup"><span data-stu-id="cdd4e-143">Response</span></span>

<span data-ttu-id="cdd4e-144">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="cdd4e-144">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
