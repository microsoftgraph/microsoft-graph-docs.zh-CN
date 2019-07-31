---
title: 创建 schedulingGroup
description: 创建新的 schedulingGroup。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 36e3399a1de4a5792f205331f3aa408a871ca836
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982957"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="7c29c-103">创建 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="7c29c-103">Create schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c29c-104">创建新的[schedulingGroup](../resources/schedulinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="7c29c-104">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c29c-105">权限</span><span class="sxs-lookup"><span data-stu-id="7c29c-105">Permissions</span></span>

<span data-ttu-id="7c29c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c29c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c29c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c29c-108">Permission type</span></span>      | <span data-ttu-id="7c29c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c29c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c29c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c29c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7c29c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c29c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7c29c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c29c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c29c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c29c-113">Not supported.</span></span>    |
|<span data-ttu-id="7c29c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c29c-114">Application</span></span> | <span data-ttu-id="7c29c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c29c-115">Not supported.</span></span> |

> <span data-ttu-id="7c29c-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="7c29c-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7c29c-117">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="7c29c-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7c29c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c29c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="7c29c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c29c-119">Request headers</span></span>

| <span data-ttu-id="7c29c-120">标头</span><span class="sxs-lookup"><span data-stu-id="7c29c-120">Header</span></span>       | <span data-ttu-id="7c29c-121">值</span><span class="sxs-lookup"><span data-stu-id="7c29c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c29c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c29c-122">Authorization</span></span>  | <span data-ttu-id="7c29c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c29c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7c29c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c29c-125">Content-Type</span></span>  | <span data-ttu-id="7c29c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c29c-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="7c29c-127">响应</span><span class="sxs-lookup"><span data-stu-id="7c29c-127">Response</span></span>

<span data-ttu-id="7c29c-128">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[schedulingGroup](../resources/schedulinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7c29c-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c29c-129">示例</span><span class="sxs-lookup"><span data-stu-id="7c29c-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7c29c-130">请求</span><span class="sxs-lookup"><span data-stu-id="7c29c-130">Request</span></span>

<span data-ttu-id="7c29c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c29c-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7c29c-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7c29c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7c29c-133">C#</span><span class="sxs-lookup"><span data-stu-id="7c29c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c29c-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="7c29c-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7c29c-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="7c29c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7c29c-136">Java</span><span class="sxs-lookup"><span data-stu-id="7c29c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7c29c-137">响应</span><span class="sxs-lookup"><span data-stu-id="7c29c-137">Response</span></span>

<span data-ttu-id="7c29c-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7c29c-138">The following is an example of the response.</span></span> 

><span data-ttu-id="7c29c-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7c29c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
