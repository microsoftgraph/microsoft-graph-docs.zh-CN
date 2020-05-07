---
title: 更新 shiftPreferences
description: 更新用户的 shift 首选项。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 51ebeecb555c426c124975682fb85f77988d6e99
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154485"
---
# <a name="update-shiftpreferences"></a><span data-ttu-id="74e88-103">更新 shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="74e88-103">Update shiftPreferences</span></span>

<span data-ttu-id="74e88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74e88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74e88-105">更新[shiftPreferences](../resources/shiftpreferences.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74e88-105">Update the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="74e88-106">权限</span><span class="sxs-lookup"><span data-stu-id="74e88-106">Permissions</span></span>

<span data-ttu-id="74e88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74e88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74e88-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="74e88-109">Permission type</span></span>      | <span data-ttu-id="74e88-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74e88-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74e88-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74e88-111">Delegated (work or school account)</span></span> | <span data-ttu-id="74e88-112">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74e88-112">User.ReadWrite.All</span></span>    |
|<span data-ttu-id="74e88-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74e88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74e88-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="74e88-114">Not supported.</span></span>    |
|<span data-ttu-id="74e88-115">Application</span><span class="sxs-lookup"><span data-stu-id="74e88-115">Application</span></span> | <span data-ttu-id="74e88-116">UserShiftPreferences</span><span class="sxs-lookup"><span data-stu-id="74e88-116">UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="74e88-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="74e88-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="74e88-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="74e88-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="74e88-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74e88-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="74e88-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="74e88-120">Request headers</span></span>

| <span data-ttu-id="74e88-121">标头</span><span class="sxs-lookup"><span data-stu-id="74e88-121">Header</span></span>       | <span data-ttu-id="74e88-122">值</span><span class="sxs-lookup"><span data-stu-id="74e88-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74e88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74e88-123">Authorization</span></span>  | <span data-ttu-id="74e88-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74e88-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="74e88-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74e88-126">Content-Type</span></span>  | <span data-ttu-id="74e88-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="74e88-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74e88-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="74e88-129">Request body</span></span>
<span data-ttu-id="74e88-130">在请求正文中，提供[shiftPreferences](../resources/shiftpreferences.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74e88-130">In the request body, supply a JSON representation of a [shiftPreferences](../resources/shiftpreferences.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="74e88-131">响应</span><span class="sxs-lookup"><span data-stu-id="74e88-131">Response</span></span>

<span data-ttu-id="74e88-132">如果成功，此方法返回 `204 NO CONTENT` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="74e88-132">If successful, this method returns a `204 NO CONTENT` response code.</span></span>

## <a name="example"></a><span data-ttu-id="74e88-133">示例</span><span class="sxs-lookup"><span data-stu-id="74e88-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="74e88-134">请求</span><span class="sxs-lookup"><span data-stu-id="74e88-134">Request</span></span>

<span data-ttu-id="74e88-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="74e88-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
PUT https://graph.microsoft.com/v1.0/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences
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
---


### <a name="response"></a><span data-ttu-id="74e88-136">响应</span><span class="sxs-lookup"><span data-stu-id="74e88-136">Response</span></span>

<span data-ttu-id="74e88-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="74e88-137">The following is an example of the response.</span></span>

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
