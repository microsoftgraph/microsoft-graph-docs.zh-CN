---
title: 获取 schedulingGroup
description: 按 ID 检索[schedulingGroup](../resources/schedulinggroup.md)的属性和关系。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 95e2e91161f2b32bf83c40a622c06fd1b70e2e88
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453791"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="f6026-103">获取 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="f6026-103">Get schedulingGroup</span></span>

<span data-ttu-id="f6026-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f6026-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6026-105">按 ID 检索[schedulingGroup](../resources/schedulinggroup.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f6026-105">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6026-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6026-106">Permissions</span></span>

<span data-ttu-id="f6026-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6026-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6026-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6026-109">Permission type</span></span>      | <span data-ttu-id="f6026-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6026-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6026-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6026-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6026-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6026-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6026-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6026-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6026-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6026-114">Not supported.</span></span>    |
|<span data-ttu-id="f6026-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6026-115">Application</span></span> | <span data-ttu-id="f6026-116">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="f6026-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="f6026-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="f6026-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="f6026-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="f6026-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f6026-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="f6026-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f6026-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6026-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="f6026-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6026-121">Request headers</span></span>

| <span data-ttu-id="f6026-122">标头</span><span class="sxs-lookup"><span data-stu-id="f6026-122">Header</span></span>       | <span data-ttu-id="f6026-123">值</span><span class="sxs-lookup"><span data-stu-id="f6026-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6026-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6026-124">Authorization</span></span>  | <span data-ttu-id="f6026-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6026-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6026-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6026-127">Request body</span></span>
<span data-ttu-id="f6026-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6026-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6026-129">响应</span><span class="sxs-lookup"><span data-stu-id="f6026-129">Response</span></span>

<span data-ttu-id="f6026-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[schedulingGroup](../resources/schedulinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f6026-130">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6026-131">示例</span><span class="sxs-lookup"><span data-stu-id="f6026-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f6026-132">请求</span><span class="sxs-lookup"><span data-stu-id="f6026-132">Request</span></span>

<span data-ttu-id="f6026-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f6026-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6026-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6026-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
# <a name="c"></a>[<span data-ttu-id="f6026-135">C#</span><span class="sxs-lookup"><span data-stu-id="f6026-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-get-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6026-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6026-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-get-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6026-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6026-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-get-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f6026-138">响应</span><span class="sxs-lookup"><span data-stu-id="f6026-138">Response</span></span>

<span data-ttu-id="f6026-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f6026-139">The following is an example of the response.</span></span> 

><span data-ttu-id="f6026-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f6026-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
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
  "description": "Get a schedulingGroup by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
