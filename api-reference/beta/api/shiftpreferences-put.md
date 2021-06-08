---
title: 更新 shiftPreferences
description: 更新用户的班次首选项。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3a209d5266fb841cff4011255be98ac6d9fe6771
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786725"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="9965c-103">更新 shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="9965c-103">Update shiftPreferences</span></span>

<span data-ttu-id="9965c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9965c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9965c-105">更新 [shiftPreferences 对象的属性和](../resources/shiftpreferences.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="9965c-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9965c-106">权限</span><span class="sxs-lookup"><span data-stu-id="9965c-106">Permissions</span></span>

<span data-ttu-id="9965c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9965c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9965c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9965c-109">Permission type</span></span>      | <span data-ttu-id="9965c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9965c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9965c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9965c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9965c-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9965c-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="9965c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9965c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9965c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9965c-114">Not supported.</span></span>    |
|<span data-ttu-id="9965c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9965c-115">Application</span></span> | <span data-ttu-id="9965c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9965c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9965c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9965c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="9965c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9965c-118">Request headers</span></span>

| <span data-ttu-id="9965c-119">标头</span><span class="sxs-lookup"><span data-stu-id="9965c-119">Header</span></span>       | <span data-ttu-id="9965c-120">值</span><span class="sxs-lookup"><span data-stu-id="9965c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9965c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9965c-121">Authorization</span></span>  | <span data-ttu-id="9965c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9965c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9965c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9965c-124">Content-Type</span></span>  | <span data-ttu-id="9965c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9965c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9965c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9965c-127">Request body</span></span>
<span data-ttu-id="9965c-128">在请求正文中，提供 [shiftPreferences](../resources/shiftpreferences.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9965c-128">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9965c-129">响应</span><span class="sxs-lookup"><span data-stu-id="9965c-129">Response</span></span>

<span data-ttu-id="9965c-130">如果成功，此方法返回 `204 NO CONTENT` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="9965c-130">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9965c-131">示例</span><span class="sxs-lookup"><span data-stu-id="9965c-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9965c-132">请求</span><span class="sxs-lookup"><span data-stu-id="9965c-132">Request</span></span>

<span data-ttu-id="9965c-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9965c-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9965c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9965c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get-3"
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
# <a name="c"></a>[<span data-ttu-id="9965c-135">C#</span><span class="sxs-lookup"><span data-stu-id="9965c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9965c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9965c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9965c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9965c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9965c-138">Java</span><span class="sxs-lookup"><span data-stu-id="9965c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9965c-139">响应</span><span class="sxs-lookup"><span data-stu-id="9965c-139">Response</span></span>

<span data-ttu-id="9965c-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9965c-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
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


