---
title: 更新 shiftPreferences
description: 更新用户的 shift 首选项。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 998a96fdf9ee874a3ae58a6029d31f270117fdca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040187"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="941a7-103">更新 shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="941a7-103">Update shiftPreferences</span></span>

<span data-ttu-id="941a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="941a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="941a7-105">更新 [shiftPreferences](../resources/shiftpreferences.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="941a7-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="941a7-106">权限</span><span class="sxs-lookup"><span data-stu-id="941a7-106">Permissions</span></span>

<span data-ttu-id="941a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="941a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="941a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="941a7-109">Permission type</span></span>      | <span data-ttu-id="941a7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="941a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="941a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="941a7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="941a7-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941a7-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="941a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="941a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="941a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="941a7-114">Not supported.</span></span>    |
|<span data-ttu-id="941a7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="941a7-115">Application</span></span> | <span data-ttu-id="941a7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="941a7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="941a7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="941a7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="941a7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="941a7-118">Request headers</span></span>

| <span data-ttu-id="941a7-119">标头</span><span class="sxs-lookup"><span data-stu-id="941a7-119">Header</span></span>       | <span data-ttu-id="941a7-120">值</span><span class="sxs-lookup"><span data-stu-id="941a7-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="941a7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="941a7-121">Authorization</span></span>  | <span data-ttu-id="941a7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="941a7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="941a7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="941a7-124">Content-Type</span></span>  | <span data-ttu-id="941a7-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="941a7-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="941a7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="941a7-127">Request body</span></span>
<span data-ttu-id="941a7-128">在请求正文中，提供 [shiftPreferences](../resources/shiftpreferences.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="941a7-128">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="941a7-129">响应</span><span class="sxs-lookup"><span data-stu-id="941a7-129">Response</span></span>

<span data-ttu-id="941a7-130">如果成功，此方法返回 `204 NO CONTENT` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="941a7-130">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="941a7-131">示例</span><span class="sxs-lookup"><span data-stu-id="941a7-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="941a7-132">请求</span><span class="sxs-lookup"><span data-stu-id="941a7-132">Request</span></span>

<span data-ttu-id="941a7-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="941a7-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="941a7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="941a7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
PUT https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
Content-type: application/json

{
    "id": "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
    "availability": [
        {
            "recurrence": {
                "pattern": {
                    "type": "Weekly",
                    "daysOfWeek": ["Monday", "Wednesday", "Friday"],
                    "interval": 1
                },
                "range": {
                    "type": "noEnd"
                }
            },
            "timeZone": "Pacific Standard Time",
            "timeSlots": null
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="941a7-135">C#</span><span class="sxs-lookup"><span data-stu-id="941a7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="941a7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="941a7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="941a7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="941a7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="941a7-138">响应</span><span class="sxs-lookup"><span data-stu-id="941a7-138">Response</span></span>

<span data-ttu-id="941a7-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="941a7-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response", 
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-12-12 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update a user's shift preferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


