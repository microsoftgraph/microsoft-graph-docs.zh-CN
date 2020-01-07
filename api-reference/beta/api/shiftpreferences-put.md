---
title: 更新 shiftPreferences
description: 更新用户的 shift 首选项。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 83bec268e918bc65f1ce139081ff88c0290acf4d
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952081"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="31d9f-103">更新 shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="31d9f-103">Update shiftPreferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31d9f-104">更新[shiftPreferences](../resources/shiftpreferences.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="31d9f-104">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31d9f-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="31d9f-105">Permissions</span></span>

<span data-ttu-id="31d9f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31d9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31d9f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="31d9f-108">Permission type</span></span>      | <span data-ttu-id="31d9f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31d9f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31d9f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31d9f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="31d9f-111">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31d9f-111">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="31d9f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31d9f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31d9f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="31d9f-113">Not supported.</span></span>    |
|<span data-ttu-id="31d9f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="31d9f-114">Application</span></span> | <span data-ttu-id="31d9f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="31d9f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31d9f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31d9f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="31d9f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="31d9f-117">Request headers</span></span>

| <span data-ttu-id="31d9f-118">标头</span><span class="sxs-lookup"><span data-stu-id="31d9f-118">Header</span></span>       | <span data-ttu-id="31d9f-119">值</span><span class="sxs-lookup"><span data-stu-id="31d9f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31d9f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="31d9f-120">Authorization</span></span>  | <span data-ttu-id="31d9f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31d9f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="31d9f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31d9f-123">Content-Type</span></span>  | <span data-ttu-id="31d9f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="31d9f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31d9f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="31d9f-126">Request body</span></span>
<span data-ttu-id="31d9f-127">在此方法的请求正文中提供新的[shiftPreferences](../resources/shiftpreferences.md)对象。</span><span class="sxs-lookup"><span data-stu-id="31d9f-127">Provide the new [shiftPreferences](../resources/shiftpreferences.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31d9f-128">响应</span><span class="sxs-lookup"><span data-stu-id="31d9f-128">Response</span></span>

<span data-ttu-id="31d9f-129">如果成功，此方法返回 `204 NO CONTENT` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="31d9f-129">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="31d9f-130">示例</span><span class="sxs-lookup"><span data-stu-id="31d9f-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="31d9f-131">请求</span><span class="sxs-lookup"><span data-stu-id="31d9f-131">Request</span></span>

<span data-ttu-id="31d9f-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="31d9f-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="31d9f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="31d9f-133">HTTP</span></span>](#tab/http)
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

#### <a name="response"></a><span data-ttu-id="31d9f-134">响应</span><span class="sxs-lookup"><span data-stu-id="31d9f-134">Response</span></span>

<span data-ttu-id="31d9f-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="31d9f-135">The following is an example of the response.</span></span>

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
