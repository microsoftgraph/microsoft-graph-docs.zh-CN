---
title: swapShiftsChangeRequest：拒绝
description: 拒绝交换转换请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d2b53c049dfb1213fdae049e0d8f1cb72b6a1f95
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217456"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="0b029-103">swapShiftsChangeRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="0b029-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="0b029-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b029-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b029-105">拒绝[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b029-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b029-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0b029-106">Permissions</span></span>

<span data-ttu-id="0b029-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b029-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b029-109">Permission type</span></span>                        | <span data-ttu-id="0b029-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b029-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="0b029-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b029-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0b029-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="0b029-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0b029-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b029-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b029-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b029-114">Not supported.</span></span>    |<span data-ttu-id="0b029-115">s</span><span class="sxs-lookup"><span data-stu-id="0b029-115">s</span></span>
|<span data-ttu-id="0b029-116">Application</span><span class="sxs-lookup"><span data-stu-id="0b029-116">Application</span></span> | <span data-ttu-id="0b029-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b029-117">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="0b029-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0b029-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0b029-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="0b029-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0b029-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b029-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="0b029-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b029-121">Request headers</span></span>

| <span data-ttu-id="0b029-122">名称</span><span class="sxs-lookup"><span data-stu-id="0b029-122">Name</span></span>          | <span data-ttu-id="0b029-123">说明</span><span class="sxs-lookup"><span data-stu-id="0b029-123">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0b029-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b029-124">Authorization</span></span> | <span data-ttu-id="0b029-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b029-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0b029-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="0b029-127">Content-type</span></span> | <span data-ttu-id="0b029-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0b029-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b029-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b029-130">Request body</span></span>

<span data-ttu-id="0b029-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0b029-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0b029-132">参数</span><span class="sxs-lookup"><span data-stu-id="0b029-132">Parameter</span></span>    | <span data-ttu-id="0b029-133">类型</span><span class="sxs-lookup"><span data-stu-id="0b029-133">Type</span></span>        | <span data-ttu-id="0b029-134">描述</span><span class="sxs-lookup"><span data-stu-id="0b029-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b029-135">message</span><span class="sxs-lookup"><span data-stu-id="0b029-135">message</span></span>|<span data-ttu-id="0b029-136">String</span><span class="sxs-lookup"><span data-stu-id="0b029-136">String</span></span>|<span data-ttu-id="0b029-137">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="0b029-137">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="0b029-138">响应</span><span class="sxs-lookup"><span data-stu-id="0b029-138">Response</span></span>

<span data-ttu-id="0b029-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0b029-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b029-141">示例</span><span class="sxs-lookup"><span data-stu-id="0b029-141">Examples</span></span>

<span data-ttu-id="0b029-142">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="0b029-142">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="0b029-143">请求</span><span class="sxs-lookup"><span data-stu-id="0b029-143">Request</span></span>

<span data-ttu-id="0b029-144">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="0b029-144">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b029-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b029-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="0b029-146">C#</span><span class="sxs-lookup"><span data-stu-id="0b029-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b029-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b029-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b029-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b029-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b029-149">Java</span><span class="sxs-lookup"><span data-stu-id="0b029-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="0b029-150">响应</span><span class="sxs-lookup"><span data-stu-id="0b029-150">Response</span></span>

<span data-ttu-id="0b029-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b029-151">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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
