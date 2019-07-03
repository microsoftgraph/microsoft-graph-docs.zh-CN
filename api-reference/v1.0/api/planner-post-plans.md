---
title: 创建 plannerPlan
description: 使用此 API 新建 **plannerPlan**。
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 94956443d88237c8df9bc06e6e237fbac2a288ac
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456160"
---
# <a name="create-plannerplan"></a><span data-ttu-id="6fa10-103">创建 plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6fa10-103">Create plannerPlan</span></span>

<span data-ttu-id="6fa10-104">使用此 API 新建 **plannerPlan**。</span><span class="sxs-lookup"><span data-stu-id="6fa10-104">Use this API to create a new **plannerPlan**.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fa10-105">权限</span><span class="sxs-lookup"><span data-stu-id="6fa10-105">Permissions</span></span>

<span data-ttu-id="6fa10-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fa10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6fa10-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fa10-108">Permission type</span></span>                        | <span data-ttu-id="6fa10-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fa10-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6fa10-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fa10-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fa10-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6fa10-111">Group.ReadWrite.All</span></span>                         |
| <span data-ttu-id="6fa10-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fa10-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fa10-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fa10-113">Not supported.</span></span>                              |
| <span data-ttu-id="6fa10-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fa10-114">Application</span></span>                            | <span data-ttu-id="6fa10-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6fa10-115">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="6fa10-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fa10-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
``` http
POST /planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="6fa10-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fa10-117">Request headers</span></span>

| <span data-ttu-id="6fa10-118">名称</span><span class="sxs-lookup"><span data-stu-id="6fa10-118">Name</span></span>          | <span data-ttu-id="6fa10-119">说明</span><span class="sxs-lookup"><span data-stu-id="6fa10-119">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6fa10-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fa10-120">Authorization</span></span> | <span data-ttu-id="6fa10-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fa10-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fa10-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fa10-123">Request body</span></span>

<span data-ttu-id="6fa10-p103">在请求正文中，提供 [plannerPlan](../resources/plannerplan.md) 对象的 JSON 表示形式。**plannerPlan** 所有者属性必须设为[组](../resources/group.md)对象的 id。</span><span class="sxs-lookup"><span data-stu-id="6fa10-p103">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object. The **plannerPlan** owner property must be set to an id of a [group](../resources/group.md) object.</span></span>

><span data-ttu-id="6fa10-126">**注意：** 正在创建计划的用户必须是拥有该计划的组的成员。</span><span class="sxs-lookup"><span data-stu-id="6fa10-126">**Note:** The user who is creating the plan must be a member of the group that will own the plan.</span></span> <span data-ttu-id="6fa10-127">使用“[创建组](../api/group-post-groups.md)”创建新组时，系统不会将你添加为组成员。</span><span class="sxs-lookup"><span data-stu-id="6fa10-127">When you create a new group by using [Create group](../api/group-post-groups.md), you are not added to the group as a member.</span></span> <span data-ttu-id="6fa10-128">创建组后，使用“[组帖子成员](../api/group-post-members.md)”将自己添加为成员。</span><span class="sxs-lookup"><span data-stu-id="6fa10-128">After the group is created, add yourself as a member by using [group post members](../api/group-post-members.md).</span></span>


## <a name="response"></a><span data-ttu-id="6fa10-129">响应</span><span class="sxs-lookup"><span data-stu-id="6fa10-129">Response</span></span>

<span data-ttu-id="6fa10-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [plannerPlan](../resources/plannerplan.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fa10-130">If successful, this method returns `201 Created` response code and [plannerPlan](../resources/plannerplan.md) object in the response body.</span></span>

<span data-ttu-id="6fa10-p105">此方法可以返回任何 [HTTP 状态代码](/graph/errors)。应用应当为此方法的处理最常见的错误为 400、403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner-overview.md#common-planner-error-conditions)。</span><span class="sxs-lookup"><span data-stu-id="6fa10-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="6fa10-134">示例</span><span class="sxs-lookup"><span data-stu-id="6fa10-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="6fa10-135">请求</span><span class="sxs-lookup"><span data-stu-id="6fa10-135">Request</span></span>

<span data-ttu-id="6fa10-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6fa10-136">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6fa10-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="6fa10-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_planner"
}-->
``` http
POST https://graph.microsoft.com/v1.0/planner/plans
Content-type: application/json
Content-length: 381

{
  "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
  "title": "title-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fa10-138">C#</span><span class="sxs-lookup"><span data-stu-id="6fa10-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-plannerplan-from-planner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fa10-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="6fa10-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-plannerplan-from-planner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fa10-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="6fa10-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-plannerplan-from-planner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="6fa10-141">在请求正文中，提供 [plannerPlan](../resources/plannerplan.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fa10-141">In the request body, supply a JSON representation of [plannerPlan](../resources/plannerplan.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="6fa10-142">响应</span><span class="sxs-lookup"><span data-stu-id="6fa10-142">Response</span></span>

<span data-ttu-id="6fa10-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6fa10-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "tocPath": "",
  "suppressions": [
  ]
}-->
