---
title: 获取 shiftPreferences
description: 按 ID 获取 shift 首选项。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9bbf5be71676b942a3df0174f781a0a6708493e2
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154330"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="a5e3d-103">获取 shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="a5e3d-103">Get shiftPreferences</span></span>

<span data-ttu-id="a5e3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5e3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5e3d-105">按 ID 检索[shiftPreferences](../resources/shiftpreferences.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-105">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5e3d-106">权限</span><span class="sxs-lookup"><span data-stu-id="a5e3d-106">Permissions</span></span>

<span data-ttu-id="a5e3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5e3d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5e3d-109">Permission type</span></span>      | <span data-ttu-id="a5e3d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5e3d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5e3d-111">委托（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5e3d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a5e3d-112">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5e3d-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5e3d-113">委托（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5e3d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5e3d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-114">Not supported.</span></span>    |
|<span data-ttu-id="a5e3d-115">Application</span><span class="sxs-lookup"><span data-stu-id="a5e3d-115">Application</span></span> | <span data-ttu-id="a5e3d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5e3d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5e3d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5e3d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a5e3d-118">Optional query parameters</span></span>

<span data-ttu-id="a5e3d-119">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-119">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5e3d-120">请求头</span><span class="sxs-lookup"><span data-stu-id="a5e3d-120">Request headers</span></span>

| <span data-ttu-id="a5e3d-121">标头</span><span class="sxs-lookup"><span data-stu-id="a5e3d-121">Header</span></span>       | <span data-ttu-id="a5e3d-122">值</span><span class="sxs-lookup"><span data-stu-id="a5e3d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5e3d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5e3d-123">Authorization</span></span>  | <span data-ttu-id="a5e3d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5e3d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5e3d-126">Request body</span></span>
<span data-ttu-id="a5e3d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5e3d-128">响应</span><span class="sxs-lookup"><span data-stu-id="a5e3d-128">Response</span></span>

<span data-ttu-id="a5e3d-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[shiftPreferences](../resources/shiftpreferences.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-129">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5e3d-130">示例</span><span class="sxs-lookup"><span data-stu-id="a5e3d-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a5e3d-131">请求</span><span class="sxs-lookup"><span data-stu-id="a5e3d-131">Request</span></span>

<span data-ttu-id="a5e3d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5e3d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5e3d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences
```
# <a name="c"></a>[<span data-ttu-id="a5e3d-134">C#</span><span class="sxs-lookup"><span data-stu-id="a5e3d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5e3d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5e3d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5e3d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5e3d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a5e3d-137">响应</span><span class="sxs-lookup"><span data-stu-id="a5e3d-137">Response</span></span>

<span data-ttu-id="a5e3d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-138">The following is an example of the response.</span></span>

><span data-ttu-id="a5e3d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a5e3d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
