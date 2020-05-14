---
title: 获取 shiftPreferences
description: 按 ID 获取 shift 首选项。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a83331992092cec3204b0279944a13c17870c295
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217359"
---
# <a name="get-shiftpreferences"></a><span data-ttu-id="ba5a3-103">获取 shiftPreferences</span><span class="sxs-lookup"><span data-stu-id="ba5a3-103">Get shiftPreferences</span></span>

<span data-ttu-id="ba5a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba5a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ba5a3-105">按 ID 检索[shiftPreferences](../resources/shiftpreferences.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-105">Retrieve the properties and relationships of a [shiftPreferences](../resources/shiftpreferences.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba5a3-106">权限</span><span class="sxs-lookup"><span data-stu-id="ba5a3-106">Permissions</span></span>

<span data-ttu-id="ba5a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba5a3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba5a3-109">Permission type</span></span>      | <span data-ttu-id="ba5a3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba5a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba5a3-111">委托（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba5a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ba5a3-112">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba5a3-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba5a3-113">委托（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba5a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba5a3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-114">Not supported.</span></span>    |
|<span data-ttu-id="ba5a3-115">Application</span><span class="sxs-lookup"><span data-stu-id="ba5a3-115">Application</span></span> | <span data-ttu-id="ba5a3-116">UserShiftPreferences、UserShiftPreferences 和所有</span><span class="sxs-lookup"><span data-stu-id="ba5a3-116">UserShiftPreferences.Read.All, UserShiftPreferences.ReadWrite.All</span></span> |

> <span data-ttu-id="ba5a3-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ba5a3-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ba5a3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba5a3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{userId}/settings/shiftPreferences
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba5a3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ba5a3-120">Optional query parameters</span></span>

<span data-ttu-id="ba5a3-121">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-121">This method does not support OData query parameters to customize the response.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ba5a3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba5a3-122">Request headers</span></span>

| <span data-ttu-id="ba5a3-123">标头</span><span class="sxs-lookup"><span data-stu-id="ba5a3-123">Header</span></span>       | <span data-ttu-id="ba5a3-124">值</span><span class="sxs-lookup"><span data-stu-id="ba5a3-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba5a3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba5a3-125">Authorization</span></span>  | <span data-ttu-id="ba5a3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba5a3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba5a3-128">Request body</span></span>
<span data-ttu-id="ba5a3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba5a3-130">响应</span><span class="sxs-lookup"><span data-stu-id="ba5a3-130">Response</span></span>

<span data-ttu-id="ba5a3-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[shiftPreferences](../resources/shiftpreferences.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-131">If successful, this method returns a `200 OK` response code and a [shiftPreferences](../resources/shiftpreferences.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba5a3-132">示例</span><span class="sxs-lookup"><span data-stu-id="ba5a3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba5a3-133">请求</span><span class="sxs-lookup"><span data-stu-id="ba5a3-133">Request</span></span>

<span data-ttu-id="ba5a3-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba5a3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba5a3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/871dbd5c-3a6a-4392-bfe1-042452793a50/shiftPreferences
```
# <a name="c"></a>[<span data-ttu-id="ba5a3-136">C#</span><span class="sxs-lookup"><span data-stu-id="ba5a3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba5a3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba5a3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba5a3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba5a3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ba5a3-139">Java</span><span class="sxs-lookup"><span data-stu-id="ba5a3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="ba5a3-140">响应</span><span class="sxs-lookup"><span data-stu-id="ba5a3-140">Response</span></span>

<span data-ttu-id="ba5a3-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-141">The following is an example of the response.</span></span>

><span data-ttu-id="ba5a3-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba5a3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
