---
title: swapShiftsChangeRequest： decline
description: 拒绝交换班次请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e94566fa87b9cd86bad56660db979650294ce49
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787189"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="83eec-103">swapShiftsChangeRequest： decline</span><span class="sxs-lookup"><span data-stu-id="83eec-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="83eec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83eec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83eec-105">拒绝 [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83eec-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="83eec-106">权限</span><span class="sxs-lookup"><span data-stu-id="83eec-106">Permissions</span></span>

<span data-ttu-id="83eec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83eec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="83eec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83eec-109">Permission type</span></span>                        | <span data-ttu-id="83eec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83eec-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="83eec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83eec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="83eec-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83eec-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="83eec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83eec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83eec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83eec-114">Not supported.</span></span> |
| <span data-ttu-id="83eec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83eec-115">Application</span></span>                            | <span data-ttu-id="83eec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83eec-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="83eec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83eec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="83eec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="83eec-118">Request headers</span></span>

| <span data-ttu-id="83eec-119">名称</span><span class="sxs-lookup"><span data-stu-id="83eec-119">Name</span></span>          | <span data-ttu-id="83eec-120">说明</span><span class="sxs-lookup"><span data-stu-id="83eec-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="83eec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83eec-121">Authorization</span></span> | <span data-ttu-id="83eec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83eec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="83eec-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="83eec-124">Content-type</span></span> | <span data-ttu-id="83eec-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="83eec-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83eec-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="83eec-127">Request body</span></span>

<span data-ttu-id="83eec-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="83eec-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="83eec-129">参数</span><span class="sxs-lookup"><span data-stu-id="83eec-129">Parameter</span></span>    | <span data-ttu-id="83eec-130">类型</span><span class="sxs-lookup"><span data-stu-id="83eec-130">Type</span></span>        | <span data-ttu-id="83eec-131">描述</span><span class="sxs-lookup"><span data-stu-id="83eec-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="83eec-132">message</span><span class="sxs-lookup"><span data-stu-id="83eec-132">message</span></span>|<span data-ttu-id="83eec-133">String</span><span class="sxs-lookup"><span data-stu-id="83eec-133">String</span></span>|<span data-ttu-id="83eec-134">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="83eec-134">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="83eec-135">响应</span><span class="sxs-lookup"><span data-stu-id="83eec-135">Response</span></span>

<span data-ttu-id="83eec-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="83eec-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83eec-138">示例</span><span class="sxs-lookup"><span data-stu-id="83eec-138">Examples</span></span>

<span data-ttu-id="83eec-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="83eec-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="83eec-140">请求</span><span class="sxs-lookup"><span data-stu-id="83eec-140">Request</span></span>

<span data-ttu-id="83eec-141">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="83eec-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="83eec-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="83eec-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="83eec-143">C#</span><span class="sxs-lookup"><span data-stu-id="83eec-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83eec-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83eec-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83eec-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83eec-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83eec-146">Java</span><span class="sxs-lookup"><span data-stu-id="83eec-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="83eec-147">响应</span><span class="sxs-lookup"><span data-stu-id="83eec-147">Response</span></span>

<span data-ttu-id="83eec-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="83eec-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


