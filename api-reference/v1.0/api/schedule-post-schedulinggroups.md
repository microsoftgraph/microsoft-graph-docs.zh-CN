---
title: 创建 schedulingGroup
description: 新建 schedulingGroup。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 71f446eab31dc3fdfcc2dfd4f025c35f9cc9239b
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312762"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="e3e88-103">创建 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="e3e88-103">Create schedulingGroup</span></span>

<span data-ttu-id="e3e88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3e88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3e88-105">新建 [schedulingGroup](../resources/schedulinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="e3e88-105">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e3e88-106">权限</span><span class="sxs-lookup"><span data-stu-id="e3e88-106">Permissions</span></span>

<span data-ttu-id="e3e88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3e88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3e88-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3e88-109">Permission type</span></span>      | <span data-ttu-id="e3e88-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3e88-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3e88-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3e88-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e3e88-112">Schedule。 All，Group. 所有</span><span class="sxs-lookup"><span data-stu-id="e3e88-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3e88-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3e88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3e88-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3e88-114">Not supported.</span></span>    |
|<span data-ttu-id="e3e88-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3e88-115">Application</span></span> |<span data-ttu-id="e3e88-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3e88-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3e88-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3e88-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="e3e88-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3e88-118">Request headers</span></span>

| <span data-ttu-id="e3e88-119">标头</span><span class="sxs-lookup"><span data-stu-id="e3e88-119">Header</span></span>       | <span data-ttu-id="e3e88-120">值</span><span class="sxs-lookup"><span data-stu-id="e3e88-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3e88-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3e88-121">Authorization</span></span>  | <span data-ttu-id="e3e88-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3e88-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e3e88-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3e88-124">Content-Type</span></span>  | <span data-ttu-id="e3e88-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e3e88-p103">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="e3e88-127">响应</span><span class="sxs-lookup"><span data-stu-id="e3e88-127">Response</span></span>

<span data-ttu-id="e3e88-128">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [schedulingGroup](../resources/schedulinggroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e3e88-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3e88-129">示例</span><span class="sxs-lookup"><span data-stu-id="e3e88-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3e88-130">请求</span><span class="sxs-lookup"><span data-stu-id="e3e88-130">Request</span></span>

<span data-ttu-id="e3e88-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e3e88-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e3e88-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3e88-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e3e88-133">C#</span><span class="sxs-lookup"><span data-stu-id="e3e88-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3e88-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3e88-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3e88-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3e88-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3e88-136">Java</span><span class="sxs-lookup"><span data-stu-id="e3e88-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="e3e88-137">响应</span><span class="sxs-lookup"><span data-stu-id="e3e88-137">Response</span></span>

<span data-ttu-id="e3e88-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e3e88-138">The following is an example of the response.</span></span> 

><span data-ttu-id="e3e88-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e3e88-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

