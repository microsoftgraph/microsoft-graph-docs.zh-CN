---
title: 创建 plannerPlan
description: 使用此 API 新建 **plannerPlan**。
localization_priority: Normal
ms.openlocfilehash: 6f0b2dcca22aa065c0c05d990813d84865c56241
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840178"
---
# <a name="create-plannerplan"></a><span data-ttu-id="00281-103">创建 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="00281-103">Create plannerPlan</span></span>

> <span data-ttu-id="00281-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00281-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00281-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00281-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00281-106">使用此 API 新建 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="00281-106">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="00281-107">权限</span><span class="sxs-lookup"><span data-stu-id="00281-107">Permissions</span></span>

<span data-ttu-id="00281-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="00281-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="00281-110">Permission type</span></span>                        | <span data-ttu-id="00281-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00281-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="00281-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00281-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="00281-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00281-113">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="00281-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00281-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00281-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="00281-115">Not supported.</span></span>                              |
| <span data-ttu-id="00281-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="00281-116">Application</span></span>                            | <span data-ttu-id="00281-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="00281-117">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="00281-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00281-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="00281-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="00281-119">Request headers</span></span>

| <span data-ttu-id="00281-120">名称</span><span class="sxs-lookup"><span data-stu-id="00281-120">Name</span></span>          | <span data-ttu-id="00281-121">说明</span><span class="sxs-lookup"><span data-stu-id="00281-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="00281-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00281-122">Authorization</span></span> | <span data-ttu-id="00281-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00281-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00281-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="00281-125">Request body</span></span>

<span data-ttu-id="00281-p104">在请求正文中，提供 [plannerPlan](../resources/plannerplan.md) 对象的 JSON 表示形式。**plannerPlan** 所有者属性必须设为[组](../resources/group.md)对象的 id。</span><span class="sxs-lookup"><span data-stu-id="00281-p104">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="00281-128">**注意：** 正在创建计划的用户必须将拥有计划的组的成员。</span><span class="sxs-lookup"><span data-stu-id="00281-128">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="00281-129">当使用[创建组](../api/group-post-groups.md)创建一个新的组时，您不是添加到组，作为成员。</span><span class="sxs-lookup"><span data-stu-id="00281-129">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="00281-130">创建组后，将自己添加为成员使用[组发布成员](../api/group-post-members.md)。</span><span class="sxs-lookup"><span data-stu-id="00281-130">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>

## <a name="response"></a><span data-ttu-id="00281-131">响应</span><span class="sxs-lookup"><span data-stu-id="00281-131">Response</span></span>

<span data-ttu-id="00281-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerPlan](../resources/plannerplan.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00281-132">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="00281-p106">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法的处理最常见的错误为 400、403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="00281-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="00281-136">示例</span><span class="sxs-lookup"><span data-stu-id="00281-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="00281-137">请求</span><span class="sxs-lookup"><span data-stu-id="00281-137">Request</span></span>

<span data-ttu-id="00281-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00281-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/beta/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```

<span data-ttu-id="00281-139">在请求正文中，提供 [plannerPlan](../resources/plannerplan.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00281-139">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="00281-140">响应</span><span class="sxs-lookup"><span data-stu-id="00281-140">Response</span></span>

<span data-ttu-id="00281-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00281-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan"
} -->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 357

{
  "createdBy": {
    "application": {
      "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
    },
    "user": {
      "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
    }
  },
  "createdDateTime": "2015-03-30T18:36:49.2407981Z",
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value",
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
