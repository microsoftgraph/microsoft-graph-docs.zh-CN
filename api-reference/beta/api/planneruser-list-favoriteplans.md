---
title: 列出 favoritePlans
description: 检索标记为用户收藏的 plannerPlans 的列表。 您可以通过更新 plannerUser 资源将计划标记为收藏。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: a0cf327148b75970c5e049850e83141751764cf0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33332321"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="5e61d-104">列出 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="5e61d-104">List favoritePlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e61d-105">检索标记为用户收藏的[plannerPlans](../resources/plannerplan.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="5e61d-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="5e61d-106">您可以通过[更新 plannerUser 资源](planneruser-update.md)将计划标记为收藏。</span><span class="sxs-lookup"><span data-stu-id="5e61d-106">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e61d-107">权限</span><span class="sxs-lookup"><span data-stu-id="5e61d-107">Permissions</span></span>
<span data-ttu-id="5e61d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e61d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e61d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e61d-110">Permission type</span></span>      | <span data-ttu-id="5e61d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e61d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e61d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e61d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5e61d-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e61d-113">Group.Read.All</span></span>    |
|<span data-ttu-id="5e61d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e61d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e61d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e61d-115">Not supported.</span></span>    |
|<span data-ttu-id="5e61d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e61d-116">Application</span></span> | <span data-ttu-id="5e61d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e61d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e61d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e61d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5e61d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5e61d-119">Optional query parameters</span></span>
<span data-ttu-id="5e61d-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5e61d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e61d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e61d-121">Request headers</span></span>
| <span data-ttu-id="5e61d-122">名称</span><span class="sxs-lookup"><span data-stu-id="5e61d-122">Name</span></span>      |<span data-ttu-id="5e61d-123">说明</span><span class="sxs-lookup"><span data-stu-id="5e61d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e61d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e61d-124">Authorization</span></span>  | <span data-ttu-id="5e61d-125">持有者 {代码}。</span><span class="sxs-lookup"><span data-stu-id="5e61d-125">Bearer {code}.</span></span> <span data-ttu-id="5e61d-126">必填。</span><span class="sxs-lookup"><span data-stu-id="5e61d-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e61d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e61d-127">Request body</span></span>
<span data-ttu-id="5e61d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5e61d-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5e61d-129">响应</span><span class="sxs-lookup"><span data-stu-id="5e61d-129">Response</span></span>
<span data-ttu-id="5e61d-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[plannerPlan](../resources/plannerplan.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="5e61d-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e61d-131">示例</span><span class="sxs-lookup"><span data-stu-id="5e61d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e61d-132">请求</span><span class="sxs-lookup"><span data-stu-id="5e61d-132">Request</span></span>
<span data-ttu-id="5e61d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e61d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
##### <a name="response"></a><span data-ttu-id="5e61d-134">响应</span><span class="sxs-lookup"><span data-stu-id="5e61d-134">Response</span></span>
<span data-ttu-id="5e61d-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5e61d-135">The following is an example of the response.</span></span> 

><span data-ttu-id="5e61d-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5e61d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtUGxhbiAgQEBAQEBAQEBAQEBAQEBDXCc=\"",
      "createdBy": {
        "user": {
          "id": "dd8a8379-1ac1-4eee-861d-ec15f6fa3611"
        },
        "application": {
          "id": "09abbdfd-ed23-44ee-a2d9-a627aa1c90f3"
        }
      },
      "createdDateTime": "2015-10-14T00:57:28.4698344Z",
      "owner": "eacd01dd-84cc-4c12-bd8a-9a33e5aeed11",
      "title": "Budget Planning (2016)",
      "id": "uZWtCtli30CGoWLIWSat1mQAC0ai"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List favoritePlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
