---
title: 获取 plannerUser
description: '检索 plannerUser 对象的属性和关系。 返回的属性包括用户最喜爱的计划和最近查看的计划。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 05e192b4b57f06b84eca8325ae08960bb74839af
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473331"
---
# <a name="get-planneruser"></a><span data-ttu-id="e99c4-104">获取 plannerUser</span><span class="sxs-lookup"><span data-stu-id="e99c4-104">Get plannerUser</span></span>

<span data-ttu-id="e99c4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e99c4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e99c4-106">检索 [plannerUser](../resources/planneruser.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e99c4-106">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="e99c4-107">返回的属性包括用户最喜爱的计划和最近查看的计划。</span><span class="sxs-lookup"><span data-stu-id="e99c4-107">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="e99c4-108">权限</span><span class="sxs-lookup"><span data-stu-id="e99c4-108">Permissions</span></span>
<span data-ttu-id="e99c4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e99c4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e99c4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e99c4-111">Permission type</span></span>      | <span data-ttu-id="e99c4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e99c4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e99c4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e99c4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e99c4-114">Tasks.Read、Tasks.ReadWrite、Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="e99c4-114">Tasks.Read, Tasks.ReadWrite, Group.Read.All</span></span>    |
|<span data-ttu-id="e99c4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e99c4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e99c4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e99c4-116">Not supported.</span></span>    |
|<span data-ttu-id="e99c4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e99c4-117">Application</span></span> | <span data-ttu-id="e99c4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e99c4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e99c4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e99c4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/{id}/planner
```

## <a name="request-headers"></a><span data-ttu-id="e99c4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e99c4-120">Request headers</span></span>
| <span data-ttu-id="e99c4-121">名称</span><span class="sxs-lookup"><span data-stu-id="e99c4-121">Name</span></span>      |<span data-ttu-id="e99c4-122">说明</span><span class="sxs-lookup"><span data-stu-id="e99c4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e99c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e99c4-123">Authorization</span></span>  | <span data-ttu-id="e99c4-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="e99c4-124">Bearer {code}.</span></span> <span data-ttu-id="e99c4-125">必需。</span><span class="sxs-lookup"><span data-stu-id="e99c4-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e99c4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e99c4-126">Request body</span></span>
<span data-ttu-id="e99c4-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e99c4-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e99c4-128">响应</span><span class="sxs-lookup"><span data-stu-id="e99c4-128">Response</span></span>
<span data-ttu-id="e99c4-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [plannerUser](../resources/planneruser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e99c4-129">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e99c4-130">示例</span><span class="sxs-lookup"><span data-stu-id="e99c4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e99c4-131">请求</span><span class="sxs-lookup"><span data-stu-id="e99c4-131">Request</span></span>
<span data-ttu-id="e99c4-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e99c4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e99c4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e99c4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_planneruser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner
```
# <a name="c"></a>[<span data-ttu-id="e99c4-134">C#</span><span class="sxs-lookup"><span data-stu-id="e99c4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-planneruser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e99c4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e99c4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-planneruser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e99c4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e99c4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-planneruser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e99c4-137">Java</span><span class="sxs-lookup"><span data-stu-id="e99c4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-planneruser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e99c4-138">响应</span><span class="sxs-lookup"><span data-stu-id="e99c4-138">Response</span></span>
<span data-ttu-id="e99c4-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e99c4-139">The following is an example of the response.</span></span> 

><span data-ttu-id="e99c4-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e99c4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


