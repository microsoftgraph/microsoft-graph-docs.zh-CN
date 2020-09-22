---
title: 创建 schedulingGroup
description: 新建 schedulingGroup。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 518544215e141c46a6f99ebd84625404d4d61591
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051205"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="0cb95-103">创建 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="0cb95-103">Create schedulingGroup</span></span>

<span data-ttu-id="0cb95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cb95-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0cb95-105">新建 [schedulingGroup](../resources/schedulinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="0cb95-105">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0cb95-106">权限</span><span class="sxs-lookup"><span data-stu-id="0cb95-106">Permissions</span></span>

<span data-ttu-id="0cb95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cb95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cb95-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cb95-109">Permission type</span></span>      | <span data-ttu-id="0cb95-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0cb95-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cb95-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cb95-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0cb95-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="0cb95-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0cb95-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cb95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cb95-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cb95-114">Not supported.</span></span>    |
|<span data-ttu-id="0cb95-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cb95-115">Application</span></span> |<span data-ttu-id="0cb95-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cb95-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="0cb95-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0cb95-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0cb95-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="0cb95-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0cb95-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cb95-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="0cb95-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cb95-120">Request headers</span></span>

| <span data-ttu-id="0cb95-121">标头</span><span class="sxs-lookup"><span data-stu-id="0cb95-121">Header</span></span>       | <span data-ttu-id="0cb95-122">值</span><span class="sxs-lookup"><span data-stu-id="0cb95-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0cb95-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cb95-123">Authorization</span></span>  | <span data-ttu-id="0cb95-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0cb95-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0cb95-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0cb95-126">Content-Type</span></span>  | <span data-ttu-id="0cb95-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0cb95-p104">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="0cb95-129">响应</span><span class="sxs-lookup"><span data-stu-id="0cb95-129">Response</span></span>

<span data-ttu-id="0cb95-130">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [schedulingGroup](../resources/schedulinggroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0cb95-130">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cb95-131">示例</span><span class="sxs-lookup"><span data-stu-id="0cb95-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cb95-132">请求</span><span class="sxs-lookup"><span data-stu-id="0cb95-132">Request</span></span>

<span data-ttu-id="0cb95-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0cb95-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0cb95-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cb95-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups
Content-type: application/json

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="0cb95-135">C#</span><span class="sxs-lookup"><span data-stu-id="0cb95-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cb95-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cb95-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cb95-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cb95-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cb95-138">Java</span><span class="sxs-lookup"><span data-stu-id="0cb95-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="0cb95-139">响应</span><span class="sxs-lookup"><span data-stu-id="0cb95-139">Response</span></span>

<span data-ttu-id="0cb95-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0cb95-140">The following is an example of the response.</span></span> 

><span data-ttu-id="0cb95-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0cb95-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

