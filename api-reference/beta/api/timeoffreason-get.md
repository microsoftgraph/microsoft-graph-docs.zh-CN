---
title: 获取 timeOffReason
description: 按 ID 获取 timeOffReason。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ad314b96290e772a18fb90a935c0eb6bc7392b02
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787336"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="ede19-103">获取 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ede19-103">Get timeOffReason</span></span>

<span data-ttu-id="ede19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ede19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ede19-105">按 ID 检索 [timeOffReason](../resources/timeoffreason.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ede19-105">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="ede19-106">权限</span><span class="sxs-lookup"><span data-stu-id="ede19-106">Permissions</span></span>

<span data-ttu-id="ede19-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ede19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ede19-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ede19-109">Permission type</span></span>      | <span data-ttu-id="ede19-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ede19-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ede19-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ede19-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ede19-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ede19-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ede19-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ede19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ede19-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ede19-114">Not supported.</span></span>    |
|<span data-ttu-id="ede19-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ede19-115">Application</span></span> | <span data-ttu-id="ede19-116">Schedule.Read.All *、Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="ede19-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span>  |

><span data-ttu-id="ede19-117">\***重要提示：** 应用程序权限目前仅为个人预览版，不可公开使用。</span><span class="sxs-lookup"><span data-stu-id="ede19-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="ede19-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="ede19-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ede19-119">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="ede19-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ede19-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ede19-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ede19-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ede19-121">Optional query parameters</span></span>

<span data-ttu-id="ede19-122">此方法不支持使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ede19-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ede19-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ede19-123">Request headers</span></span>

| <span data-ttu-id="ede19-124">标头</span><span class="sxs-lookup"><span data-stu-id="ede19-124">Header</span></span>       | <span data-ttu-id="ede19-125">值</span><span class="sxs-lookup"><span data-stu-id="ede19-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ede19-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ede19-126">Authorization</span></span>  | <span data-ttu-id="ede19-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ede19-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ede19-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ede19-129">Request body</span></span>
<span data-ttu-id="ede19-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ede19-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ede19-131">响应</span><span class="sxs-lookup"><span data-stu-id="ede19-131">Response</span></span>

<span data-ttu-id="ede19-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [timeOffReason](../resources/timeoffreason.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ede19-132">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ede19-133">示例</span><span class="sxs-lookup"><span data-stu-id="ede19-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ede19-134">请求</span><span class="sxs-lookup"><span data-stu-id="ede19-134">Request</span></span>

<span data-ttu-id="ede19-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ede19-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ede19-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ede19-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="ede19-137">C#</span><span class="sxs-lookup"><span data-stu-id="ede19-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ede19-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ede19-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ede19-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ede19-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ede19-140">Java</span><span class="sxs-lookup"><span data-stu-id="ede19-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ede19-141">响应</span><span class="sxs-lookup"><span data-stu-id="ede19-141">Response</span></span>

<span data-ttu-id="ede19-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ede19-142">The following is an example of the response.</span></span> 

><span data-ttu-id="ede19-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ede19-143">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOffReason by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


