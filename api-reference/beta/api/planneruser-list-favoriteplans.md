---
title: 列表 favoritePlans
description: 检索 plannerPlans 由用户标记为最喜爱的列表。 您可以通过更新 plannerUser 资源标记为最喜爱的计划。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c189b3a3a7ed6d36272c05e9614fd6d0327600d4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519120"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="78315-104">列表 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="78315-104">List favoritePlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78315-105">检索[plannerPlans](../resources/plannerplan.md)由用户标记为最喜爱的列表。</span><span class="sxs-lookup"><span data-stu-id="78315-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="78315-106">您可以按[更新 plannerUser 资源](planneruser-update.md)标记为最喜爱的计划。</span><span class="sxs-lookup"><span data-stu-id="78315-106">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="78315-107">权限</span><span class="sxs-lookup"><span data-stu-id="78315-107">Permissions</span></span>
<span data-ttu-id="78315-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78315-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78315-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="78315-110">Permission type</span></span>      | <span data-ttu-id="78315-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78315-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78315-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78315-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78315-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="78315-113">Group.Read.All</span></span>    |
|<span data-ttu-id="78315-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78315-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78315-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="78315-115">Not supported.</span></span>    |
|<span data-ttu-id="78315-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="78315-116">Application</span></span> | <span data-ttu-id="78315-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="78315-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78315-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78315-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78315-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="78315-119">Optional query parameters</span></span>
<span data-ttu-id="78315-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="78315-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78315-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="78315-121">Request headers</span></span>
| <span data-ttu-id="78315-122">名称</span><span class="sxs-lookup"><span data-stu-id="78315-122">Name</span></span>      |<span data-ttu-id="78315-123">说明</span><span class="sxs-lookup"><span data-stu-id="78315-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78315-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="78315-124">Authorization</span></span>  | <span data-ttu-id="78315-p104">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="78315-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78315-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="78315-127">Request body</span></span>
<span data-ttu-id="78315-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="78315-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="78315-129">响应</span><span class="sxs-lookup"><span data-stu-id="78315-129">Response</span></span>
<span data-ttu-id="78315-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[plannerPlan](../resources/plannerplan.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="78315-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78315-131">示例</span><span class="sxs-lookup"><span data-stu-id="78315-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78315-132">请求</span><span class="sxs-lookup"><span data-stu-id="78315-132">Request</span></span>
<span data-ttu-id="78315-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="78315-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
##### <a name="response"></a><span data-ttu-id="78315-134">响应</span><span class="sxs-lookup"><span data-stu-id="78315-134">Response</span></span>
<span data-ttu-id="78315-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="78315-135">The following is an example of the response.</span></span> 

><span data-ttu-id="78315-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="78315-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-favoriteplans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
