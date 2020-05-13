---
title: 更换 schedulingGroup
description: 替换现有的 schedulingGroup。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b9bc875b3bd01cc2083f7726a1c0abb42c0bb316
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "42453771"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="18bc9-103">更换 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="18bc9-103">Replace schedulingGroup</span></span>

<span data-ttu-id="18bc9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18bc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18bc9-105">替换现有的[schedulingGroup](../resources/schedulinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="18bc9-105">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="18bc9-106">如果指定的[schedulingGroup](../resources/schedulinggroup.md)不存在，则此方法返回 `404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="18bc9-106">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="18bc9-107">权限</span><span class="sxs-lookup"><span data-stu-id="18bc9-107">Permissions</span></span>

<span data-ttu-id="18bc9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18bc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18bc9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="18bc9-110">Permission type</span></span>      | <span data-ttu-id="18bc9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18bc9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18bc9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18bc9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="18bc9-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18bc9-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="18bc9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18bc9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18bc9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="18bc9-115">Not supported.</span></span>    |
|<span data-ttu-id="18bc9-116">Application</span><span class="sxs-lookup"><span data-stu-id="18bc9-116">Application</span></span> | <span data-ttu-id="18bc9-117">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="18bc9-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="18bc9-118">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="18bc9-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="18bc9-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="18bc9-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="18bc9-120">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="18bc9-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="18bc9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18bc9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="18bc9-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="18bc9-122">Request headers</span></span>

| <span data-ttu-id="18bc9-123">标头</span><span class="sxs-lookup"><span data-stu-id="18bc9-123">Header</span></span>       | <span data-ttu-id="18bc9-124">值</span><span class="sxs-lookup"><span data-stu-id="18bc9-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18bc9-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="18bc9-125">Authorization</span></span>  | <span data-ttu-id="18bc9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18bc9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18bc9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18bc9-128">Content-Type</span></span>  | <span data-ttu-id="18bc9-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="18bc9-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18bc9-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="18bc9-131">Request body</span></span>

<span data-ttu-id="18bc9-132">在请求正文中，提供[schedulingGroup](../resources/schedulinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18bc9-132">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="18bc9-133">响应</span><span class="sxs-lookup"><span data-stu-id="18bc9-133">Response</span></span>

<span data-ttu-id="18bc9-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[schedulingGroup](../resources/schedulinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="18bc9-134">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18bc9-135">示例</span><span class="sxs-lookup"><span data-stu-id="18bc9-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="18bc9-136">请求</span><span class="sxs-lookup"><span data-stu-id="18bc9-136">Request</span></span>

<span data-ttu-id="18bc9-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="18bc9-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18bc9-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="18bc9-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-put-schedulinggroups"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="18bc9-139">C#</span><span class="sxs-lookup"><span data-stu-id="18bc9-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-put-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18bc9-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18bc9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-put-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18bc9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18bc9-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-put-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="18bc9-142">响应</span><span class="sxs-lookup"><span data-stu-id="18bc9-142">Response</span></span>

<span data-ttu-id="18bc9-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="18bc9-143">The following is an example of the response.</span></span> 

><span data-ttu-id="18bc9-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="18bc9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Replace an existing schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
