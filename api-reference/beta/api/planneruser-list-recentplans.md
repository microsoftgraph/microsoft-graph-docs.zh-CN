---
title: 列表 recentPlans
description: 检索 plannerPlans 用户最近查看的列表。 您可以通过更新 plannerUser 资源更新最近查看的计划。
ms.openlocfilehash: 58c4d786dfdf596df8786db93c32e88b0cf93dfd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048166"
---
# <a name="list-recentplans"></a><span data-ttu-id="01050-104">列表 recentPlans</span><span class="sxs-lookup"><span data-stu-id="01050-104">List recentPlans</span></span>

> <span data-ttu-id="01050-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01050-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01050-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01050-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01050-107">检索[plannerPlans](../resources/plannerplan.md)用户最近查看的列表。</span><span class="sxs-lookup"><span data-stu-id="01050-107">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="01050-108">您可以通过[更新 plannerUser 资源](planneruser-update.md)更新最近查看的计划。</span><span class="sxs-lookup"><span data-stu-id="01050-108">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="01050-109">权限</span><span class="sxs-lookup"><span data-stu-id="01050-109">Permissions</span></span>
<span data-ttu-id="01050-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01050-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01050-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="01050-112">Permission type</span></span>      | <span data-ttu-id="01050-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01050-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01050-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01050-114">Delegated (work or school account)</span></span> | <span data-ttu-id="01050-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="01050-115">Group.Read.All</span></span>    |
|<span data-ttu-id="01050-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01050-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01050-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="01050-117">Not supported.</span></span>    |
|<span data-ttu-id="01050-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="01050-118">Application</span></span> | <span data-ttu-id="01050-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="01050-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01050-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01050-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/<id>/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="01050-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="01050-121">Request headers</span></span>
| <span data-ttu-id="01050-122">名称</span><span class="sxs-lookup"><span data-stu-id="01050-122">Name</span></span>      |<span data-ttu-id="01050-123">说明</span><span class="sxs-lookup"><span data-stu-id="01050-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="01050-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="01050-124">Authorization</span></span>  | <span data-ttu-id="01050-p105">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="01050-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="01050-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="01050-127">Request body</span></span>
<span data-ttu-id="01050-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01050-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="01050-129">响应</span><span class="sxs-lookup"><span data-stu-id="01050-129">Response</span></span>
<span data-ttu-id="01050-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[plannerPlan](../resources/plannerplan.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="01050-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01050-131">示例</span><span class="sxs-lookup"><span data-stu-id="01050-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01050-132">请求</span><span class="sxs-lookup"><span data-stu-id="01050-132">Request</span></span>
<span data-ttu-id="01050-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="01050-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
##### <a name="response"></a><span data-ttu-id="01050-134">响应</span><span class="sxs-lookup"><span data-stu-id="01050-134">Response</span></span>
<span data-ttu-id="01050-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="01050-135">The following is an example of the response.</span></span> 

><span data-ttu-id="01050-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="01050-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
