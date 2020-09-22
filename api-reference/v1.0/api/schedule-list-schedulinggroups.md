---
title: 列出 schedulingGroups
description: 获取此计划中的 schedulingGroup 列表。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dba5ffe34a7c7e56ffe98dd1ab8207a8c39eedf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051282"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="5739d-103">列出 scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="5739d-103">List scheduleGroups</span></span>

<span data-ttu-id="5739d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5739d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5739d-105">获取此[计划](../resources/schedule.md)中的[schedulingGroups](../resources/schedulinggroup.md)列表。</span><span class="sxs-lookup"><span data-stu-id="5739d-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5739d-106">权限</span><span class="sxs-lookup"><span data-stu-id="5739d-106">Permissions</span></span>

<span data-ttu-id="5739d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5739d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5739d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5739d-109">Permission type</span></span>      | <span data-ttu-id="5739d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5739d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5739d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5739d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5739d-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="5739d-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5739d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5739d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5739d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5739d-114">Not supported.</span></span>    |
|<span data-ttu-id="5739d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5739d-115">Application</span></span> | <span data-ttu-id="5739d-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="5739d-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="5739d-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="5739d-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5739d-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="5739d-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5739d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5739d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="5739d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5739d-120">Request headers</span></span>

| <span data-ttu-id="5739d-121">标头</span><span class="sxs-lookup"><span data-stu-id="5739d-121">Header</span></span>       | <span data-ttu-id="5739d-122">值</span><span class="sxs-lookup"><span data-stu-id="5739d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5739d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5739d-123">Authorization</span></span>  | <span data-ttu-id="5739d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5739d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5739d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5739d-126">Request body</span></span>
<span data-ttu-id="5739d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5739d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5739d-128">响应</span><span class="sxs-lookup"><span data-stu-id="5739d-128">Response</span></span>

<span data-ttu-id="5739d-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [schedulingGroup](../resources/schedulinggroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5739d-129">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5739d-130">示例</span><span class="sxs-lookup"><span data-stu-id="5739d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5739d-131">请求</span><span class="sxs-lookup"><span data-stu-id="5739d-131">Request</span></span>

<span data-ttu-id="5739d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5739d-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5739d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5739d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups
```
# <a name="c"></a>[<span data-ttu-id="5739d-134">C#</span><span class="sxs-lookup"><span data-stu-id="5739d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5739d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5739d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5739d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5739d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5739d-137">Java</span><span class="sxs-lookup"><span data-stu-id="5739d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="5739d-138">响应</span><span class="sxs-lookup"><span data-stu-id="5739d-138">Response</span></span>

<span data-ttu-id="5739d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5739d-139">The following is an example of the response.</span></span> 

><span data-ttu-id="5739d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5739d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

