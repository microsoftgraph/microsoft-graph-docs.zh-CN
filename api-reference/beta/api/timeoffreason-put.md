---
title: 替换 timeOffReason
description: 替换现有的 timeOffReason。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8c37304d6556bfcee47a0bb631933f29cd8b3986
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657810"
---
# <a name="replace-timeoffreason"></a><span data-ttu-id="83924-103">替换 timeOffReason</span><span class="sxs-lookup"><span data-stu-id="83924-103">Replace timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83924-104">替换现有的[timeOffReason](../resources/timeoffreason.md)。</span><span class="sxs-lookup"><span data-stu-id="83924-104">Replace an existing [timeOffReason](../resources/timeoffreason.md).</span></span>

<span data-ttu-id="83924-105">如果指定的[timeOffReason](../resources/timeoffreason.md)不存在, 则此方法`404 Not found`返回。</span><span class="sxs-lookup"><span data-stu-id="83924-105">If the specified [timeOffReason](../resources/timeoffreason.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="83924-106">权限</span><span class="sxs-lookup"><span data-stu-id="83924-106">Permissions</span></span>

<span data-ttu-id="83924-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83924-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83924-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83924-109">Permission type</span></span>      | <span data-ttu-id="83924-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83924-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83924-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83924-111">Delegated (work or school account)</span></span> | <span data-ttu-id="83924-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83924-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="83924-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83924-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83924-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83924-114">Not supported.</span></span>    |
|<span data-ttu-id="83924-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83924-115">Application</span></span> | <span data-ttu-id="83924-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83924-116">Not supported.</span></span> |

> <span data-ttu-id="83924-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="83924-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="83924-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="83924-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="83924-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83924-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="83924-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="83924-120">Request headers</span></span>

| <span data-ttu-id="83924-121">标头</span><span class="sxs-lookup"><span data-stu-id="83924-121">Header</span></span>       | <span data-ttu-id="83924-122">值</span><span class="sxs-lookup"><span data-stu-id="83924-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83924-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83924-123">Authorization</span></span>  | <span data-ttu-id="83924-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83924-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="83924-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83924-126">Content-Type</span></span>  | <span data-ttu-id="83924-127">application/json</span><span class="sxs-lookup"><span data-stu-id="83924-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83924-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="83924-128">Request body</span></span>

<span data-ttu-id="83924-129">在请求正文中, 提供[timeOffReason](../resources/timeoffreason.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83924-129">In the request body, supply a JSON representation of a [timeOffReason](../resources/timeoffreason.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="83924-130">响应</span><span class="sxs-lookup"><span data-stu-id="83924-130">Response</span></span>

<span data-ttu-id="83924-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[timeOffReason](../resources/timeoffreason.md)对象。</span><span class="sxs-lookup"><span data-stu-id="83924-131">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83924-132">示例</span><span class="sxs-lookup"><span data-stu-id="83924-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="83924-133">请求</span><span class="sxs-lookup"><span data-stu-id="83924-133">Request</span></span>

<span data-ttu-id="83924-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="83924-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```

#### <a name="response"></a><span data-ttu-id="83924-135">响应</span><span class="sxs-lookup"><span data-stu-id="83924-135">Response</span></span>

<span data-ttu-id="83924-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="83924-136">The following is an example of the response.</span></span> 

><span data-ttu-id="83924-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="83924-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Replace an existing timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
