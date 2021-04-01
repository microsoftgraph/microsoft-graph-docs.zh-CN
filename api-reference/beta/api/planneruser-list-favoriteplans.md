---
title: 列出 favoritePlans
description: 检索由用户标记为收藏的 plannerPlans 列表。 可以通过更新 plannerUser 资源将计划标记为收藏。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 1650ea55e1fc7dc6200e4985e417fdfb67fb0ee3
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473484"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="80797-104">列出 favoritePlans</span><span class="sxs-lookup"><span data-stu-id="80797-104">List favoritePlans</span></span>

<span data-ttu-id="80797-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80797-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80797-106">检索用户 [标记为收藏的 plannerPlans](../resources/plannerplan.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="80797-106">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="80797-107">可以通过更新 [plannerUser](planneruser-update.md)资源 将计划标记为收藏。</span><span class="sxs-lookup"><span data-stu-id="80797-107">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80797-108">权限</span><span class="sxs-lookup"><span data-stu-id="80797-108">Permissions</span></span>
<span data-ttu-id="80797-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80797-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80797-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="80797-111">Permission type</span></span>      | <span data-ttu-id="80797-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80797-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80797-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80797-113">Delegated (work or school account)</span></span> | <span data-ttu-id="80797-114">Tasks.Read、Tasks.ReadWrite、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="80797-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span></span>    |
|<span data-ttu-id="80797-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80797-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80797-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80797-116">Not supported.</span></span>    |
|<span data-ttu-id="80797-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="80797-117">Application</span></span> | <span data-ttu-id="80797-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="80797-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80797-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80797-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/{id}/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="80797-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80797-120">Optional query parameters</span></span>
<span data-ttu-id="80797-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80797-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80797-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="80797-122">Request headers</span></span>
| <span data-ttu-id="80797-123">名称</span><span class="sxs-lookup"><span data-stu-id="80797-123">Name</span></span>      |<span data-ttu-id="80797-124">说明</span><span class="sxs-lookup"><span data-stu-id="80797-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="80797-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="80797-125">Authorization</span></span>  | <span data-ttu-id="80797-126">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="80797-126">Bearer {code}.</span></span> <span data-ttu-id="80797-127">必需。</span><span class="sxs-lookup"><span data-stu-id="80797-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80797-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="80797-128">Request body</span></span>
<span data-ttu-id="80797-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80797-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="80797-130">响应</span><span class="sxs-lookup"><span data-stu-id="80797-130">Response</span></span>
<span data-ttu-id="80797-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [plannerPlan](../resources/plannerplan.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="80797-131">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="80797-132">示例</span><span class="sxs-lookup"><span data-stu-id="80797-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80797-133">请求</span><span class="sxs-lookup"><span data-stu-id="80797-133">Request</span></span>
<span data-ttu-id="80797-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80797-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80797-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="80797-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
# <a name="c"></a>[<span data-ttu-id="80797-136">C#</span><span class="sxs-lookup"><span data-stu-id="80797-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-favoriteplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80797-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80797-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-favoriteplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80797-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80797-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-favoriteplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80797-139">Java</span><span class="sxs-lookup"><span data-stu-id="80797-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-favoriteplans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="80797-140">响应</span><span class="sxs-lookup"><span data-stu-id="80797-140">Response</span></span>
<span data-ttu-id="80797-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80797-141">The following is an example of the response.</span></span> 

><span data-ttu-id="80797-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="80797-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
