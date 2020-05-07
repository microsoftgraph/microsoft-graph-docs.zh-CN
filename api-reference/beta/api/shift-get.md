---
title: 获取 shift
description: 按 ID 获取 shift。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7059b58689173e5e47fc96ad32babbb85dc0b046
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154211"
---
# <a name="get-shift"></a><span data-ttu-id="b26e2-103">获取 shift</span><span class="sxs-lookup"><span data-stu-id="b26e2-103">Get shift</span></span>

<span data-ttu-id="b26e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b26e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b26e2-105">按 ID 检索[shift](../resources/shift.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b26e2-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="b26e2-106">权限</span><span class="sxs-lookup"><span data-stu-id="b26e2-106">Permissions</span></span>

<span data-ttu-id="b26e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b26e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b26e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b26e2-109">Permission type</span></span>      | <span data-ttu-id="b26e2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b26e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b26e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b26e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b26e2-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b26e2-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b26e2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b26e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b26e2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b26e2-114">Not supported.</span></span>    |<span data-ttu-id="b26e2-115">s</span><span class="sxs-lookup"><span data-stu-id="b26e2-115">s</span></span>
|<span data-ttu-id="b26e2-116">Application</span><span class="sxs-lookup"><span data-stu-id="b26e2-116">Application</span></span> | <span data-ttu-id="b26e2-117">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="b26e2-117">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="b26e2-118">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="b26e2-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="b26e2-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="b26e2-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b26e2-120">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="b26e2-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b26e2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b26e2-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b26e2-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b26e2-122">Optional query parameters</span></span>

<span data-ttu-id="b26e2-123">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b26e2-123">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b26e2-124">请求头</span><span class="sxs-lookup"><span data-stu-id="b26e2-124">Request headers</span></span>

| <span data-ttu-id="b26e2-125">标头</span><span class="sxs-lookup"><span data-stu-id="b26e2-125">Header</span></span>       | <span data-ttu-id="b26e2-126">值</span><span class="sxs-lookup"><span data-stu-id="b26e2-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b26e2-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b26e2-127">Authorization</span></span>  | <span data-ttu-id="b26e2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b26e2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b26e2-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b26e2-130">Request body</span></span>
<span data-ttu-id="b26e2-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b26e2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b26e2-132">响应</span><span class="sxs-lookup"><span data-stu-id="b26e2-132">Response</span></span>

<span data-ttu-id="b26e2-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和[shift](../resources/shift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b26e2-133">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b26e2-134">示例</span><span class="sxs-lookup"><span data-stu-id="b26e2-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b26e2-135">请求</span><span class="sxs-lookup"><span data-stu-id="b26e2-135">Request</span></span>

<span data-ttu-id="b26e2-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b26e2-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b26e2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b26e2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="b26e2-138">C#</span><span class="sxs-lookup"><span data-stu-id="b26e2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b26e2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b26e2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b26e2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b26e2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b26e2-141">响应</span><span class="sxs-lookup"><span data-stu-id="b26e2-141">Response</span></span>

<span data-ttu-id="b26e2-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b26e2-142">The following is an example of the response.</span></span> 

><span data-ttu-id="b26e2-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b26e2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
