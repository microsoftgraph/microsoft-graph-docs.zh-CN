---
title: 获取 timeOffRequest
description: 检索 timeOffRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 99683f33448c4d7b492b19f07f2f0fc704b73753
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52034390"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="9a387-103">获取 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="9a387-103">Get timeOffRequest</span></span>

<span data-ttu-id="9a387-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a387-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9a387-105">检索 [timeoffrequest 对象的属性和](../resources/timeoffrequest.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="9a387-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a387-106">权限</span><span class="sxs-lookup"><span data-stu-id="9a387-106">Permissions</span></span>

<span data-ttu-id="9a387-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a387-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a387-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a387-109">Permission type</span></span>                        | <span data-ttu-id="9a387-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a387-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="9a387-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a387-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a387-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a387-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a387-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a387-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a387-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a387-114">Not supported.</span></span>    |
|<span data-ttu-id="9a387-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a387-115">Application</span></span> | <span data-ttu-id="9a387-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a387-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="9a387-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="9a387-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="9a387-118">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="9a387-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="9a387-119">目前仅在个人预览版中，不可用于公共用途。</span><span class="sxs-lookup"><span data-stu-id="9a387-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="9a387-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a387-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a387-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9a387-121">Optional query parameters</span></span>

<span data-ttu-id="9a387-122">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9a387-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a387-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a387-123">Request headers</span></span>

| <span data-ttu-id="9a387-124">名称</span><span class="sxs-lookup"><span data-stu-id="9a387-124">Name</span></span>      |<span data-ttu-id="9a387-125">说明</span><span class="sxs-lookup"><span data-stu-id="9a387-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a387-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a387-126">Authorization</span></span> | <span data-ttu-id="9a387-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a387-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a387-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a387-129">Request body</span></span>

<span data-ttu-id="9a387-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9a387-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a387-131">响应</span><span class="sxs-lookup"><span data-stu-id="9a387-131">Response</span></span>

<span data-ttu-id="9a387-132">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [timeOffRequest](../resources/timeoffrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9a387-132">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a387-133">示例</span><span class="sxs-lookup"><span data-stu-id="9a387-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a387-134">请求</span><span class="sxs-lookup"><span data-stu-id="9a387-134">Request</span></span>

<span data-ttu-id="9a387-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a387-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9a387-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a387-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="9a387-137">C#</span><span class="sxs-lookup"><span data-stu-id="9a387-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a387-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a387-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a387-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a387-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a387-140">Java</span><span class="sxs-lookup"><span data-stu-id="9a387-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="9a387-141">响应</span><span class="sxs-lookup"><span data-stu-id="9a387-141">Response</span></span>

<span data-ttu-id="9a387-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9a387-142">The following is an example of the response.</span></span>

> <span data-ttu-id="9a387-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9a387-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "startDateTime": "datetime-value",
  "endDateTime": "datetime-value",
  "timeOffReasonId": "timeOffReasonId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

