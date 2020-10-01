---
title: 列出 schedulingGroups
description: 获取此计划中的 schedulingGroup 列表。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7628c20df5e72e5c780361e3c858648b586d7c8d
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315089"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="1ec64-103">列出 scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="1ec64-103">List scheduleGroups</span></span>

<span data-ttu-id="1ec64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ec64-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1ec64-105">获取此[计划](../resources/schedule.md)中的[schedulingGroups](../resources/schedulinggroup.md)列表。</span><span class="sxs-lookup"><span data-stu-id="1ec64-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1ec64-106">权限</span><span class="sxs-lookup"><span data-stu-id="1ec64-106">Permissions</span></span>

<span data-ttu-id="1ec64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ec64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ec64-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ec64-109">Permission type</span></span>      | <span data-ttu-id="1ec64-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ec64-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ec64-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ec64-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1ec64-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="1ec64-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ec64-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ec64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ec64-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ec64-114">Not supported.</span></span>    |
|<span data-ttu-id="1ec64-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ec64-115">Application</span></span> | <span data-ttu-id="1ec64-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="1ec64-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ec64-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ec64-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="1ec64-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ec64-118">Request headers</span></span>

| <span data-ttu-id="1ec64-119">标头</span><span class="sxs-lookup"><span data-stu-id="1ec64-119">Header</span></span>       | <span data-ttu-id="1ec64-120">值</span><span class="sxs-lookup"><span data-stu-id="1ec64-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ec64-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ec64-121">Authorization</span></span>  | <span data-ttu-id="1ec64-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ec64-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ec64-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ec64-124">Request body</span></span>
<span data-ttu-id="1ec64-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ec64-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ec64-126">响应</span><span class="sxs-lookup"><span data-stu-id="1ec64-126">Response</span></span>

<span data-ttu-id="1ec64-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [schedulingGroup](../resources/schedulinggroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1ec64-127">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ec64-128">示例</span><span class="sxs-lookup"><span data-stu-id="1ec64-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ec64-129">请求</span><span class="sxs-lookup"><span data-stu-id="1ec64-129">Request</span></span>

<span data-ttu-id="1ec64-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ec64-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1ec64-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ec64-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups
```
# <a name="c"></a>[<span data-ttu-id="1ec64-132">C#</span><span class="sxs-lookup"><span data-stu-id="1ec64-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ec64-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ec64-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ec64-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ec64-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ec64-135">Java</span><span class="sxs-lookup"><span data-stu-id="1ec64-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="1ec64-136">响应</span><span class="sxs-lookup"><span data-stu-id="1ec64-136">Response</span></span>

<span data-ttu-id="1ec64-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ec64-137">The following is an example of the response.</span></span> 

><span data-ttu-id="1ec64-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1ec64-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

