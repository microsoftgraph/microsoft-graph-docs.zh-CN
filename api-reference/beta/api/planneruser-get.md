---
title: 获取 plannerUser
description: '检索的属性和 plannerUser 对象的关系。 返回的属性包括用户的收藏夹计划和最近查看的计划。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 742d29d65c5d80db96c8cff199e25465f7a80dd7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915989"
---
# <a name="get-planneruser"></a><span data-ttu-id="7cfe2-104">获取 plannerUser</span><span class="sxs-lookup"><span data-stu-id="7cfe2-104">Get plannerUser</span></span>

> <span data-ttu-id="7cfe2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cfe2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7cfe2-107">检索的属性和[plannerUser](../resources/planneruser.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-107">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="7cfe2-108">返回的属性包括用户的收藏夹计划和最近查看的计划。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-108">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="7cfe2-109">权限</span><span class="sxs-lookup"><span data-stu-id="7cfe2-109">Permissions</span></span>
<span data-ttu-id="7cfe2-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cfe2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cfe2-112">Permission type</span></span>      | <span data-ttu-id="7cfe2-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cfe2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cfe2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cfe2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7cfe2-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cfe2-115">Group.Read.All</span></span>    |
|<span data-ttu-id="7cfe2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cfe2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cfe2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-117">Not supported.</span></span>    |
|<span data-ttu-id="7cfe2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cfe2-118">Application</span></span> | <span data-ttu-id="7cfe2-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cfe2-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cfe2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/<id>/planner
```

## <a name="request-headers"></a><span data-ttu-id="7cfe2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cfe2-121">Request headers</span></span>
| <span data-ttu-id="7cfe2-122">名称</span><span class="sxs-lookup"><span data-stu-id="7cfe2-122">Name</span></span>      |<span data-ttu-id="7cfe2-123">说明</span><span class="sxs-lookup"><span data-stu-id="7cfe2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7cfe2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cfe2-124">Authorization</span></span>  | <span data-ttu-id="7cfe2-p105">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cfe2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cfe2-127">Request body</span></span>
<span data-ttu-id="7cfe2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7cfe2-129">响应</span><span class="sxs-lookup"><span data-stu-id="7cfe2-129">Response</span></span>
<span data-ttu-id="7cfe2-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[plannerUser](../resources/planneruser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-130">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7cfe2-131">示例</span><span class="sxs-lookup"><span data-stu-id="7cfe2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cfe2-132">请求</span><span class="sxs-lookup"><span data-stu-id="7cfe2-132">Request</span></span>
<span data-ttu-id="7cfe2-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="7cfe2-134">响应</span><span class="sxs-lookup"><span data-stu-id="7cfe2-134">Response</span></span>
<span data-ttu-id="7cfe2-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-135">The following is an example of the response.</span></span> 

><span data-ttu-id="7cfe2-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7cfe2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
