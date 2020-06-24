---
title: swapShiftsChangeRequest：拒绝
description: 拒绝交换转换请求。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4814fb3ef9d416d6d3bc5be1815b746277a25426
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846182"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="22b04-103">swapShiftsChangeRequest：拒绝</span><span class="sxs-lookup"><span data-stu-id="22b04-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="22b04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22b04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22b04-105">拒绝[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="22b04-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22b04-106">权限</span><span class="sxs-lookup"><span data-stu-id="22b04-106">Permissions</span></span>

<span data-ttu-id="22b04-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="22b04-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="22b04-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22b04-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22b04-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="22b04-109">Permission type</span></span>                        | <span data-ttu-id="22b04-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22b04-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22b04-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22b04-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22b04-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="22b04-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="22b04-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22b04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22b04-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="22b04-114">Not supported.</span></span>                              |
| <span data-ttu-id="22b04-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="22b04-115">Application</span></span>                            | <span data-ttu-id="22b04-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22b04-116">Schedule.ReadWrite.All</span></span>                      |

> <span data-ttu-id="22b04-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="22b04-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="22b04-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="22b04-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="22b04-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22b04-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="22b04-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="22b04-120">Request headers</span></span>

| <span data-ttu-id="22b04-121">名称</span><span class="sxs-lookup"><span data-stu-id="22b04-121">Name</span></span>          | <span data-ttu-id="22b04-122">说明</span><span class="sxs-lookup"><span data-stu-id="22b04-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="22b04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22b04-123">Authorization</span></span> | <span data-ttu-id="22b04-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="22b04-124">Bearer {token}.</span></span> <span data-ttu-id="22b04-125">Required.</span><span class="sxs-lookup"><span data-stu-id="22b04-125">Required.</span></span> |
| <span data-ttu-id="22b04-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="22b04-126">Content-type</span></span> | <span data-ttu-id="22b04-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="22b04-127">application/json.</span></span> <span data-ttu-id="22b04-128">Required.</span><span class="sxs-lookup"><span data-stu-id="22b04-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22b04-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="22b04-129">Request body</span></span>

<span data-ttu-id="22b04-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="22b04-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="22b04-131">参数</span><span class="sxs-lookup"><span data-stu-id="22b04-131">Parameter</span></span>    | <span data-ttu-id="22b04-132">类型</span><span class="sxs-lookup"><span data-stu-id="22b04-132">Type</span></span>        | <span data-ttu-id="22b04-133">描述</span><span class="sxs-lookup"><span data-stu-id="22b04-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22b04-134">message</span><span class="sxs-lookup"><span data-stu-id="22b04-134">message</span></span>|<span data-ttu-id="22b04-135">String</span><span class="sxs-lookup"><span data-stu-id="22b04-135">String</span></span>|<span data-ttu-id="22b04-136">自定义拒绝邮件。</span><span class="sxs-lookup"><span data-stu-id="22b04-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="22b04-137">响应</span><span class="sxs-lookup"><span data-stu-id="22b04-137">Response</span></span>

<span data-ttu-id="22b04-138">If successful, this method returns a `200 OK` response code.</span><span class="sxs-lookup"><span data-stu-id="22b04-138">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="22b04-139">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="22b04-139">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22b04-140">示例</span><span class="sxs-lookup"><span data-stu-id="22b04-140">Examples</span></span>

<span data-ttu-id="22b04-141">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="22b04-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="22b04-142">请求</span><span class="sxs-lookup"><span data-stu-id="22b04-142">Request</span></span>

<span data-ttu-id="22b04-143">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="22b04-143">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="22b04-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="22b04-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="22b04-145">C#</span><span class="sxs-lookup"><span data-stu-id="22b04-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22b04-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22b04-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22b04-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22b04-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22b04-148">Java</span><span class="sxs-lookup"><span data-stu-id="22b04-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="22b04-149">响应</span><span class="sxs-lookup"><span data-stu-id="22b04-149">Response</span></span>

<span data-ttu-id="22b04-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="22b04-150">The following is an example of the response.</span></span>
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
