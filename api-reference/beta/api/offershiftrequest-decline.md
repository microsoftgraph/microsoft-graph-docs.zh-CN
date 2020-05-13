---
title: offerShiftRequest：拒绝
description: 拒绝促销活动请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c3edf437b87af8bc222a51c1532367e12ad44953
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217006"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="4fbbb-103">offerShiftRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="4fbbb-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="4fbbb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fbbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fbbb-105">拒绝[offershiftrequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-105">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fbbb-106">权限</span><span class="sxs-lookup"><span data-stu-id="4fbbb-106">Permissions</span></span>

<span data-ttu-id="4fbbb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4fbbb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fbbb-109">Permission type</span></span>                        | <span data-ttu-id="4fbbb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4fbbb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4fbbb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fbbb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4fbbb-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fbbb-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="4fbbb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fbbb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4fbbb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-114">Not supported.</span></span> |
| <span data-ttu-id="4fbbb-115">Application</span><span class="sxs-lookup"><span data-stu-id="4fbbb-115">Application</span></span>                            | <span data-ttu-id="4fbbb-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="4fbbb-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="4fbbb-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="4fbbb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fbbb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="4fbbb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fbbb-119">Request headers</span></span>

| <span data-ttu-id="4fbbb-120">名称</span><span class="sxs-lookup"><span data-stu-id="4fbbb-120">Name</span></span>          | <span data-ttu-id="4fbbb-121">说明</span><span class="sxs-lookup"><span data-stu-id="4fbbb-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4fbbb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fbbb-122">Authorization</span></span> | <span data-ttu-id="4fbbb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4fbbb-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="4fbbb-125">Content-type</span></span> | <span data-ttu-id="4fbbb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4fbbb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fbbb-128">Request body</span></span>

<span data-ttu-id="4fbbb-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4fbbb-130">参数</span><span class="sxs-lookup"><span data-stu-id="4fbbb-130">Parameter</span></span>    | <span data-ttu-id="4fbbb-131">类型</span><span class="sxs-lookup"><span data-stu-id="4fbbb-131">Type</span></span>        | <span data-ttu-id="4fbbb-132">描述</span><span class="sxs-lookup"><span data-stu-id="4fbbb-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4fbbb-133">message</span><span class="sxs-lookup"><span data-stu-id="4fbbb-133">message</span></span>|<span data-ttu-id="4fbbb-134">String</span><span class="sxs-lookup"><span data-stu-id="4fbbb-134">String</span></span>|<span data-ttu-id="4fbbb-135">在拒绝时发送自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-135">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="4fbbb-136">响应</span><span class="sxs-lookup"><span data-stu-id="4fbbb-136">Response</span></span>

<span data-ttu-id="4fbbb-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4fbbb-139">示例</span><span class="sxs-lookup"><span data-stu-id="4fbbb-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4fbbb-140">请求</span><span class="sxs-lookup"><span data-stu-id="4fbbb-140">Request</span></span>

<span data-ttu-id="4fbbb-141">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-141">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4fbbb-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4fbbb-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="javascript"></a>[<span data-ttu-id="4fbbb-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4fbbb-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="4fbbb-144">C#</span><span class="sxs-lookup"><span data-stu-id="4fbbb-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4fbbb-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4fbbb-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4fbbb-146">响应</span><span class="sxs-lookup"><span data-stu-id="4fbbb-146">Response</span></span>

<span data-ttu-id="4fbbb-147">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="4fbbb-147">The following example shows the response.</span></span>
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
