---
title: 获取 shift
description: 按 ID 获取 shift。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1074150b77b8608a158a25db2224bd913f8cd157
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453301"
---
# <a name="get-shift"></a><span data-ttu-id="a685b-103">获取 shift</span><span class="sxs-lookup"><span data-stu-id="a685b-103">Get shift</span></span>

<span data-ttu-id="a685b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a685b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a685b-105">按 ID 检索[shift](../resources/shift.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a685b-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="a685b-106">权限</span><span class="sxs-lookup"><span data-stu-id="a685b-106">Permissions</span></span>

<span data-ttu-id="a685b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a685b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a685b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a685b-109">Permission type</span></span>      | <span data-ttu-id="a685b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a685b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a685b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a685b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a685b-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a685b-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a685b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a685b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a685b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a685b-114">Not supported.</span></span>    |<span data-ttu-id="a685b-115">s</span><span class="sxs-lookup"><span data-stu-id="a685b-115">s</span></span>
|<span data-ttu-id="a685b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a685b-116">Application</span></span> | <span data-ttu-id="a685b-117">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="a685b-117">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="a685b-118">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="a685b-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="a685b-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a685b-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a685b-120">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="a685b-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a685b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a685b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="a685b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a685b-122">Request headers</span></span>

| <span data-ttu-id="a685b-123">标头</span><span class="sxs-lookup"><span data-stu-id="a685b-123">Header</span></span>       | <span data-ttu-id="a685b-124">值</span><span class="sxs-lookup"><span data-stu-id="a685b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a685b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a685b-125">Authorization</span></span>  | <span data-ttu-id="a685b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a685b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a685b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a685b-128">Request body</span></span>
<span data-ttu-id="a685b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a685b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a685b-130">响应</span><span class="sxs-lookup"><span data-stu-id="a685b-130">Response</span></span>

<span data-ttu-id="a685b-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[shift](../resources/shift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a685b-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a685b-132">示例</span><span class="sxs-lookup"><span data-stu-id="a685b-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a685b-133">请求</span><span class="sxs-lookup"><span data-stu-id="a685b-133">Request</span></span>

<span data-ttu-id="a685b-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a685b-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a685b-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a685b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="a685b-136">C#</span><span class="sxs-lookup"><span data-stu-id="a685b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a685b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a685b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a685b-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a685b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a685b-139">响应</span><span class="sxs-lookup"><span data-stu-id="a685b-139">Response</span></span>

<span data-ttu-id="a685b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a685b-140">The following is an example of the response.</span></span> 

><span data-ttu-id="a685b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a685b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "id": "SHFT_ca485cdd-a42c-4b93-9e6a-6fa54fd45fe1",
    "createdDateTime": "2019-06-06T20:15:38.9Z",
    "lastModifiedDateTime": "2019-11-18T01:12:08.318Z",
    "schedulingGroupId": "TAG_d18fd675-3ac8-41b2-8038-d17fdac8b0d3",
    "userId": "a7b0c8c4-3f5c-492f-ab13-40f0e0f0ffa8",
    "draftShift": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "1c717a55-febd-4850-b5f6-101f3a29972c",
            "displayName": "Sumanth Lingom"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a shift by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
