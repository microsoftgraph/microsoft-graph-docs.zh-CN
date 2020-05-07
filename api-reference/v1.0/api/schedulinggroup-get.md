---
title: 获取 schedulingGroup
description: 按 ID 检索[schedulingGroup](../resources/schedulinggroup.md)的属性和关系。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f58d41c588c9937645480d3d0f5075c9753fda17
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154190"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="0008d-103">获取 schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="0008d-103">Get schedulingGroup</span></span>

<span data-ttu-id="0008d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0008d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0008d-105">按 ID 检索[schedulingGroup](../resources/schedulinggroup.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0008d-105">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="0008d-106">权限</span><span class="sxs-lookup"><span data-stu-id="0008d-106">Permissions</span></span>

<span data-ttu-id="0008d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0008d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0008d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0008d-109">Permission type</span></span>      | <span data-ttu-id="0008d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0008d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0008d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0008d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0008d-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="0008d-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0008d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0008d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0008d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0008d-114">Not supported.</span></span>    |
|<span data-ttu-id="0008d-115">Application</span><span class="sxs-lookup"><span data-stu-id="0008d-115">Application</span></span> | <span data-ttu-id="0008d-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="0008d-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |


> <span data-ttu-id="0008d-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="0008d-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="0008d-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="0008d-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="0008d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0008d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0008d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0008d-120">Optional query parameters</span></span>

<span data-ttu-id="0008d-121">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0008d-121">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0008d-122">请求头</span><span class="sxs-lookup"><span data-stu-id="0008d-122">Request headers</span></span>

| <span data-ttu-id="0008d-123">标头</span><span class="sxs-lookup"><span data-stu-id="0008d-123">Header</span></span>       | <span data-ttu-id="0008d-124">值</span><span class="sxs-lookup"><span data-stu-id="0008d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0008d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0008d-125">Authorization</span></span>  | <span data-ttu-id="0008d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0008d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0008d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0008d-128">Request body</span></span>
<span data-ttu-id="0008d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0008d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0008d-130">响应</span><span class="sxs-lookup"><span data-stu-id="0008d-130">Response</span></span>

<span data-ttu-id="0008d-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[schedulingGroup](../resources/schedulinggroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0008d-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0008d-132">示例</span><span class="sxs-lookup"><span data-stu-id="0008d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0008d-133">请求</span><span class="sxs-lookup"><span data-stu-id="0008d-133">Request</span></span>

<span data-ttu-id="0008d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0008d-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```
---


### <a name="response"></a><span data-ttu-id="0008d-135">响应</span><span class="sxs-lookup"><span data-stu-id="0008d-135">Response</span></span>

<span data-ttu-id="0008d-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0008d-136">The following is an example of the response.</span></span> 

><span data-ttu-id="0008d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0008d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Get a schedulingGroup by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
