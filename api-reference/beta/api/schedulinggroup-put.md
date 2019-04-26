---
title: 更换 schedulingGroup
description: 替换现有的 schedulingGroup。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 90f28648bffb9f57e10ba2a5c3c52c871c9251af
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331396"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="83156-103">更换 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="83156-103">Replace schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83156-104">替换现有的[schedulingGroup](../resources/schedulinggroup.md)。</span><span class="sxs-lookup"><span data-stu-id="83156-104">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="83156-105">如果指定的[schedulingGroup](../resources/schedulinggroup.md)不存在, 则此方法`404 Not found`返回。</span><span class="sxs-lookup"><span data-stu-id="83156-105">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="83156-106">权限</span><span class="sxs-lookup"><span data-stu-id="83156-106">Permissions</span></span>

<span data-ttu-id="83156-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83156-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="83156-109">Permission type</span></span>      | <span data-ttu-id="83156-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83156-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="83156-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83156-111">Delegated (work or school account)</span></span> | <span data-ttu-id="83156-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83156-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="83156-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83156-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83156-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="83156-114">Not supported.</span></span>    |
|<span data-ttu-id="83156-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="83156-115">Application</span></span> | <span data-ttu-id="83156-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83156-116">Not supported.</span></span> |

> <span data-ttu-id="83156-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="83156-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="83156-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="83156-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="83156-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83156-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="83156-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="83156-120">Request headers</span></span>

| <span data-ttu-id="83156-121">标头</span><span class="sxs-lookup"><span data-stu-id="83156-121">Header</span></span>       | <span data-ttu-id="83156-122">值</span><span class="sxs-lookup"><span data-stu-id="83156-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83156-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83156-123">Authorization</span></span>  | <span data-ttu-id="83156-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="83156-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="83156-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="83156-126">Content-Type</span></span>  | <span data-ttu-id="83156-127">application/json</span><span class="sxs-lookup"><span data-stu-id="83156-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83156-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="83156-128">Request body</span></span>

<span data-ttu-id="83156-129">在请求正文中, 提供[schedulingGroup](../resources/schedulinggroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83156-129">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="83156-130">响应</span><span class="sxs-lookup"><span data-stu-id="83156-130">Response</span></span>

<span data-ttu-id="83156-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[schedulingGroup](../resources/schedulinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="83156-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83156-132">示例</span><span class="sxs-lookup"><span data-stu-id="83156-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="83156-133">请求</span><span class="sxs-lookup"><span data-stu-id="83156-133">Request</span></span>

<span data-ttu-id="83156-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="83156-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="83156-135">响应</span><span class="sxs-lookup"><span data-stu-id="83156-135">Response</span></span>

<span data-ttu-id="83156-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="83156-136">The following is an example of the response.</span></span> 

><span data-ttu-id="83156-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="83156-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
