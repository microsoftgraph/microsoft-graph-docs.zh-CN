---
title: 列出 recentPlans
description: 检索用户最近查看过的 plannerPlans 列表。 您可以通过更新 plannerUser 资源更新最近查看过的计划。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: d0fe691e1a0cb34fcc29215fafe4784ca85cdc63
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264272"
---
# <a name="list-recentplans"></a><span data-ttu-id="85436-104">列出 recentPlans</span><span class="sxs-lookup"><span data-stu-id="85436-104">List recentPlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85436-105">检索用户最近查看过的[plannerPlans](../resources/plannerplan.md)列表。</span><span class="sxs-lookup"><span data-stu-id="85436-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="85436-106">您可以通过[更新 plannerUser 资源](planneruser-update.md)更新最近查看过的计划。</span><span class="sxs-lookup"><span data-stu-id="85436-106">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="85436-107">权限</span><span class="sxs-lookup"><span data-stu-id="85436-107">Permissions</span></span>
<span data-ttu-id="85436-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85436-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85436-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="85436-110">Permission type</span></span>      | <span data-ttu-id="85436-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85436-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85436-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85436-112">Delegated (work or school account)</span></span> | <span data-ttu-id="85436-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="85436-113">Group.Read.All</span></span>    |
|<span data-ttu-id="85436-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85436-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85436-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="85436-115">Not supported.</span></span>    |
|<span data-ttu-id="85436-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="85436-116">Application</span></span> | <span data-ttu-id="85436-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="85436-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85436-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85436-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/<id>/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="85436-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="85436-119">Request headers</span></span>
| <span data-ttu-id="85436-120">名称</span><span class="sxs-lookup"><span data-stu-id="85436-120">Name</span></span>      |<span data-ttu-id="85436-121">说明</span><span class="sxs-lookup"><span data-stu-id="85436-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85436-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85436-122">Authorization</span></span>  | <span data-ttu-id="85436-123">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="85436-123">Bearer {code}.</span></span> <span data-ttu-id="85436-124">必需。</span><span class="sxs-lookup"><span data-stu-id="85436-124">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="85436-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="85436-125">Request body</span></span>
<span data-ttu-id="85436-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="85436-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="85436-127">响应</span><span class="sxs-lookup"><span data-stu-id="85436-127">Response</span></span>
<span data-ttu-id="85436-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[plannerPlan](../resources/plannerplan.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="85436-128">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85436-129">示例</span><span class="sxs-lookup"><span data-stu-id="85436-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85436-130">请求</span><span class="sxs-lookup"><span data-stu-id="85436-130">Request</span></span>
<span data-ttu-id="85436-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="85436-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
##### <a name="response"></a><span data-ttu-id="85436-132">响应</span><span class="sxs-lookup"><span data-stu-id="85436-132">Response</span></span>
<span data-ttu-id="85436-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="85436-133">The following is an example of the response.</span></span> 

><span data-ttu-id="85436-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="85436-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="85436-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="85436-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="85436-137">C#</span><span class="sxs-lookup"><span data-stu-id="85436-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_recentplans-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85436-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="85436-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_recentplans-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="85436-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="85436-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_recentplans-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-recentplans.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/planneruser-list-recentplans.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/planneruser-list-recentplans.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
