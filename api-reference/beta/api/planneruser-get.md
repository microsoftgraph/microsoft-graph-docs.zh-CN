---
title: 获取 plannerUser
description: '检索 plannerUser 对象的属性和关系。 返回的属性包括用户的收藏计划和最近查看的计划。 '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f87a84d9297fbbde1d5fb9d6045dadae10e6bd72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455576"
---
# <a name="get-planneruser"></a><span data-ttu-id="f0f53-104">获取 plannerUser</span><span class="sxs-lookup"><span data-stu-id="f0f53-104">Get plannerUser</span></span>

<span data-ttu-id="f0f53-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f0f53-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0f53-106">检索[plannerUser](../resources/planneruser.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0f53-106">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="f0f53-107">返回的属性包括用户的收藏计划和最近查看的计划。</span><span class="sxs-lookup"><span data-stu-id="f0f53-107">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="f0f53-108">权限</span><span class="sxs-lookup"><span data-stu-id="f0f53-108">Permissions</span></span>
<span data-ttu-id="f0f53-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0f53-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0f53-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0f53-111">Permission type</span></span>      | <span data-ttu-id="f0f53-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0f53-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0f53-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0f53-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f0f53-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0f53-114">Group.Read.All</span></span>    |
|<span data-ttu-id="f0f53-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0f53-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0f53-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0f53-116">Not supported.</span></span>    |
|<span data-ttu-id="f0f53-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0f53-117">Application</span></span> | <span data-ttu-id="f0f53-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0f53-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0f53-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0f53-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/{id}/planner
```

## <a name="request-headers"></a><span data-ttu-id="f0f53-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0f53-120">Request headers</span></span>
| <span data-ttu-id="f0f53-121">名称</span><span class="sxs-lookup"><span data-stu-id="f0f53-121">Name</span></span>      |<span data-ttu-id="f0f53-122">说明</span><span class="sxs-lookup"><span data-stu-id="f0f53-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0f53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0f53-123">Authorization</span></span>  | <span data-ttu-id="f0f53-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="f0f53-124">Bearer {code}.</span></span> <span data-ttu-id="f0f53-125">必需。</span><span class="sxs-lookup"><span data-stu-id="f0f53-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0f53-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0f53-126">Request body</span></span>
<span data-ttu-id="f0f53-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0f53-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f0f53-128">响应</span><span class="sxs-lookup"><span data-stu-id="f0f53-128">Response</span></span>
<span data-ttu-id="f0f53-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[plannerUser](../resources/planneruser.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f0f53-129">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0f53-130">示例</span><span class="sxs-lookup"><span data-stu-id="f0f53-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0f53-131">请求</span><span class="sxs-lookup"><span data-stu-id="f0f53-131">Request</span></span>
<span data-ttu-id="f0f53-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f0f53-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="f0f53-133">响应</span><span class="sxs-lookup"><span data-stu-id="f0f53-133">Response</span></span>
<span data-ttu-id="f0f53-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f0f53-134">The following is an example of the response.</span></span> 

><span data-ttu-id="f0f53-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f0f53-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
