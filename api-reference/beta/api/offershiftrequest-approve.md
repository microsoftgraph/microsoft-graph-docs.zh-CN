---
title: offerShiftRequest：批准
description: 批准 offershiftrequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aef00c4de700624eac54e3aca8bbc2773799b377
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456605"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="7fa1f-103">offerShiftRequest：批准</span><span class="sxs-lookup"><span data-stu-id="7fa1f-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="7fa1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fa1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fa1f-105">批准[offershiftrequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-105">Approve an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fa1f-106">权限</span><span class="sxs-lookup"><span data-stu-id="7fa1f-106">Permissions</span></span>

<span data-ttu-id="7fa1f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7fa1f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7fa1f-109">Permission type</span></span>                        | <span data-ttu-id="7fa1f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7fa1f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7fa1f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7fa1f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7fa1f-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fa1f-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="7fa1f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7fa1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fa1f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-114">Not supported.</span></span> |
| <span data-ttu-id="7fa1f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fa1f-115">Application</span></span>                            | <span data-ttu-id="7fa1f-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="7fa1f-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="7fa1f-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="7fa1f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7fa1f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/schedule/offerShiftRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="7fa1f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7fa1f-119">Request headers</span></span>

| <span data-ttu-id="7fa1f-120">名称</span><span class="sxs-lookup"><span data-stu-id="7fa1f-120">Name</span></span>          | <span data-ttu-id="7fa1f-121">说明</span><span class="sxs-lookup"><span data-stu-id="7fa1f-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7fa1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fa1f-122">Authorization</span></span> | <span data-ttu-id="7fa1f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7fa1f-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="7fa1f-125">Content-type</span></span> | <span data-ttu-id="7fa1f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7fa1f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fa1f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="7fa1f-128">Request body</span></span>

<span data-ttu-id="7fa1f-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7fa1f-130">参数</span><span class="sxs-lookup"><span data-stu-id="7fa1f-130">Parameter</span></span>    | <span data-ttu-id="7fa1f-131">类型</span><span class="sxs-lookup"><span data-stu-id="7fa1f-131">Type</span></span>        | <span data-ttu-id="7fa1f-132">描述</span><span class="sxs-lookup"><span data-stu-id="7fa1f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7fa1f-133">message</span><span class="sxs-lookup"><span data-stu-id="7fa1f-133">message</span></span>|<span data-ttu-id="7fa1f-134">String</span><span class="sxs-lookup"><span data-stu-id="7fa1f-134">String</span></span>|<span data-ttu-id="7fa1f-135">在审批时发送的自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-135">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="7fa1f-136">响应</span><span class="sxs-lookup"><span data-stu-id="7fa1f-136">Response</span></span>

<span data-ttu-id="7fa1f-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fa1f-139">示例</span><span class="sxs-lookup"><span data-stu-id="7fa1f-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7fa1f-140">请求</span><span class="sxs-lookup"><span data-stu-id="7fa1f-140">Request</span></span>

<span data-ttu-id="7fa1f-141">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-141">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fa1f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fa1f-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="7fa1f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fa1f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7fa1f-144">响应</span><span class="sxs-lookup"><span data-stu-id="7fa1f-144">Response</span></span>

<span data-ttu-id="7fa1f-145">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="7fa1f-145">The following example shows the response.</span></span>
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
