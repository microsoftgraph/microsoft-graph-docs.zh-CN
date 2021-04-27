---
title: 列出 schedulingGroups
description: 获取此计划中的 schedulingGroup 列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e4d45bb7b3948a6e8626299fd35adc1308a33a6c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053508"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="9c299-103">列出 scheduleGroups</span><span class="sxs-lookup"><span data-stu-id="9c299-103">List scheduleGroups</span></span>

<span data-ttu-id="9c299-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c299-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c299-105">获取此 [计划中的 schedulingGroups](../resources/schedulinggroup.md) [列表](../resources/schedule.md)。</span><span class="sxs-lookup"><span data-stu-id="9c299-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c299-106">权限</span><span class="sxs-lookup"><span data-stu-id="9c299-106">Permissions</span></span>

<span data-ttu-id="9c299-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c299-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c299-109">Permission type</span></span>      | <span data-ttu-id="9c299-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9c299-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c299-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c299-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9c299-112">Schedule.Read.All、Group.Read.All、Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c299-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c299-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c299-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c299-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c299-114">Not supported.</span></span>    |
|<span data-ttu-id="9c299-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c299-115">Application</span></span> | <span data-ttu-id="9c299-116">Schedule.Read.All、Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c299-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c299-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c299-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="9c299-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c299-118">Request headers</span></span>

| <span data-ttu-id="9c299-119">标头</span><span class="sxs-lookup"><span data-stu-id="9c299-119">Header</span></span>       | <span data-ttu-id="9c299-120">值</span><span class="sxs-lookup"><span data-stu-id="9c299-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c299-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c299-121">Authorization</span></span>  | <span data-ttu-id="9c299-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9c299-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c299-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c299-124">Request body</span></span>
<span data-ttu-id="9c299-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c299-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c299-126">响应</span><span class="sxs-lookup"><span data-stu-id="9c299-126">Response</span></span>

<span data-ttu-id="9c299-127">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [schedulingGroup](../resources/schedulinggroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9c299-127">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c299-128">示例</span><span class="sxs-lookup"><span data-stu-id="9c299-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9c299-129">请求</span><span class="sxs-lookup"><span data-stu-id="9c299-129">Request</span></span>

<span data-ttu-id="9c299-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9c299-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c299-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c299-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
```
# <a name="c"></a>[<span data-ttu-id="9c299-132">C#</span><span class="sxs-lookup"><span data-stu-id="9c299-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c299-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c299-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c299-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c299-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c299-135">Java</span><span class="sxs-lookup"><span data-stu-id="9c299-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9c299-136">响应</span><span class="sxs-lookup"><span data-stu-id="9c299-136">Response</span></span>

<span data-ttu-id="9c299-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9c299-137">The following is an example of the response.</span></span> 

><span data-ttu-id="9c299-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9c299-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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


