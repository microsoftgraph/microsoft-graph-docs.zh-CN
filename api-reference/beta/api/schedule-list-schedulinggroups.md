---
title: 列出 schedulingGroups
description: 获取此计划中的 schedulingGroup 列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 995c27fadaee51b423b171a5c60417d0e89239db
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "42453844"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="22023-103">列出 scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="22023-103">List scheduleGroups</span></span>

<span data-ttu-id="22023-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22023-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22023-105">获取此[计划](../resources/schedule.md)中的[schedulingGroups](../resources/schedulinggroup.md)列表。</span><span class="sxs-lookup"><span data-stu-id="22023-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="22023-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="22023-106">Permissions</span></span>

<span data-ttu-id="22023-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22023-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22023-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="22023-109">Permission type</span></span>      | <span data-ttu-id="22023-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22023-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22023-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22023-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22023-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22023-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="22023-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22023-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22023-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="22023-114">Not supported.</span></span>    |
|<span data-ttu-id="22023-115">Application</span><span class="sxs-lookup"><span data-stu-id="22023-115">Application</span></span> | <span data-ttu-id="22023-116">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="22023-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="22023-117">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="22023-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="22023-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="22023-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="22023-119">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="22023-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="22023-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22023-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="22023-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="22023-121">Request headers</span></span>

| <span data-ttu-id="22023-122">标头</span><span class="sxs-lookup"><span data-stu-id="22023-122">Header</span></span>       | <span data-ttu-id="22023-123">值</span><span class="sxs-lookup"><span data-stu-id="22023-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="22023-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="22023-124">Authorization</span></span>  | <span data-ttu-id="22023-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="22023-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="22023-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="22023-127">Request body</span></span>
<span data-ttu-id="22023-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22023-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22023-129">响应</span><span class="sxs-lookup"><span data-stu-id="22023-129">Response</span></span>

<span data-ttu-id="22023-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[schedulingGroup](../resources/schedulinggroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="22023-130">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22023-131">示例</span><span class="sxs-lookup"><span data-stu-id="22023-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="22023-132">请求</span><span class="sxs-lookup"><span data-stu-id="22023-132">Request</span></span>

<span data-ttu-id="22023-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="22023-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22023-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="22023-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
```
# <a name="c"></a>[<span data-ttu-id="22023-135">C#</span><span class="sxs-lookup"><span data-stu-id="22023-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22023-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22023-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22023-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22023-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22023-138">响应</span><span class="sxs-lookup"><span data-stu-id="22023-138">Response</span></span>

<span data-ttu-id="22023-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="22023-139">The following is an example of the response.</span></span> 

><span data-ttu-id="22023-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="22023-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
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
        "@odata.type":"microsoft.graph.identitySet",
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of schedulingGroup in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
