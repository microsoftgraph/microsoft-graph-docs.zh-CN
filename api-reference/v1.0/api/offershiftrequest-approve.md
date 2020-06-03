---
title: offerShiftRequest：批准
description: 批准 offerShiftRequest 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5e1d9058fb3f4da69fa8cfb8886f92aff81c65fa
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44218164"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="14cc9-103">offerShiftRequest：批准</span><span class="sxs-lookup"><span data-stu-id="14cc9-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="14cc9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14cc9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14cc9-105">批准[offerShiftRequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="14cc9-105">Approve an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14cc9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="14cc9-106">Permissions</span></span>

<span data-ttu-id="14cc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14cc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14cc9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="14cc9-109">Permission type</span></span>                        | <span data-ttu-id="14cc9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="14cc9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14cc9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14cc9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14cc9-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="14cc9-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="14cc9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14cc9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14cc9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="14cc9-114">Not supported.</span></span> |
| <span data-ttu-id="14cc9-115">Application</span><span class="sxs-lookup"><span data-stu-id="14cc9-115">Application</span></span>                            | <span data-ttu-id="14cc9-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14cc9-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="14cc9-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="14cc9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="14cc9-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="14cc9-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="14cc9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14cc9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="14cc9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="14cc9-120">Request headers</span></span>

| <span data-ttu-id="14cc9-121">名称</span><span class="sxs-lookup"><span data-stu-id="14cc9-121">Name</span></span>          | <span data-ttu-id="14cc9-122">说明</span><span class="sxs-lookup"><span data-stu-id="14cc9-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="14cc9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14cc9-123">Authorization</span></span> | <span data-ttu-id="14cc9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="14cc9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14cc9-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="14cc9-126">Content-type</span></span> | <span data-ttu-id="14cc9-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="14cc9-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14cc9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="14cc9-129">Request body</span></span>

<span data-ttu-id="14cc9-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="14cc9-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="14cc9-131">参数</span><span class="sxs-lookup"><span data-stu-id="14cc9-131">Parameter</span></span>    | <span data-ttu-id="14cc9-132">类型</span><span class="sxs-lookup"><span data-stu-id="14cc9-132">Type</span></span>        | <span data-ttu-id="14cc9-133">描述</span><span class="sxs-lookup"><span data-stu-id="14cc9-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14cc9-134">message</span><span class="sxs-lookup"><span data-stu-id="14cc9-134">message</span></span>|<span data-ttu-id="14cc9-135">String</span><span class="sxs-lookup"><span data-stu-id="14cc9-135">String</span></span>|<span data-ttu-id="14cc9-136">在审批时发送的自定义邮件。</span><span class="sxs-lookup"><span data-stu-id="14cc9-136">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="14cc9-137">响应</span><span class="sxs-lookup"><span data-stu-id="14cc9-137">Response</span></span>

<span data-ttu-id="14cc9-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="14cc9-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14cc9-140">示例</span><span class="sxs-lookup"><span data-stu-id="14cc9-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14cc9-141">请求</span><span class="sxs-lookup"><span data-stu-id="14cc9-141">Request</span></span>

<span data-ttu-id="14cc9-142">以下示例显示了一个请求。</span><span class="sxs-lookup"><span data-stu-id="14cc9-142">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14cc9-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="14cc9-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
# <a name="c"></a>[<span data-ttu-id="14cc9-144">C#</span><span class="sxs-lookup"><span data-stu-id="14cc9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14cc9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14cc9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14cc9-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14cc9-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14cc9-147">Java</span><span class="sxs-lookup"><span data-stu-id="14cc9-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="14cc9-148">响应</span><span class="sxs-lookup"><span data-stu-id="14cc9-148">Response</span></span>

<span data-ttu-id="14cc9-149">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="14cc9-149">The following example shows the response.</span></span>
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
