---
title: 创建 timeOffReason
description: 创建新的 timeOffReason。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 297b3188de82b432cb3dab4e198b8bf6ae41d835
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052717"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="ceba9-103">创建 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="ceba9-103">Create timeOffReason</span></span>

<span data-ttu-id="ceba9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceba9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ceba9-105">创建新的 [timeOffReason](../resources/timeoffreason.md)。</span><span class="sxs-lookup"><span data-stu-id="ceba9-105">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ceba9-106">权限</span><span class="sxs-lookup"><span data-stu-id="ceba9-106">Permissions</span></span>

<span data-ttu-id="ceba9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ceba9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceba9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ceba9-109">Permission type</span></span>      | <span data-ttu-id="ceba9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ceba9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ceba9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ceba9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ceba9-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceba9-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ceba9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ceba9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceba9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ceba9-114">Not supported.</span></span>    |
|<span data-ttu-id="ceba9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ceba9-115">Application</span></span> | <span data-ttu-id="ceba9-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="ceba9-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="ceba9-117">\***重要提示：** 应用程序权限目前仅为个人预览版，不可公开使用。</span><span class="sxs-lookup"><span data-stu-id="ceba9-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="ceba9-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="ceba9-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ceba9-119">全局管理员可以访问他们不是其成员组。</span><span class="sxs-lookup"><span data-stu-id="ceba9-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ceba9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ceba9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="ceba9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ceba9-121">Request headers</span></span>

| <span data-ttu-id="ceba9-122">标头</span><span class="sxs-lookup"><span data-stu-id="ceba9-122">Header</span></span>       | <span data-ttu-id="ceba9-123">值</span><span class="sxs-lookup"><span data-stu-id="ceba9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ceba9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceba9-124">Authorization</span></span>  | <span data-ttu-id="ceba9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ceba9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ceba9-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ceba9-127">Content-Type</span></span>  | <span data-ttu-id="ceba9-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ceba9-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="ceba9-130">响应</span><span class="sxs-lookup"><span data-stu-id="ceba9-130">Response</span></span>

<span data-ttu-id="ceba9-131">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [timeOffReason](../resources/timeoffreason.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ceba9-131">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ceba9-132">示例</span><span class="sxs-lookup"><span data-stu-id="ceba9-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ceba9-133">请求</span><span class="sxs-lookup"><span data-stu-id="ceba9-133">Request</span></span>

<span data-ttu-id="ceba9-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ceba9-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ceba9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ceba9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-timeoffreasons"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
Content-type: application/json

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```
# <a name="c"></a>[<span data-ttu-id="ceba9-136">C#</span><span class="sxs-lookup"><span data-stu-id="ceba9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ceba9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ceba9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ceba9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ceba9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ceba9-139">Java</span><span class="sxs-lookup"><span data-stu-id="ceba9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-timeoffreasons-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ceba9-140">响应</span><span class="sxs-lookup"><span data-stu-id="ceba9-140">Response</span></span>

<span data-ttu-id="ceba9-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ceba9-141">The following is an example of the response.</span></span> 

><span data-ttu-id="ceba9-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ceba9-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


