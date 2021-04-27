---
title: 更换 schedulingGroup
description: 替换现有的 schedulingGroup。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 776dd553c6573455e5577156a52e9b5d69a7add8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051996"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="b9cdd-103">更换 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="b9cdd-103">Replace schedulingGroup</span></span>

<span data-ttu-id="b9cdd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9cdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9cdd-105">替换现有的 [schedulingGroup](../resources/schedulinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-105">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="b9cdd-106">如果指定的 [schedulingGroup](../resources/schedulinggroup.md) 不存在，此方法将返回 `404 Not found` 。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-106">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9cdd-107">权限</span><span class="sxs-lookup"><span data-stu-id="b9cdd-107">Permissions</span></span>

<span data-ttu-id="b9cdd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9cdd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9cdd-110">Permission type</span></span>      | <span data-ttu-id="b9cdd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9cdd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9cdd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9cdd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b9cdd-113">Schedule.ReadWrite.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9cdd-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9cdd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9cdd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9cdd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-115">Not supported.</span></span>    |
|<span data-ttu-id="b9cdd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9cdd-116">Application</span></span> | <span data-ttu-id="b9cdd-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9cdd-117">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9cdd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9cdd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="b9cdd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9cdd-119">Request headers</span></span>

| <span data-ttu-id="b9cdd-120">标头</span><span class="sxs-lookup"><span data-stu-id="b9cdd-120">Header</span></span>       | <span data-ttu-id="b9cdd-121">值</span><span class="sxs-lookup"><span data-stu-id="b9cdd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9cdd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9cdd-122">Authorization</span></span>  | <span data-ttu-id="b9cdd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b9cdd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9cdd-125">Content-Type</span></span>  | <span data-ttu-id="b9cdd-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b9cdd-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9cdd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9cdd-128">Request body</span></span>

<span data-ttu-id="b9cdd-129">在请求正文中，提供 [schedulingGroup](../resources/schedulinggroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-129">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b9cdd-130">响应</span><span class="sxs-lookup"><span data-stu-id="b9cdd-130">Response</span></span>

<span data-ttu-id="b9cdd-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [schedulingGroup](../resources/schedulinggroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9cdd-132">示例</span><span class="sxs-lookup"><span data-stu-id="b9cdd-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b9cdd-133">请求</span><span class="sxs-lookup"><span data-stu-id="b9cdd-133">Request</span></span>

<span data-ttu-id="b9cdd-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9cdd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9cdd-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b9cdd-136">C#</span><span class="sxs-lookup"><span data-stu-id="b9cdd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-put-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9cdd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9cdd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-put-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9cdd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9cdd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-put-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9cdd-139">Java</span><span class="sxs-lookup"><span data-stu-id="b9cdd-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-put-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b9cdd-140">响应</span><span class="sxs-lookup"><span data-stu-id="b9cdd-140">Response</span></span>

<span data-ttu-id="b9cdd-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-141">The following is an example of the response.</span></span> 

><span data-ttu-id="b9cdd-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b9cdd-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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


