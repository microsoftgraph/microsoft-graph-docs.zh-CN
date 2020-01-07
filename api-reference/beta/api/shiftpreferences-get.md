---
title: 获取 shiftPreferences
description: 按 ID 获取 shift 首选项。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b0ef9a067cfb106c6cee5fadb113da5aabfa7f3a
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952116"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="e183b-103">获取 shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="e183b-103">Get shiftPreferences</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e183b-104">按 ID 检索[shiftPreferences](../resources/shiftpreferences.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e183b-104">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="e183b-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="e183b-105">Permissions</span></span>

<span data-ttu-id="e183b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e183b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e183b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e183b-108">Permission type</span></span>      | <span data-ttu-id="e183b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e183b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e183b-110">委托（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e183b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e183b-111">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e183b-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="e183b-112">委托（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e183b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e183b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e183b-113">Not supported.</span></span>    |
|<span data-ttu-id="e183b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e183b-114">Application</span></span> | <span data-ttu-id="e183b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e183b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e183b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e183b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="request-headers"></a><span data-ttu-id="e183b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e183b-117">Request headers</span></span>

| <span data-ttu-id="e183b-118">标头</span><span class="sxs-lookup"><span data-stu-id="e183b-118">Header</span></span>       | <span data-ttu-id="e183b-119">值</span><span class="sxs-lookup"><span data-stu-id="e183b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e183b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e183b-120">Authorization</span></span>  | <span data-ttu-id="e183b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e183b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e183b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e183b-123">Request body</span></span>
<span data-ttu-id="e183b-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e183b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e183b-125">响应</span><span class="sxs-lookup"><span data-stu-id="e183b-125">Response</span></span>

<span data-ttu-id="e183b-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[shiftPreferences](../resources/shiftpreferences.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e183b-126">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e183b-127">示例</span><span class="sxs-lookup"><span data-stu-id="e183b-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e183b-128">请求</span><span class="sxs-lookup"><span data-stu-id="e183b-128">Request</span></span>

<span data-ttu-id="e183b-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e183b-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e183b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e183b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences
```

#### <a name="response"></a><span data-ttu-id="e183b-131">响应</span><span class="sxs-lookup"><span data-stu-id="e183b-131">Response</span></span>

<span data-ttu-id="e183b-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e183b-132">The following is an example of the response.</span></span>

><span data-ttu-id="e183b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e183b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shiftPreferences"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "id": "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
    "@odata.etag": "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
    "availability": [
        {
            "recurrence": {
                "pattern": {
                    "type": "Weekly",
                    "daysOfWeek": ["Tuesday"],
                    "interval": 1
                },
                "range": {
                    "type": "noEnd"
                }
            },
            "timeZone": "Pacific Standard Time",
            "timeSlots": [
                {
                    "startTime": "09:15:00.000000",
                    "endTime": "12:30:00.000000"
                },
                {
                    "startTime": "16:00:00.000000",
                    "endTime": "20:00:00.000000"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-12-12 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a user's shift preferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
