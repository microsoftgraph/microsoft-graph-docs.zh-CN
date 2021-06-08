---
title: offerShiftRequest： decline
description: 拒绝产品/服务班次请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9cdb5fbe381008b4146d649fb862b25a3687c251
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786330"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="3ab1d-103">offerShiftRequest： decline</span><span class="sxs-lookup"><span data-stu-id="3ab1d-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="3ab1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ab1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ab1d-105">拒绝 [offerShiftRequest](../resources/offershiftrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3ab1d-105">Decline an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ab1d-106">权限</span><span class="sxs-lookup"><span data-stu-id="3ab1d-106">Permissions</span></span>

<span data-ttu-id="3ab1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ab1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ab1d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ab1d-109">Permission type</span></span>                        | <span data-ttu-id="3ab1d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ab1d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ab1d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ab1d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ab1d-112">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ab1d-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="3ab1d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ab1d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ab1d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ab1d-114">Not supported.</span></span> |
| <span data-ttu-id="3ab1d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ab1d-115">Application</span></span>                            | <span data-ttu-id="3ab1d-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ab1d-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ab1d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ab1d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="3ab1d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ab1d-118">Request headers</span></span>

| <span data-ttu-id="3ab1d-119">名称</span><span class="sxs-lookup"><span data-stu-id="3ab1d-119">Name</span></span>          | <span data-ttu-id="3ab1d-120">说明</span><span class="sxs-lookup"><span data-stu-id="3ab1d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3ab1d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ab1d-121">Authorization</span></span> | <span data-ttu-id="3ab1d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ab1d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ab1d-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="3ab1d-124">Content-type</span></span> | <span data-ttu-id="3ab1d-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3ab1d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ab1d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ab1d-127">Request body</span></span>

<span data-ttu-id="3ab1d-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3ab1d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ab1d-129">参数</span><span class="sxs-lookup"><span data-stu-id="3ab1d-129">Parameter</span></span>    | <span data-ttu-id="3ab1d-130">类型</span><span class="sxs-lookup"><span data-stu-id="3ab1d-130">Type</span></span>        | <span data-ttu-id="3ab1d-131">描述</span><span class="sxs-lookup"><span data-stu-id="3ab1d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ab1d-132">message</span><span class="sxs-lookup"><span data-stu-id="3ab1d-132">message</span></span>|<span data-ttu-id="3ab1d-133">String</span><span class="sxs-lookup"><span data-stu-id="3ab1d-133">String</span></span>|<span data-ttu-id="3ab1d-134">拒绝发送的自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="3ab1d-134">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="3ab1d-135">响应</span><span class="sxs-lookup"><span data-stu-id="3ab1d-135">Response</span></span>

<span data-ttu-id="3ab1d-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3ab1d-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ab1d-138">示例</span><span class="sxs-lookup"><span data-stu-id="3ab1d-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ab1d-139">请求</span><span class="sxs-lookup"><span data-stu-id="3ab1d-139">Request</span></span>

<span data-ttu-id="3ab1d-140">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="3ab1d-140">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3ab1d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ab1d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="c"></a>[<span data-ttu-id="3ab1d-142">C#</span><span class="sxs-lookup"><span data-stu-id="3ab1d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ab1d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ab1d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ab1d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ab1d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ab1d-145">Java</span><span class="sxs-lookup"><span data-stu-id="3ab1d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="3ab1d-146">响应</span><span class="sxs-lookup"><span data-stu-id="3ab1d-146">Response</span></span>

<span data-ttu-id="3ab1d-147">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="3ab1d-147">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
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

